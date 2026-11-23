# Privacy Policy for Whoish

*Last updated: November 22, 2026*

## Overview

Whoish is a domain, DNS, and network analysis app for macOS and iPadOS. This policy explains what data the app handles and where it goes.

## Data Collection

Whoish does **not** collect personal data. There is no account, no analytics, no advertising, no tracking cookies, and no third-party tracking SDK. Nothing you look up is sent to the developer.

## Network Connections

To answer a lookup, the app connects directly from your device to:

* **Your chosen DNS resolver** (Cloudflare, Google, Quad9, or OpenDNS) over DNS-over-HTTPS, to read DNS records
* **Team Cymru** (`asn.cymru.com`), through that same resolver, to learn which network an IP address belongs to. The query contains only the IP address.
* **WHOIS servers** (for example `whois.verisign-grs.com` or `whois.iana.org`) over TCP port 43, for registration data
* **rdap.org**, for domain registration data and IP ownership
* **The domain you look up** (its public web servers), to read its SSL/TLS certificate and HTTP headers
* **Certificate Transparency services** (`crt.sh`, with `api.certspotter.com` as a fallback), to find subdomains
* **Apple**, to verify purchases and subscription status with StoreKit, and to check whether a newer version of Whoish is available in the App Store. The update check sends only the app's bundle identifier.

These connections happen when you run a lookup, when monitoring checks a favorite you turned on, and when the app checks for updates. They do not include your name, email, Apple ID, or any device identifier. Each service receives the domain or address it needs to answer, and handles it under its own privacy policy.

## Data Stored on Your Device

Everything Whoish saves stays on your device:

* **Search history and favorites**, stored with SwiftData
* **Monitoring snapshots and alerts**, stored with SwiftData
* **Settings** such as appearance, DNS resolver, and content size, stored in UserDefaults

You can delete history and favorites in the app at any time. Deleting the app removes all of it.

## Monitoring and Notifications

If you turn on monitoring for a favorite, Whoish checks it at the interval you choose. On a Mac this happens while Whoish is running. On an iPad it happens while Whoish is the app on screen. When something changes, the app shows a **local notification** created on your device. Whoish uses no push service, and no notification token or list of domains leaves your device.

## Reports

PDF and text reports are created in your device's memory. They are saved or shared only where you choose, through the system save dialog or share sheet. Whoish does not upload them anywhere.

## Purchases

Purchases and subscriptions are handled by Apple through the App Store. Whoish never sees your payment details.

## Children's Privacy

Whoish does not collect personal data from anyone, including children under 13.

## Changes to This Policy

If this policy changes, the new version will be posted on this page with a new date.

## Contact

Questions about this policy: tony@mailish.se
