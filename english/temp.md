# self-hosting-tamil-book
Book about self hosting in tamil language

----

Draft

----

#+title: Easy way to self hosting
#+author: Thanga Ayyanar

# Introduction
## What is Hosting ?
## What is Self Hosting ?
## Minimalist self hosting, why?
## Is this the only way to do it.

# Chapter 1: Preparing the device
## Choosing the distro
### Debian/Ubuntu
- CasaOS
### Proxmox
## Installing essentials
### SSH
## Things to note in android
### SSH
## Security
### Firewall
### Fail2Ban

# Chapter 2: Docker/Podman
## Do you need docker for selfhosting
## Portainer
## Watch tower (Container)
- Keeping your containers uptodate

# Chapter 3: Media server
## What is media server?
## miniDNLA
## Jellyfin
## Samba (You can use samba to share media)

# Chapter 4: Sharing folders
## Samba
## NFS

# Chapter 5: Syncing folders between devices
## Rsync
## Syncthing
- To expose in local network
- `$HOME/.local/state/syncthing` then find port 8384
- Change 127.0.0.1:8384 to :8384 (colon is important)
- ref:
  - https://forum.syncthing.net/t/solved-changing-listening-port/69/5
  - https://docs.syncthing.net/users/config.html

# Chapter 6: Image gallery
## Static image gallery generator
## Dynamic image gallery generator
## Immich, photoprism

# Chapter 7: Documents & Notes
## Next cloud
- Your knowledge base
- Medical documents
- Scanned documents

# Chapter 8: Finance
## Ledger/hledger/beancount
## paisa
## FireflyIII

# Chapter 9: Task management
## Next cloud
## Task warrior
## Org mode - GTD (for Emacs users)

# Chapter 10: Downloader
## Aria2
- Integration with yt-dlp or youtube-dl
## Transmission

# Chapter 11: Version control
## Git bare
## Charmcli - ssh git
## Cgit
## Forgejo or Gitea

# Chapter 12: Monitoring services
## Uptime kuma
## Netdata
## staus-ng
## Glances - system monitor (python) 
- https://nicolargo.github.io/glances/

# Chapter 13: Notification service
## Ntfy
## Gotify

# Chapter 14: DNS and Ad-Blocking
## Dnsmasq
- https://www.imaginaryrobots.net/posts/2022-01-26-full-network-adblocking-with-dnsmasq/
## Pihole
## Adguard
## blocky
## Gravity
https://github.com/BeryJu/gravity

# Chapter 15: RSS Reader
## Tiny tiny rss
- Also support integrating with newsboat
## Miniflux (go based)

# Chapter 16: Library
## Calibre

# Chapter 17: Password manager
## Password store
## vaultwarden

# Chapter 18: Encryption
## Veracrypt
## GPG2

# Chapter v: Dashboard
## Cooking our own
## Homer or other

# Chapter w: Backup
## Refer chapter 5
## Use docker or ansible

# Chapter x: Reverse proxy
## Ngnix reverse proxy
## Caddy
## Haproxy

# Chapter y: Exposing to the internet
## DDNS
## Tailscale
## Cloudflare tunnels
## Private VPS

# Chapter z: Misc
- Tools or software which are niche
## Hosting static pages
### Light httpd
### caddy
- You can also try our apache2 or ngnix
## Automation
- Rabbit hole of its own
- software based
- IOT based
## Ansible
## Tracking progress
- Activity watch
- arbtt (haskell)
- Timetracker (Rust)
  - https://github.com/phiresky/timetrackrs
## Laminar - CI/CD
## IRC bouncer
## Quiz app
## Wake on lan
- ref
  - https://www.cyberciti.biz/tips/linux-send-wake-on-lan-wol-magic-packets.html

# Troubleshooting & Tricks
## Auto start programs in ubuntu
- https://askubuntu.com/questions/48321/how-do-i-start-applications-automatically-on-login#48327
## Check if service is running 
    - lsof -i :port -S
    - netstat -a | grep port
## Shutdown over ssh
- sudo poweroff

# Bonus
## PARA
## JBOD
- Hard disk
  
# Finishing thoughts
- Hope this will kick start your journey in self-hosting.
- The dream self hosting setup differs for person to person.

# Reference
- https://landchad.net/
- Reddit - Selfhost, homelab

# Drafts
## Creating bridge for hypervisor / Virtual machine
