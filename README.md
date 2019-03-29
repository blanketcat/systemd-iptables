# iptables/ip6tables systemd configuration

Example of a persistent firewall based on systemd for Debian Jessie.

### Install Steps
```sh
cp -r etc/iptables /etc/iptables
cp -r etc/systemd/system/iptables.service /etc/systemd/system/
cp -r etc/systemd/system/ip6tables.service /etc/systemd/system/

systemctl daemon-reload

systemctl enable iptables.service
systemctl enable ip6tables.service

systemctl start iptables.service
systemctl start ip6tables.service
```

### Repo is deprecated.
Evidently you cannot change a public fork of a repo to a private one. Don't add rules here. Actual development has moved to the private repo.
