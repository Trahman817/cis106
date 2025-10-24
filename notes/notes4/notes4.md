# Notes 4

## How to install and remove software using the APT command

APT stands for Advanced Package Tool — it’s a command-line utility used to install, update, upgrade, and remove software packages in Debian-based Linux distributions.

Installing Software with APT
1. Update the Package List

Before installing anything, it’s best to update our package list so APT knows about the latest available software versions.
bash sudo apt update
2. Install a Package

Update package list	
## Command sudo apt update
Install package	
## Command sudo apt install <package>
Remove package (keep config)	
## Command sudo apt remove <package>
Remove package (delete config)	
## Command sudo apt purge <package>
Remove unused packages	
## Command sudo apt autoremove
Upgrade system	
## Command sudo apt upgrade

## How to create a shell script step by step including screenshots and how to run it. Try to be as detailed as possible.

1) Pick (or create) a file for script

bash vim example_script.sh
2) Add the shebang and script content

At the top of the file put a shebang so the system knows which shell to use:

#!/usr/bin/env bash
# example_script.sh - demo of a shell script with args, functions, and simple logic
# Usage:
#   ./example_script.sh NAME TIMES
# Example:
#   ./example_script.sh Alice 3

set -euo pipefail
IFS=$'\n\t'

# --- helper functions ---
log() {
  # print a timestamped message to stdout
  printf '%s %s\n' "$(date +'%Y-%m-%d %H:%M:%S')" "$*"
}

usage() {
  cat <<EOF
Usage: $0 NAME TIMES
  NAME   - name to greet
  TIMES  - how many times to print the greeting (positive integer)
EOF
}

# --- parse args ---
if [[ "${1:-}" == "-h" || "${1:-}" == "--help" ]]; then
  usage
  exit 0
fi

NAME="${1:-World}"
TIMES="${2:-1}"

# validate TIMES is a positive integer
if ! [[ "$TIMES" =~ ^[0-9]+$ ]] || [ "$TIMES" -le 0 ]; then
  log "ERROR: TIMES must be a positive integer."
  usage
  exit 2
fi

# --- main work ---
log "Starting greetings: NAME=$NAME TIMES=$TIMES"
for ((i=1;i<=TIMES;i++)); do
  printf "Hello, %s! (greeting %d/%d)\n" "$NAME" "$i" "$TIMES"
  sleep 0.2
done
log "Done."

3) Save the file and make it executable

From the terminal run:
chmod +x example_script.sh
You can verify it’s executable:
ls -l example_script.sh
# -rwxr-xr-x ... means executable
4) Run the script

Run with positional arguments (or let defaults apply):
./example_script.sh Alice 3

