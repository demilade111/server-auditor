# Server Health & Compliance Auditor

A lightweight Bash-based auditing tool for Linux servers.  
Collects key system health metrics, service statuses, and OS facts, and saves them in timestamped reports.

## Features (current)
- **CPU load** (1-minute average)
- **Memory usage** (% used)
- **Disk usage** (% used on `/`)
- **Inode usage** (% used on `/`)
- **Service status** (from `config/services.list`)
- **OS facts** (hostname, kernel version, uptime)

## Project Structure
