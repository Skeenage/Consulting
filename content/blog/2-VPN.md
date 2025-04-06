+++
author = "Oliver DeVito"
title = "Windows Native IKEv2 Always-On VPN Deployment"
date = "2024-01-01"
description = "Certificate authentication & Entra ID Conditional Access"
summary = "Certificate authentication & Entra ID Conditional Access"
image = "/img/projects/vpn.avif"
draft = false
tags = [
    "markdown",
    "text",
]
+++

Centrally & automatically deployed via Intune to Entra ID Joined Devices, we have configured a cutting edge VPN configuration that works flawlessly out of the box, using Windows native capabilities and with modern and secure authentication & protocols, ensuring compliance with the highest encryption standards.

As the devices are Entra ID Joined, it was necessary to configure NDES servers for users to automatically receive their user-based certificates while not connected to the corporate network. The NDES itself is also configured to receive certificates automaically, and uses a gMSA for additional security instead of a standard user-based service account. 

*the Intune Certificate Connecor also uses the gMSA

Additionally, the SCEP certificate type was chosen over PKCS, providing enhanced flexibility & security as the private key is generated on the client device directly. Entra ID Application Proxy is used to publish the NDES server to Intune devices, acting as a reverse proxy and 

The VPN is configured to be 'Always-On', and uses Windows native configuration settings for auto-switching on/off the VPN based on connetivity to the corporate network using a domain profile.

NDES gMSA
app proxy
certificates secured, no exportable keys and SHA 512

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

{{< css.inline >}}
<style>
.canon { background: white; width: 100%; height: auto; }
</style>
{{< /css.inline >}}
