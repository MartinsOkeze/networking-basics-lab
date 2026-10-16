# Networking Basics Lab

## Project Overview

This project demonstrates beginner-level networking concepts and practical troubleshooting methods relevant to entry-level IT Support and Help Desk roles.

The lab covers IP addresses, default gateways, DNS, internet connectivity checks, and common Windows networking commands.

## 1. Understanding IP Addresses

An IP address identifies a device on a network and allows devices to communicate.

**Example:** `192.168.1.25`

**What I learned:**
- Devices connected to a network may receive IP addresses automatically from a router.
- An incorrect or missing IP configuration can prevent network access.
- The `ipconfig` command displays Windows IP configuration details.

**Practice command:**

```cmd
ipconfig
```

## 2. Understanding the Default Gateway

A default gateway is usually the router that allows a device to communicate with networks outside its local network.

**Troubleshooting steps:**
1. Open Command Prompt.
2. Run `ipconfig`.
3. Locate the Default Gateway entry.
4. If a gateway is listed, test connectivity to it using `ping`, where permitted.

**Example command:**

```cmd
ping 192.168.1.1
```

Replace the example address with the actual gateway shown on your computer.

## 3. Understanding DNS

DNS (Domain Name System) translates domain names, such as `example.com`, into IP addresses that computers use to communicate.

**Common symptom:** A user cannot access websites by name.

**Practice command:**

```cmd
nslookup example.com
```

**What to check:**
- Whether DNS returns an answer.
- Whether the displayed DNS server responds.
- Whether the issue affects one website or multiple websites.

A failed lookup can indicate a DNS issue, but further checks are needed before confirming the cause.

## 4. Testing Network Connectivity

The `ping` command tests whether a destination responds to network requests.

**Example command:**

```cmd
ping example.com
```

**How to interpret the result:**
- Replies indicate that the destination responded to the ping.
- Request timeouts mean no reply was received within the allowed time.
- Some devices and websites block ping requests, so a timeout does not automatically mean the internet is down.

## 5. Troubleshooting: Unable to Access the Internet

**Simulated scenario:** A user reports that their computer cannot access websites.

**Troubleshooting process:**
1. Check whether Wi-Fi or Ethernet is connected.
2. Determine whether other devices have internet access.
3. Run `ipconfig` to inspect the IP address and default gateway.
4. Use `ping` to test connectivity where appropriate.
5. Use `nslookup example.com` to investigate DNS resolution.
6. Record findings and escalate if administrator access or further investigation is needed.

**Verification:** Retry the affected website or application after any corrective action and confirm whether access has returned.

## 6. Useful Windows Networking Commands

| Command | Purpose |
|---|---|
| `ipconfig` | Displays IP configuration |
| `ipconfig /all` | Displays detailed network configuration |
| `ping example.com` | Tests whether a destination responds |
| `nslookup example.com` | Checks DNS name resolution |
| `tracert example.com` | Shows the route toward a destination |

These commands are for learning and troubleshooting. Results depend on network settings, permissions, and the destination being tested.

## Skills Practised

- Basic networking concepts
- IP address and gateway identification
- DNS troubleshooting fundamentals
- Windows Command Prompt
- Network connectivity testing
- Structured troubleshooting and documentation
- Technical communication and escalation

## Learning Note

This repository documents learning exercises and example commands. Results should be recorded from actual practice when performed. No simulated scenario should be presented as verified workplace experience.
