Before we can start, we have to add the repository.
This gives us access to the latest package versions:
`curl -s https://packagecloud.io/install/repositories/crowdsec/crowdsec/script.deb.sh | bash`{{execute T1}}

Great, now we can install the `CrowdSec agent`{{}} it allows you to detect bad behaviors by analyzing log files and other data sources.
:

`apt install crowdsec -y`{{execute T1}}

Once crowdsec is installed we can install the bouncers!

```
apt install crowdsec-firewall-bouncer-iptables crowdsec-nginx-bouncer -y
```{{exec}}