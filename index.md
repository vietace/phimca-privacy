---
layout: default
title: Privacy Policy — PhimCa (Local Media Bridge)
---

**Effective Date:** June 3, 2026

Your privacy is important to us. This Privacy Policy explains how Local Media Bridge ("the App", "PhimCa") collects, uses, and protects your information. The App is designed to prioritize on-device processing and minimize off-device data transmission.

---

## 1. Data Collected and Shared with Third-Party Processors

The App integrates **RevenueCat** to manage in-app purchases (the one-time unlock product). When you launch the App, purchase entitlement state is shared with RevenueCat's backend servers (`api.revenuecat.com`) to verify your purchase status.

**What RevenueCat Collects:**
- **Anonymous App User ID:** An auto-generated UUID. It is **not** linked to your Google account, email address, name, or any personally identifiable information (PII).
- **Purchase History:** Purchased product IDs, entitlement names, and purchase timestamps (required for entitlement gating).
- **Device & App Metrics:** App ID, app version, build number, and SDK version (required for receipt validation).
- **Location Data (Derived):** Your IP address is used at request time to derive your country/region (for region-specific pricing display) and is then immediately discarded. RevenueCat does not retain the IP address.

**What RevenueCat Does NOT Collect:**
- The App does not collect or transmit your name, email address, phone number, or payment method. All payment processing is handled exclusively and securely by Google Play Billing.
- RevenueCat does not have access to your media files, SMB credentials, browsing history, or any other app data.

RevenueCat acts as a third-party data processor. For more details on how they handle data, please refer to the [RevenueCat Privacy Policy](https://www.revenuecat.com/privacy).

---

## 2. On-Device Data (Not Transmitted Off-Device)

The following data is processed and stored strictly locally on your device or transmitted only to destinations you explicitly authorize on your Local Area Network (LAN):

### a. SMB/NAS Credentials
To stream media from your personal network attached storage (NAS), you may provide SMB credentials (username and password). 
- These credentials live **only in memory** during your active connection session and are never saved to disk.
- They are transmitted **only to the LAN server** you specify over your local Wi-Fi network. 
- **Important Security Note:** The App transmits these credentials without app-layer encryption to maintain compatibility with standard consumer NAS devices. If you require wire encryption, please ensure your NAS is configured to enforce SMB signing. The App does not transmit your credentials to us or any third party.

### b. Privacy Mode (`PACKAGE_USAGE_STATS`)
If you enable the "Privacy Mode" feature for screen mirroring, the App requests the `PACKAGE_USAGE_STATS` permission to detect the currently active foreground app. This allows the App to automatically pause the screen mirror if you switch away from the media app (e.g., preventing a banking app or private message from appearing on your TV).
- The identity of the foreground app is analyzed **entirely on your device** and is never collected, logged, or transmitted off-device.

### c. Local Crash Logs
If enabled in Settings, the App may write diagnostic logs or crash reports to your device's local storage (e.g., the `Downloads` folder). 
- These logs are generated for your personal troubleshooting use. 
- They are **never automatically transmitted** to the developer or any third-party analytics service. You maintain full control over whether to email or share these logs using the system's standard share menu.

### d. Media and Browsing Data
- Your local media files, playlists, and cover art remain on your device.
- Any URLs you type or paste into the in-app WebStream browser are processed locally. The App does not track, collect, or transmit your browsing history.

### e. Screen Mirror Audio Capture (`RECORD_AUDIO`)
When you use the optional "Mirror Screen" feature, the App captures **system playback audio** (music, video, and game audio) so it can be streamed alongside the screen video to the DLNA renderer (TV or projector) you choose on your LAN.
- The **microphone is never opened.** Android requires the `RECORD_AUDIO` permission for system-playback capture even though no microphone audio is ever accessed. Capture is filtered to media, game, and unknown audio only — voice calls, voice assistants, notifications, and alarms are excluded by design.
- This audio is **never recorded, stored, or transmitted off-device.** It is streamed only to the DLNA renderer you select on your local Wi-Fi network, and only for the duration of the mirror session.

---

## 3. Data Deletion Rights

Because the App does not require a user account and any data collected by RevenueCat is tied to an anonymous, device-specific UUID, there is no centralized account to delete. 

To exercise your right to delete data:
- **Uninstalling the App** will clear all local data (including bookmarks and settings) and effectively orphan the anonymous purchase record on RevenueCat's servers, permanently disassociating it from your device.
- **Proactive server-side deletion:** If you would like the orphaned RevenueCat record proactively deleted from their servers, email us at epicmediadev@gmail.com with your request. We will forward your anonymous App User ID to RevenueCat's deletion endpoint on your behalf.

If you are located in the EU/EEA or the UK, you may exercise your rights under the GDPR — including access, deletion, portability, and the right to object — using the contact email above. We will respond within the timeframes required by applicable law.

---

## 4. Children's Privacy

This App is not directed at children under 13 (or the minimum age of digital consent in your jurisdiction). We do not knowingly collect personal information from children. If you believe a child has provided information through the App, please contact us at the email below and we will take steps to address it.

## 5. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in our practices or for other operational, legal, or regulatory reasons. The updated version will be indicated by an updated "Effective Date."

## 6. Contact Us

If you have any questions or concerns about this Privacy Policy or our data practices, please contact us at:

**Email:** epicmediadev@gmail.com
