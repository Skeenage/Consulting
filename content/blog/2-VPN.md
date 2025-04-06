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
***
#### Centrally & automatically deployed via Intune to Entra ID Joined Devices, we have configured a cutting edge VPN configuration that works flawlessly out of the box, using Windows native capabilities and with modern and secure authentication & protocols, ensuring compliance with the highest encryption standards.

As the devices are Entra ID Joined, it was necessary to configure NDES servers for users to automatically receive their user-based certificates through Intune, which also allows certificate enrollment while not connected to the corporate network. The NDES itself is also configured to receive certificates automatically, and the IIS providing the service in addition to the Intune Certificate Connector both use a gMSA for additional security instead of a standard user-based service account. 

Additionally, the SCEP certificate type was chosen over PKCS, providing enhanced flexibility & security as the private key is generated on the client device directly. Entra ID Application Proxy is used to publish the NDES server to Intune devices, acting as a reverse proxy and removing the need to expose inbound ports to the public internet.

The VPN is configured to be 'Always-On', and uses Windows native configuration settings for auto-switching on/off the VPN based on connectivity to the corporate network using a domain profile.

All certificates used for both the backend services & end users are secured with SHA512 encryption, with no exportable keys, and client certificate private keys stored inside the device TPM module.

RADIUS is used to authenticate the user-based certificates, which is also integrated with Azure Certification Authority, allowing conditional access to be applied to each VPN session, based on short-lived certificates issued from Azure.

The IKEv2 VPN can be split or force tunnel, and is configured with maximum strength encryption both on the client device and gateway, allowing only the strongest protocols to be used to initiate a connection.


{{< css.inline >}}
<style>
.canon { background: white; width: 100%; height: auto; }
</style>
{{< /css.inline >}}
