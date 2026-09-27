# Detection — Failed SSH Authentication

**SPL**
```spl
index=soc_lab sourcetype=linux_secure ("Failed password" OR "Invalid user")
| stats count by host
| where count >= 5
```

**Alert:** `SOC - SSH Failed Authentication Threshold`  
**Schedule:** Every 5 minutes  
**Window:** Last 5 minutes  
**Trigger:** Number of results > 0  
**Severity:** Medium
