# TryHackMe - Intro to Offensive Security: Bank Hack Walkthrough

**Date:** 01/11/2025
**Room:** Intro to Offensive Security
**Difficulty:** Beginner
**Platform:** TryHackMe
**Concepts:** Directory Brute-forcing, Web Application Security

## Overview
Completed my first simulated penetration test against a vulnerable bank application. Successfully discovered a hidden bank transfer portal and exploited missing authentication controls to transfer funds between accounts.

## Tools Used
- **Gobuster** - Directory brute-forcing tool
- **Linux Terminal** - Command line interface
- **Web Browser** - Application interaction

## Attack Steps

### 1. Reconnaissance & Enumeration
Used Gobuster to discover hidden directories on the target website:
```bash
gobuster -u http://fakebank.thm -w wordlist.txt dir
