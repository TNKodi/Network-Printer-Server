# Raspberry Pi Printer Network (Virtual Printer)

This README explains how to set up a simple printer network on a Raspberry Pi—even if you don’t have a physical printer—by using CUPS (Common Unix Printing System) and CUPS-PDF (a virtual PDF printer).

---

## Table of Contents

1. [Introduction](#introduction)  
2. [Prerequisites](#prerequisites)  
3. [Step 1: Update & Install CUPS](#step-1-update--install-cups)  
4. [Step 2: Configure CUPS for Network Access](#step-2-configure-cups-for-network-access)  
5. [Step 3: Install & Configure CUPS-PDF](#step-3-install--configure-cups-pdf)  
6. [Step 4: Test the Virtual Printer](#step-4-test-the-virtual-printer)  
7. [Future Steps (Adding a Physical Printer)](#future-steps-adding-a-physical-printer)  
8. [Troubleshooting](#troubleshooting)  
9. [References](#references)  

---

## Introduction

This guide walks you through turning a Raspberry Pi into a networked “printer” by using CUPS and a virtual PDF printer (CUPS-PDF). Any print job sent to this virtual printer will be saved as a PDF instead of being sent to physical hardware. Later, you can replace or supplement the virtual printer with a real one.

---

## Prerequisites

- A Raspberry Pi (any recent model) with Raspberry Pi OS installed.  
- A working network connection (Ethernet or Wi-Fi).  
- SSH or direct terminal access to the Pi (via keyboard + monitor or SSH).  
- A non-root user account (e.g., `pi`) with `sudo` privileges.  
- Basic familiarity with command-line operations.

---

## Step 1: Update & Install CUPS

1. **Update system packages**  
   ```bash
   sudo apt update
   sudo apt upgrade -y

2. **Install Cups
   ```bash
   sudo apt install -y cups

