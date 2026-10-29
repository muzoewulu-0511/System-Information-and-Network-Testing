
# Linux System Information & Network Connectivity Testing

![Linux](https://img.shields.io/badge/OS-Kali%20Linux-557C94?logo=kalilinux&logoColor=white)
![Networking](https://img.shields.io/badge/Focus-Networking%20Fundamentals-blue)
![System Administration](https://img.shields.io/badge/Focus-System%20Administration-orange)
![Project Type](https://img.shields.io/badge/Type-Practical%20Lab-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## Project Overview

This project demonstrates foundational Linux system administration and networking skills through practical exercises performed in a Kali Linux environment.

The assignment explores how to identify a Linux user and system environment, retrieve operating system and hardware information, and test network connectivity using the `ping` utility.

It provides practical experience with system identification, hardware information, IP connectivity, domain name resolution, and basic network troubleshooting.

The project is documented through screenshots, recorded system information, and network testing observations.

## Problem Statement

Understanding a computer's operating environment and verifying network connectivity are essential foundational skills in IT infrastructure, system administration, and cybersecurity.

This exercise addresses two practical questions:

1. How can a user identify their Linux system, operating environment, and available hardware resources?
2. How can network connectivity be tested using an IP address and a domain name?

The assignment uses Kali Linux command-line tools to investigate these questions and document the results.

## Project Objectives

The main objectives were to:

- Identify the current Linux username and hostname.
- Determine the current working directory.
- Retrieve operating system and hardware information.
- Examine available RAM and disk space.
- Test connectivity to a known IP address.
- Test connectivity to a domain name.
- Observe DNS resolution and differences in network response times.
- Interpret basic ping results, including packet loss and round-trip time.

## Key Features and Activities

### 1. Linux System Identification

Explored basic system information to identify the active user and machine environment.

**Recorded results:**

| Information | Result |
|---|---|
| Username | `kali` |
| Hostname | `kali` |
| Directory | `home/kali` |

This exercise demonstrates familiarity with the Linux environment and basic system navigation.

### 2. Operating System and Hardware Information

Examined the operating system and available system resources.

**Recorded results:**

| System Information | Result |
|---|---|
| Operating environment | Kali Linux |
| Reported version | 6.18.12 |
| Total RAM | 5.5 GiB |
| Available disk space | 4.6 GiB |

These results provide a snapshot of the system environment used during the exercise.

### 3. Network Connectivity Testing Using an IP Address

Performed a connectivity test against the known IP address `8.8.8.8`.

The `ping` utility was used to evaluate network reachability and observe packet transmission responses.

**Recorded results:**

| Metric | Result |
|---|---|
| Target IP address | `8.8.8.8` |
| Average round-trip time | 1004 ms |
| Packet loss | 0% |

The test recorded no packet loss, indicating that all transmitted packets received responses during the observed test.

### 4. Network Connectivity Testing Using a Domain Name

Performed a connectivity test using `google.com` to observe domain name resolution and network response.

**Recorded results:**

| Metric | Result |
|---|---|
| Domain name | `google.com` |
| Resolved IP address | `142.250.139.138` |
| Ping utility | `ping` |
| Packet count option discussed | `-c 4` |

The exercise demonstrated that a domain name can resolve to an IP address, allowing connectivity testing through a hostname rather than entering an IP address directly.

### 5. Understanding Ping Parameters

The assignment also explored the `-c` option used with the Linux `ping` utility.

For example:

- `-c 2` specifies two ping requests.
- `-c 4` specifies four ping requests.

The assignment observed differences between the recorded response times for the IP-address and domain-name tests and considered the different packet counts as a possible explanation.

## Technologies and Tools Used

| Technology / Tool | Purpose |
|---|---|
| Kali Linux | Linux operating environment |
| Linux Terminal | Command-line interaction |
| `ping` | Network connectivity testing |
| IP addressing | Testing connectivity to a known IP address |
| DNS | Domain name resolution |
| System information utilities | Examining system and hardware information |

**Note:** The original assignment does not provide a complete list of the system information commands used. This README therefore does not claim specific additional utilities were executed.

## Project Structure

Suggested GitHub repository organization:

```text
linux-system-network-testing/
│
├── README.md
│
├── Assignment 1.pdf
│
└── screenshots/
    ├── system-identification.png
    ├── system-information.png
    ├── hardware-information.png
    ├── ip-connectivity-test.png
    └── domain-connectivity-test.png
```

The screenshots directory is optional. Add the individual images only if you export them from the original assignment PDF.

## Getting Started

### Prerequisites

To reproduce the exercises, you will need:

- A computer or virtual machine running Kali Linux.
- Access to a Linux terminal.
- An active network connection.
- Basic familiarity with command-line operations.

### Installation

This project does not require a custom application installation or additional software dependencies.

If Kali Linux is already installed, you can proceed directly to the exercises.

For a new environment, obtain Kali Linux from its official website:

https://www.kali.org/get-kali/

Follow the official installation instructions for your chosen environment.

## Usage Instructions

The following steps describe how to reproduce the general activities documented in the assignment.

### Step 1: Identify the Current User

Open the Linux terminal and identify the active username.

```bash
whoami
```

### Step 2: Identify the Hostname

Check the machine's hostname.

```bash
hostname
```

### Step 3: Identify the Current Directory

Display the current working directory.

```bash
pwd
```

### Step 4: Examine System Information

Use Linux system information utilities to inspect the operating system and hardware environment.

For example:

```bash
uname -a
```

```bash
free -h
```

```bash
df -h
```

These are example commands for reproducing the system-information exercise; the original report does not establish that each was used.

### Step 5: Test Connectivity to an IP Address

Use the `ping` utility to test connectivity to a known IP address.

```bash
ping -c 4 8.8.8.8
```

Observe:

- Whether responses are received.
- Packet loss percentage.
- Round-trip time.
- Minimum, average, and maximum response times, where reported.

### Step 6: Test Connectivity to a Domain Name

Test connectivity using a domain name.

```bash
ping -c 4 google.com
```

Observe:

- Whether the domain resolves to an IP address.
- Whether packets receive responses.
- Round-trip time.
- Packet loss.

### Step 7: Compare the Results

Compare the IP-address and domain-name tests.

Consider how DNS resolution, network conditions, destination infrastructure, and the number of transmitted packets may affect the observations.

**Important:** The commands in this section are reproducible examples, not a verified transcript of every command used in the original assignment.

## Skills Demonstrated

This project demonstrates introductory practical skills in:

- Linux system identification.
- Linux command-line navigation.
- Operating system and hardware information gathering.
- RAM and disk-space inspection.
- Basic IP networking.
- Network connectivity testing.
- DNS resolution.
- Understanding ICMP ping responses.
- Interpreting packet loss and round-trip time.
- Technical documentation and screenshot-based reporting.

## Key Learning Outcomes

Through this exercise, I gained practical exposure to:

1. Identifying users, hostnames, and working directories in Linux.
2. Examining operating system and hardware information.
3. Understanding basic network connectivity testing.
4. Using IP addresses and domain names as network test targets.
5. Interpreting packet loss and network response times.
6. Understanding the purpose of the `-c` parameter in the Linux ping utility.
7. Documenting technical findings using screenshots and recorded observations.

These fundamentals provide a foundation for further learning in Linux administration, networking, information security, and cybersecurity.

## Contribution Guidelines

This repository is primarily an educational portfolio project.

Suggestions and contributions that improve the documentation, explanations, or reproducibility of the exercises are welcome.

Potential improvements include:

- Adding additional Linux system identification exercises.
- Improving explanations of network testing results.
- Adding screenshots and command outputs.
- Documenting DNS resolution in greater detail.
- Including additional network troubleshooting exercises.
- Improving the presentation of technical findings.

### Contribution Process

1. Fork the repository.
2. Create a new branch for your changes.
3. Make the proposed documentation or educational improvements.
4. Review the changes for technical accuracy.
5. Submit a pull request describing your contribution.

Please avoid including personal information, passwords, credentials, or sensitive system details in screenshots or documentation.

## Author

**Maureen Uzoewulu**

Areas of interest:
- Linux System Administration
- Networking Fundamentals
- Cybersecurity
- Governance, Risk & Compliance (GRC)
- Information Security and Privacy

Location: Toronto, Canada

## Project Documentation

The original assignment is available in:

`Assignment 1.pdf`

It contains the documented exercises, screenshots, and recorded results.

---

*This project represents practical introductory work in Linux system information gathering and basic network connectivity testing.*
