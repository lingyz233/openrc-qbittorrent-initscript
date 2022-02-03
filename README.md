### Dependencies
- Openrc
- qBittorrent (Required USE flags: webui)

### Installation
`cp ./qbittorrent /etc/init.d/qbittorrent`  
`chmod +x /etc/init.d/qbittorrent`

### Usage
- Start: `rc-service qbittorrent start`  
- Stop: `rc-service qbittorrent stop`  
- Run on startup: `rc-update add qbittorrent default`

### Note
[=Running `rc-service qbittorrent restart` will not work because qBittorrent does not=]
[=stop immediately and will refuse to start if it detects that it is already running. =]
In this version, it seems that `rc-service qbittorrent restart` works without any errors.
