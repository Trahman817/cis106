
# Question no 1
## What are the server hardware specifications (virtual machine settings)? Take a screenshot - don’t type it!
![img](question1.png)
# Question 2
## What is the Debian Login Screen? (Take screenshot - do not type it!)
![img](question2%20(Edited).png)
# Question 3
## What is the IP address of your Debian Server Virtual Machine? (type the command and show a screenshot of the commands output)
Command line: hostname -I 
![img](question3.png)
 # Question 4
 ## How do you work with the Firewall in Debian? (Type and explain what each command does)## Question no 4

## UFW Firewall Commands – Summary Table (Debian)

| Task | Command | Explanation |
|------|---------|-------------|
| Install UFW | `sudo apt install ufw` | Installs the Uncomplicated Firewall package |
| Enable firewall | `sudo ufw enable` | Turns the firewall on and enables it at startup |
| Check firewall status | `sudo ufw status` | Displays firewall status and active rules |
| Disable firewall | `sudo ufw disable` | Turns the firewall off |
| Default rule: deny incoming | `sudo ufw default deny incoming` | Blocks all incoming connections by default |
| Default rule: allow outgoing | `sudo ufw default allow outgoing` | Allows all outgoing connections |
| Allow Apache | `sudo ufw allow 'Apache Full'` | Allows HTTP (80) and HTTPS (443) traffic |
| Reload firewall | `sudo ufw reload` | Applies firewall rule changes immediately |

![img](question3.1.png)
![img](question3.2.png)
![img](question3.3.png)
![img](question3.4.png)
![img](question3.5.png)
# Question 5
## What different commands do we use to work with Apache? 
## Apache Configuration Files and Directories (Debian)

| File / Directory | Purpose |
|------------------|---------|
| `apache2.conf` | Main Apache configuration file |
| `ports.conf` | Defines which ports Apache listens on |
| `envvars` | Sets environment variables used by Apache |
| `sites-available/` | Stores available virtual host configuration files |
| `sites-enabled/` | Contains enabled virtual host configurations (symbolic links) |
| `mods-available/` | Stores available Apache modules |
| `mods-enabled/` | Contains enabled Apache modules (symbolic links) |
| `conf-available/` | Stores additional Apache configuration files |
| `conf-enabled/` | Contains enabled extra configuration files |

What is the command you use to check if Apache is running?
  * The command is: systemctl status apache2
![img](question5.1.png)
What is the command you use to stop Apache?
  * The command is: sudo systemctl stop apache2 
![img](question5.2.png)
What is the command you use to restart Apache?
  * sudo systemctl restart apache2
![img](question5_3.png)
What is the command used to test Apache configuration?
  * The command is: sudo apachectl configtest
![img](question5_3(1).png)
What is the command used to check the installed version of Apache?
  * /usr/sbin/apache2 -v
![img](question5.5.png)
# Question 6
## What are some common configuration files for Apache?
![img](question6.png)
# Question 7
## Where does Apache store logs?
  * Apache logs are stored at: /var/log
![img](question7.png)
What are some basic commands we can use to review logs?
## Basic Commands to Review Apache Logs

The most basic commands used to review Apache log files are:

| Command | Purpose |
|--------|---------|
| `cat` | Displays the entire log file |
| `less` | Views log files one page at a time |
| `more` | Simple paged log viewer |
| `tail` | Shows the last lines of a log file |
| `tail -f` | Monitors log files in real time |
| `head` | Shows the first lines of a log file |
| `grep` | Searches for specific text patterns in logs |
| `wc -l` | Counts the number of entries (lines) in a log file |

![img](question8.png)


