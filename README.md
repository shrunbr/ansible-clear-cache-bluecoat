# ansible-clear-cache-bluecoat
Using Ansible to clear the DNS cache on a Bluecoat Proxy.

**Prerequisites**

 - Ansible 2.7+
 - Bluecoat Proxy

**File Customization**
You will need to customize all files to use this playbook.

 - YML File
	- Enter in the proxies enable password where it says "PROXYPASS" under the "enable on proxy" section.
- ansible.cfg
	- You will need to set your logging destination here for the playbooks log file.
- proxy_inventory.txt
	- You will need to put in your proxies IP where it says "10.PROXY.IP.HERE". You will also need to put your login password where it says "PASSWORD" and your enable password where it says "ENABLEPASS"

**Additional Information** 
The logging destination I specifically use because I have this playbook run on cron job every 24 hours.

