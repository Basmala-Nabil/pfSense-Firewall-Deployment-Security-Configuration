# Securing a Network Perimeter with pfSense & pfBlockerNG

## Overview

This project demonstrates the deployment and configuration of a secure network perimeter using **pfSense** and **pfBlockerNG** in a virtual lab environment. The objective was to implement firewall security controls, enhance network protection through threat intelligence, and validate that all security policies were properly enforced using firewall logs and monitoring tools.

## Objectives

* Deploy and configure a pfSense firewall.
* Create WAN/LAN network segmentation.
* Install and configure pfBlockerNG.
* Implement GeoIP-based traffic filtering.
* Configure DNSBL to block access to specified domains.
* Restrict administrative access to the pfSense WebGUI.
* Monitor firewall logs and pfBlockerNG reports to verify rule enforcement.

## Lab Environment

* VMware Workstation
* pfSense Community Edition
* pfBlockerNG
* Windows 11 Client
* Kali Linux (Testing)
* Virtual Networks (WAN & LAN)

## Implementation

### 1. pfSense Deployment

* Installed pfSense as a virtual machine.
* Configured separate WAN and LAN interfaces.
* Assigned IP addresses and verified network connectivity.
* Enabled DHCP service on the LAN interface.

### 2. pfBlockerNG Configuration

* Installed pfBlockerNG from the Package Manager.
* Configured IP reputation and threat intelligence feeds.
* Updated feeds and verified successful synchronization.

### 3. GeoIP Blocking

* Configured GeoIP filtering to block traffic from selected high-risk countries.
* Applied firewall rules using pfBlockerNG.
* Verified that blocked traffic was denied as expected.

### 4. DNSBL Configuration

* Enabled DNSBL.
* Added custom domains to the block list.
* Confirmed that requests to blocked websites were redirected and denied.

### 5. Firewall Hardening

* Restricted WebGUI access to authorized hosts only.
* Applied firewall rules to prevent unauthorized administrative access.
* Verified management access restrictions.

### 6. Monitoring and Validation

* Monitored firewall logs to confirm blocked connections.
* Reviewed pfBlockerNG reports to validate IP and DNS filtering.
* Confirmed that all implemented security controls generated the expected logs and alerts.

## Key Skills Gained

* Firewall Administration
* Network Segmentation
* pfSense Configuration
* pfBlockerNG Management
* GeoIP Filtering
* DNS-Based Blocking (DNSBL)
* Firewall Rule Management
* Security Monitoring
* Log Analysis
* Network Hardening

## Conclusion

This project provided hands-on experience in deploying and securing a network perimeter using pfSense. Beyond configuring firewall rules, the project emphasized validating security controls through monitoring and log analysis, reinforcing the importance of verification in real-world network security and Blue Team operations.
