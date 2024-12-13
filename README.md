# Xenonstack-Task2-
sysopctl - System Resource and Task Manager
Overview
sysopctl is a custom command-line tool designed to manage system services, processes, and overall system health. This script provides an intuitive interface for Linux system administrators to perform essential tasks such as monitoring services, analyzing logs, and managing system resources.

Features
Section A: Basic Features
Manual Page: Access documentation using man sysopctl.
Help Option: View usage instructions and examples with sysopctl --help.
Version Information: Display the current version of the tool using sysopctl --version.
Section B: System Management Operations
Level Easy
List Running Services:
Command:


sysopctl service list
Outputs a list of all active services (similar to systemctl list-units --type=service).

View System Load:
Command:


sysopctl system load
Outputs the current system load averages (like uptime).

Level Intermediate
Manage System Services:

Start a service:

sysopctl service start <service-name>
Stop a service:

sysopctl service stop <service-name>
Outputs status updates confirming the start or stop of services.

Check Disk Usage:
Command:


sysopctl disk usage

Outputs disk usage statistics by partition (like df -h).

Level Advanced
Monitor System Processes:
Command:


sysopctl process monitor

Outputs real-time process activity (like top or htop).

Analyze System Logs:
Command:


sysopctl logs analyze
Outputs a summary of recent critical log entries using tools like journalctl.

Backup System Files:

Command:


sysopctl backup <path>
Initiates a backup process and provides status updates (using rsync for file transfers).

Requirements

Operating System: Linux

Tools/Dependencies:

Bash Shell

Utilities: systemctl, uptime, journalctl, df, rsync, top

Installation

Clone the repository:

git clone <repository-url>

Navigate to the project directory:

cd sysopctl

Make the script executable:

chmod +x sysopctl

Move it to a directory in your PATH (e.g., /usr/local/bin):

sudo mv sysopctl /usr/local/bin/


Help Option

To see all available commands and usage examples:


sysopctl --help

Version Information

To check the current version:


sysopctl --version

Managing Services

To list active services:


sysopctl service list

To start or stop a service:


sysopctl service start <service-name>

sysopctl service stop <service-name>

Disk Usage

To check disk usage statistics:


sysopctl disk usage
