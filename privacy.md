# Privacy Policy for Whoish

_Last updated: February 28, 2026_

## Overview

Whoish is a domain and network analysis tool for macOS. Your privacy is important to us. This policy explains what data the app handles and how.

## Data Collection

Whoish does **not** collect, transmit, or store any personal data on external servers. There are no analytics, tracking, advertising, or third-party SDKs.

## Network Connections

To perform domain lookups, the app makes outgoing network connections to:

- **DNS resolvers** (Cloudflare, Google, Quad9, or OpenDNS) to resolve DNS records via DNS-over-HTTPS
- **WHOIS servers** (e.g., whois.verisign-grs.com) to retrieve domain registration data via TCP port 43
- **Target domains** to inspect SSL certificates and HTTP headers
- **rdap.org** to look up IP address ownership information
- **Apple App Store** for in-app purchase verification via StoreKit

These connections are initiated only when you perform a lookup. No personal information is included in these requests.

## Local Storage

The app stores the following data locally on your Mac:

- **Search history** and **favorites** (stored via SwiftData, on-device only)
- **User preferences** such as appearance, DNS resolver choice, and content scale (stored in UserDefaults)

This data never leaves your device and can be deleted at any time from within the app.

## In-App Purchases

Purchases are handled entirely by Apple's StoreKit framework. Whoish does not process or store any payment information.

## Children's Privacy

Whoish does not knowingly collect data from children under 13. The app does not collect data from anyone.

## Changes to This Policy

If this policy is updated, the changes will be posted on this page with an updated date.

## Contact

If you have questions about this privacy policy, contact: tony@mailish.se
