# Detection — Possible Port Scan

**SPL**
```spl
index=soc_lab sourcetype=portscan_test "10.10.10.2"
| stats count
| where count >= 20
```

**Alert:** `SOC - Possible Port Scan`  
**Schedule:** Every 5 minutes  
**Window:** Last 5 minutes  
**Trigger:** Number of results > 0  
**Severity:** Medium
