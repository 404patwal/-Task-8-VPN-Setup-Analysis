# Internship Task 8 — VPN Setup & Analysis

**Analyst:** Avinash Patwal  
**Date:** 2025-09-26  
**Tool used:** ProtonVPN (Free)  — Windows 10

## 1. Objective
Set up a VPN client, connect to a VPN server, verify IP & DNS change, compare speed, and document benefits & limitations.

## 2. Steps performed
1. Created ProtonVPN free account and installed ProtonVPN Windows client.  
2. Captured baseline public IP and DNS (before connecting).  
   - `screenshots/ip_before.png`  
   - `screenshots/dnsleak_before.png`  
   - Speed baseline: `screenshots/speed_before.png` (Download: X Mbps, Upload: Y Mbps)
3. Connected to ProtonVPN server: **[server name / country]**.  
   - Screenshot: `screenshots/vpn_connected.png`
4. Verified new public IP and DNS while connected:
   - `screenshots/ip_after.png` (IP after: [IP_AFTER])  
   - `screenshots/dnsleak_after.png`
5. Ran speed test while connected: `screenshots/speed_after.png` (Download: A Mbps, Upload: B Mbps)  
6. Disconnected VPN: `screenshots/vpn_disconnected.png`
7. Compared results and documented findings.

## 3. Observations / Results
- **IP before:** [IP_BEFORE] (see `ip_before.png`)  
- **IP after (VPN):** [IP_AFTER] (see `ip_after.png`)  
- **DNS before:** [DNS_BEFORE] (see `dnsleak_before.png`)  
- **DNS after:** [DNS_AFTER] (see `dnsleak_after.png`)  
- **Speed before:** Download = [X] Mbps, Upload = [Y] Mbps (see `speed_before.png`)  
- **Speed while VPN:** Download = [A] Mbps, Upload = [B] Mbps (see `speed_after.png`)  
- **Interpretation:** IP changed correctly → traffic is routed via VPN server. Speed decreased by ~[percent]%, which is expected.

## 4. VPN Benefits (summary)
- Encrypts traffic on insecure networks (public Wi-Fi).  
- Masks public IP and approximate location.  
- Allows accessing geo-restricted content (if provider allows).  
- Adds privacy layer from local ISP / network snoopers.

## 5. VPN Limitations & Risks
- Provider can see your traffic — trust their logging policy.  
- Free tiers often limit speed and server locations.  
- Some websites block VPN IPs.  
- Encryption doesn’t protect from site-level tracking (cookies, accounts).

## 6. Tools & Links used
- `https://protonvpn.com` — client used.  
- `https://whatismyipaddress.com` / `https://ipinfo.io` — public IP checks.  
- `https://dnsleaktest.com` — DNS leak test.  
- `https://www.speedtest.net` — speed comparison.

## 7. Conclusion & recommendation
VPN was successfully set up and verified (IP changed, DNS routed). Use VPN on public Wi-Fi and prefer paid reputable providers for stronger privacy guarantees. Always check provider’s privacy policy and enable kill switch feature for safety.

## 8. Files submitted
- `report.md`  
- `screenshots/` (ip_before.png, dnsleak_before.png, speed_before.png, vpn_connected.png, ip_after.png, dnsleak_after.png, speed_after.png, vpn_disconnected.png)
