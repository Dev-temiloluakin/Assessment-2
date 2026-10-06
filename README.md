# Assessment-2
# Assessment 2 — Git, Linux & Cron

This project was completed as part of **Assessment 2**, covering fundamental concepts and practical tasks in **Git, GitHub, Linux file permissions, shell scripting, system uptime monitoring, and cron job scheduling**.

## Project Overview

The assessment demonstrates practical Linux and DevOps fundamentals through the creation, execution, scheduling, and version control of a simple system-monitoring script.

The main task is to create a Bash script that records the current date/time and system uptime in a log file and automatically executes the script every five minutes using `cron`.

## Objectives

The project covers the following:

* Understanding the difference between **Git** and **GitHub**
* Understanding Linux file permissions and the `chmod +x` command
* Understanding how **cron** scheduling works
* Creating and managing a Git repository
* Writing and executing a Bash shell script
* Recording system uptime information
* Scheduling automated tasks with `cron`
* Committing and pushing project files to GitHub

## Project Structure

```text
Assessment-2/
├── README.md
└── log-uptime.sh
```

## `log-uptime.sh`

The `log-uptime.sh` script records the current date and time together with the system's uptime and appends the information to:

```text
/var/log/uptime.log
```

The script uses the append operation so that previous entries are preserved rather than overwritten.

Example output:

```text
2026-10-06 12:00:01 - Uptime: up 2 hours, 15 minutes
2026-10-06 12:05:01 - Uptime: up 2 hours, 20 minutes
```

## Making the Script Executable

The script is given execute permission using:

```bash
chmod +x log-uptime.sh
```

This allows the script to be executed directly as a program.

## Cron Scheduling

The script is scheduled to run automatically every five minutes using `cron`.

The cron schedule is:

```text
*/5 * * * * /path/to/log-uptime.sh
```

This means the script runs once every five minutes, every hour, every day.

## Git & GitHub

Git is used for **version control**, allowing changes to the project to be tracked through commits.

GitHub is used as the **remote repository**, allowing the project and its Git history to be stored and accessed online.

The project was initialized as a Git repository, committed with a meaningful commit message, and pushed to GitHub.

## Technologies Used

* **Linux / Ubuntu**
* **Bash**
* **Git**
* **GitHub**
* **Cron**

## Learning Outcomes

Through this assessment, I gained practical experience with:

1. Linux file permissions
2. Bash scripting
3. System monitoring
4. Automated task scheduling
5. Git repository management
6. GitHub remote repositories
7. Basic DevOps automation concepts

## Assessment Submission

**Assessment:** Assessment 2
**Deadline:** 8 October 2026, 11:59 PM WAT

This repository contains the practical files associated with the assessment.

