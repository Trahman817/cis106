# Deliverable 1

## 1. What is a web server?
A **web server** is a software application that serves web pages to users over the internet or an intranet using the HTTP/HTTPS protocols. It listens for incoming requests from clients (like web browsers) and responds with requested web content (HTML, CSS, JS, images).  
**Example:** Apache HTTP Server.

---

## 2. Different web server applications

| Web Server | Definition | Website / Download | Operating System | Latest Version |
|------------|-----------|-----------------|----------------|----------------|
| **Apache HTTP Server** | Open-source web server software that serves web pages over HTTP/HTTPS. | [https://httpd.apache.org/](https://httpd.apache.org/) | Linux, Windows, macOS | 2.4.57 |
| **Nginx** | Lightweight, high-performance web server and reverse proxy server. | [https://nginx.org/](https://nginx.org/) | Linux, Windows, macOS | 1.26.1 |
| **Microsoft IIS** | Web server developed by Microsoft for hosting web applications. | [https://www.iis.net/](https://www.iis.net/) | Windows | 10.0 |
| **LiteSpeed** | High-performance commercial web server with free OpenLiteSpeed version. | [https://www.litespeedtech.com/](https://www.litespeedtech.com/) | Linux, Windows | OpenLiteSpeed 1.8.29 |


## 3. What is virtualization?
**Virtualization** is the process of creating a virtual version of something, such as an operating system, server, storage device, or network resource. It allows multiple virtual systems to run on a single physical machine.

---

## 4. What is VirtualBox?
**VirtualBox** is a free and open-source virtualization software that allows users to create and run virtual machines on their computers. It supports running multiple operating systems simultaneously on a host machine.

---

## 5. What is a virtual machine?
A **virtual machine (VM)** is a software-based emulation of a physical computer that runs an operating system and applications as if it were a real computer.

---

## 6. Host machine vs Guest machine
- **Host machine:** The physical computer that runs virtualization software.  
- **Guest machine:** The virtual machine that runs on the host system.

---

## 7. What is Debian?
**Debian** is a free and open-source Linux distribution known for stability and security. It serves as a base for many other distributions like Ubuntu.

---

## 8. What is a firewall?
A **firewall** is a network security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules.

---

## 9. What is SSH?
**SSH (Secure Shell)** is a network protocol that allows secure remote login and command execution over an encrypted connection.

---

## 10. What is an IP Address?
An **IP Address** is a unique identifier assigned to a device on a network. It allows devices to communicate over a network using the Internet Protocol.

---

## 11. What is a network mask?
A **network mask** (or subnet mask) defines which portion of an IP address represents the network and which portion represents the host.  
**Example:** `255.255.255.0`

---

## 12. What is a port?
A **port** is a numerical identifier for a communication endpoint in networking. It allows multiple services to run on the same IP address.  
**Example:** HTTP uses port 80.

---

## 13. What is port forwarding?
**Port forwarding** is a technique that allows external devices to access services on a private network by mapping a port from the router to a specific device on the internal network.

---

## 14. What is localhost?
**Localhost** is a hostname that refers to the local computer. It is used to access network services running on the same machine.

---

## 15. What does the IP address 127.0.0.1 represent?
The IP `127.0.0.1` is the **loopback address** that points to the local machine, used to test networking and software locally.

---

## 16. What is Git?
**Git** is a distributed version control system used to track changes in source code during software development.

---

## 17. What is GitHub?
**GitHub** is a web-based platform that hosts Git repositories. It provides collaboration, version control, and project management tools for developers.  
Website: [https://github.com](https://github.com)

---
## Concepts I Did Not Understand

- **Systemctl:** I was not sure how to manage services with `systemctl`.  
  **Research:** `systemctl` is a command-line tool for controlling `systemd` services. You can start, stop, enable, or check the status of services.  
  Example: `systemctl status apache2` checks if the Apache server is running.

- **SSH keys:** I did not fully understand how SSH keys work for secure login.  
  **Research:** SSH keys use a public/private key pair. The public key is stored on the server, and the private key stays on the client. This allows passwordless and encrypted authentication.

- **Firewall rules:** I was unsure how firewall rules are applied in Linux.  
  **Research:** Firewalls filter network traffic. Using `ufw` or `iptables`, you can allow or block traffic on specific ports and protocols.

- **Port forwarding:** I was confused about how external ports connect to internal devices.  
  **Research:** Port forwarding maps a port on a router to a device inside a private network. Example: forwarding port 8080 to a local web server at `192.168.1.10`.

- **Subnet mask:** I did not understand how subnet masks divide networks.  
  **Research:** A subnet mask separates the network and host portions of an IP address. Example: `255.255.255.0` means the first 3 octets are network, the last octet is for hosts.

- **Virtual machines:** I was unclear about how resources are shared between host and guest machines.  
  **Research:** A virtual machine runs an operating system in software. CPU, RAM, and disk are allocated to the VM, while the host machine controls overall resources.

- **Git staging vs commit:** I did not understand the difference between staging and committing changes.  
  **Research:** Staging (`git add`) selects changes for the next commit. Committing (`git commit`) saves these changes to the local repository.

- **Loopback / localhost:** I was unsure why `127.0.0.1` works for testing without an internet connection.  
  **Research:** The loopback interface sends network traffic back to the same machine. `127.0.0.1` (localhost) is used to test services locally without network access.
