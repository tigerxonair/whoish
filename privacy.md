# Privacy Policy for Whoish

*Last updated: September 17, 2026*

## Overview

Whoish is a domain, DNS, and network analysis tool for macOS and iPadOS. Your privacy is fundamental to our design. This policy explains what data the app handles and how.

## Data Collection

Whoish does **not** collect, track, transmit, or store any personal data on external servers. There are no analytics frameworks, tracking cookies, advertising networks, or third-party tracking SDKs.

## Network Connections

To perform domain lookups and analysis, the app initiates direct outgoing network connections to:
* **DNS resolvers** (Cloudflare, Google, Quad9, or OpenDNS) to resolve DNS records securely via DNS-over-HTTPS
* **WHOIS servers** (e.g., whois.verisign-grs.com) to retrieve domain registration and expiration data via TCP port 43
* **Target domains** (their public web servers) to inspect SSL/TLS certificates and HTTP security headers
* **rdap.org** to query IP address allocation and network ownership data
* **Certificate Transparency Log aggregators** (`crt.sh`) via HTTPS to discover publicly registered subdomains and certificates for the queried domain
* **Apple App Store** for in-app purchase verification and subscription status via StoreKit

These connections are initiated only when you perform a lookup, when you export a report, or during automatic favorite checks that you have enabled. No personal information or user identity is included in these requests.

## Local Storage & Background Monitoring

The app stores all data locally on your device:
* **Search history and favorites** (stored via SwiftData, strictly on-device)
* **Favorites monitoring snapshots and alerts** (stored locally via SwiftData)
* **User preferences** such as appearance, DNS resolver choice, and content scale (stored in UserDefaults)

If you enable **Favorites Monitoring**, the app periodically checks your monitored domains and schedules **local on-device notifications** when changes occur. No push notification tokens, device identifiers, or domain lists are ever transmitted to any external server.

## Report Generation & Export

PDF and text reports are generated on the fly directly in your device’s memory (RAM). Reports are only saved to locations that you explicitly choose through the system save dialog or share sheet. Whoish does not upload or transmit your generated reports to external cloud storage.

## In-App Purchases

Purchases and subscriptions are processed entirely by Apple’s StoreKit framework. Whoish does not collect, process, or store payment details or billing information.

## Children’s Privacy

Whoish does not knowingly collect personal data from children under 13. The app does not collect personal data from any user.

## Changes to This Policy

If this policy is updated, changes will be posted on this page with an updated date.

## Contact

If you have questions about this privacy policy, contact: tony@mailish.se
