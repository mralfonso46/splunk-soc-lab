# Lessons Learned

1. Verify log readability and running-process group membership when a Splunk monitor reports that a file is not readable.
2. Keep the SIEM index size appropriate for the available VM storage.
3. Use simple SPL first; add field extraction only when it provides real investigation value.
4. Authentication logs are useful for SSH and sudo detections but do not replace network telemetry.
5. Alerts should be tested with controlled events and then verified through Triggered Alerts and raw evidence.
6. Incident conclusions should distinguish observed evidence from assumptions about intent.
