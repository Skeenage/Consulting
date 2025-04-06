+++
author = "Oliver DeVito"
title = "Intune Migration"
date = "2025-01-01"
description = "Full end to end secure deployment in 6 months"
summary = "Full end to end secure deployment in 6 months"
image = "/img/projects/intune.jpg"
draft = false
tags = [
    "markdown",
    "text",
]
+++
***
We have successfully completed an Intune migration project in under 6 months, including the integration of;

### 1. Windows Native IKEv2 Always-On VPN, secured with;
* User-based SCEP Certificates integrated with Active Directory Certification Authority
  *  Deployed with NDES & Azure Application Proxy
* LDAP & RADIUS authentication
* Conditional Access Policy based on device compliance

### 2. Full centralised Defender deployment with 96% device security score & 3% vulnerability score;
* Firewall configuration
* SmartScreen configuration
* Antivirus configuration
* Attack Surface Reduction Rules
* Automated Investigation & Response
* Device risk score integration

### 3. Fully automated Autopilot deployment process from OEM ISO;
* Without reboot & keeps the same authentication token to provision Windows Hello for Business;
  *  A user never needs to know their password
* Clean, structured & minimalist device-based group management
* Automatic deployment of several languages & keyboard layouts
* Removes OEM pre-installed applications
* Deploys device & user certificates for Wifi & VPN authentication
* Automatically provisions organisation-managed TeamViewer with different deployment scenarios
* Everything is configured automatically from the beginning - when the user reaches the desktop;
  *  Several applications have been installed & configured
  *  Wifi is configured and auto-switches
  *  Printers & on-premises network drive mappings configured
  *  User is silently enrolled to OneDrive
  *  The device is silently encrypted with BitLocker
  *  Migration begins from AD user home profile to OneDrive
  *  Browser & Outlook are configured
  *  Default desktop & lock screen wallpapers deployed
  *  Default taskbar configured

### 4. Deployment rings configured for Windows, BIOS & application updates, configuration changes .etc;
* Preview Ring
* Limited Ring
* Broad Ring
* Critical Ring

### 5. Fully Entra ID Joined devices with;
* Centrally managed Local Administrator Password Solution, with each device having a unique local administrator password rotating on a frequent basis
* Device Compliance policies fully enabled including risk-based protection
* Cloud Kerberos single sign on to on-premises with Windows Hello for Business
* Azure File shares integrated with Entra ID Kerberos for single sign on and Azure Identity Access Control, automatically mapped as network drives.
* Domain network location profile configured

### 6. Centralised BIOS policies deployed with;
* Certificate authentication & QR code BIOS login
* Configuration settings
* Automatic updates

### 7. Fully automated centralised application updates;
* Based on a standalone deployment of WinGet
* Possibility to prevent the upgrade of specific applications

### 8. Clean, organised & centrally managed Security Baselines, configured into logical categories and subcategories including;
* Office 365 with Trusted Locations
* Audit logging
* Account & Authentication policies
* Silent BitLocker enrollment
* Local Device, Group, and User policies
* Microsoft Edge configuration with;
  *  Exception configuration
  *  Enterprise Mode Site List
  *  Zone configuration

### 9. Device Restrictions & exceptions including;
* Microsoft App Store
* Browser installation restricted with AppLocker, allowing only Microsoft Edge

### 10. Fully automated, silent, & parameterised application & script deployments & configuration from the Company Portal including;
* Centrally managed Intune management files, allowing organisation of directories on the local device, registry locations & scheduled tasks
* Code Signing certificates
* Grant Local Administrator permissions for Admins temporarily
* SAP GUI
* Specific Drivers
* Jabra Xpress
* Office 365
* Visio
* Project
* Custom Line of Business applications
* RSAT Tools
* Customised Windows experience
* Greenshot
* Remote Desktop Manager with Single Sign On

### 11. Centrally managed Remote Desktop configured allowing IT access to all devices


{{< css.inline >}}
<style>
.canon { background: white; width: 100%; height: auto; }
</style>
{{< /css.inline >}}
