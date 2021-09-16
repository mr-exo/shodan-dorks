# Top 100 Interesting Shodan Dorks

_This is the list of most interesting shodan dorks that you can use on Shodan.io_
</br>

# Cameras and Webcams

webcamXP/webcam7: \
`("webcam 7" OR "webcamXP") http.component:"mootools" -401`

Some Webcams(SQ Webcams?): \
`Server: SQ-WEBCAM`

Yawcam Webcams: \
`"Server: yawcam" "Mime-Type: text/html"`

Surveillance Cams: \
`Server: uc-httpd 1.0.0`\
`NETSurveillance uc-httpd`\
***Surveillance cams with admin:admin or admin:(none) creds***

Hikvision Cameras: \
`product:"Hikvision IP Camera"` \
***Link for Hikvision backdoor here:*** https://ipvm.com/reports/hik-exploit

Generic dork for finding cameras: \
`title:camera`

Generic dork for finding cameras (with screenshots): \
`webcam has_screenshot:true`

Dahua Cameras: \
`http.title:"WEB VIEW"`

Some random webcams: \
`http.title:"Webcam"`

</br>

# Vulnerable Services / Servers

EternalBlue SMB RCE: \
`os:"Windows 10 Home 19041`
***please dont use this much :d***

ProFTPD 1.3.5 (mod_copy exec; CVE-2015-3306) : \
`"220 ProFTPD 1.3.5"`

Anonymous FTP Login #1: \
`"230 User anonymous"`

Anonymous FTP Login #2: \
`"220" "230 Login successful." port:21`

Already Logged-In as root via Telnet: \
`"root@" port:23 -login -password -name -Session`

No password for Telnet Access: \
`port:23 console gateway`

</br>

# Other Services that you can find

OpenSSH: \
`openssh port:22`

Logitech Media Servers: \
`"Server: Logitech Media Server" "200 OK"`

Jenkins Unrestricted Dashboard: \
`x-jenkins 200`

MySQL: \
`"product:MySQL"`

MongoDB #1: \
`mongodb port:27017`

MongoDB #2: \
`product:"MongoDB"`

</br>

# Interesting Things that you can find on Shodan

RDP/VNC's WITHOUT AUTH: \
`"authentication disabled" "RFB 003.008"`\
`remote desktop "port:3389"`

XZERES Wind Turbines: \
`title:"xzeres wind"`

MikroTik Routers: \
`port:8291 os:"MikroTik RouterOS 6.45.9"`

Minecraft Servers: \
`"Minecraft Server" "protocol 340" port:25565`
***There are too many minecraft servers lol***

Smart TVs: \
"Chromecast:" port:8008

Maritime Satellites: \
`"Cobham SATCOM" OR ("Sailor" "VSAT")`
***Real-time location of ships via satelite***

Tesla PowerPack Charging Status Page: \
`http.title:"Tesla PowerPack System" http.component:"d3"`

Samsung Electronic Billboards: \
`"Server: Prismview Player"`

# Info:
***Stuff that i've posted here are for educational purposes only.***\
***Some dorks i found on different gits and different websites, so they ain't mine (most of em)***\
***Send me better Shodan.io dorks that i can post on here to my discord at: exo?#0001***
