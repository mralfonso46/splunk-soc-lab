# Data Ingestion

## Authentication Logs
- Path: `/var/log/auth.log`
- Sourcetype: `linux_secure`
- Index: `soc_lab`
- Continuous file monitoring: enabled

## Port Scan Telemetry
- Path: `/var/log/portscan.log`
- Sourcetype: `portscan_test`
- Index: `soc_lab`
- Captured on `ens38` with tcpdump using a TCP SYN filter.

The network telemetry source was added because the existing authentication log source did not provide reliable evidence of Nmap port scanning.
