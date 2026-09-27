# Splunk Installation

- Platform: Ubuntu Server 24.04
- Splunk Enterprise: 10.4.3
- Package: Linux AMD64 `.deb`
- Web interface: `10.10.10.1:8000`

Splunk was configured to run under the `splunk` account. The `splunk` user was added to the `adm` group so it could read `/var/log/auth.log`. Splunk was restarted after the group change so the running `splunkd` process inherited the group membership.
