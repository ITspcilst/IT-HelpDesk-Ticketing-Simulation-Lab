# Ticket 001 – Network Connectivity Issue

## Incident Summary
User reported inability to access the internet and internal resources. LAN cable connected and link light active.

## User Impact
User unable to perform work tasks requiring network access.

## Environment
Windows 10 workstation connected to corporate LAN using DHCP.

## Troubleshooting Performed
- Verified physical network connection
- Checked IP configuration using `ipconfig`
- Confirmed device obtained valid DHCP lease
- Pinged default gateway – successful
- Pinged external IP (8.8.8.8) – successful
- Tested DNS resolution – failed
- Flushed DNS cache (`ipconfig /flushdns`)
- Renewed DHCP lease (`ipconfig /renew`)

## Findings
Network connectivity functioning locally but DNS resolution failing.

## Root Cause
Suspected DNS server issue.

## Resolution / Action Taken
Escalated to Tier 2 Network Team for DNS infrastructure investigation.

## Screenshot Evidence
![Network Ticket](/screenshots/Network_Connectivity_Issue.png)
