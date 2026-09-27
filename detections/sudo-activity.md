# Detection — Repeated Sudo Activity

**SPL**
```spl
index=soc_lab "sudo:" earliest=-5m
| stats count by host
| where count >= 5
```

The controlled test produced 15 matching events on `ubuntu-server`.
