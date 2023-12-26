# Docker and Self-Hosting Setup Guides

A pillar for self-hosting pourposes and anyone starting their journey with Docker, a companion for:

* My RPi guide: <https://jalcocert.github.io/RPi/#Prerequisites>
* My Linux guide: <https://github.com/JAlcocerT/Linux>
* The [self-hosting](https://fossengineer.com/tags/self-hosting/) and [docker](https://fossengineer.com/tags/docker/) entries in my blog <https://fossengineer.com/>.
  * [Install Portainer and get ready to deploy docker containers with a UI.](https://fossengineer.com/selfhosting-portainer-docker/)

## Repository Structure:
  * [Introduction: Why Docker?](#Intro)
  * [Back-up related containers](#Backups)
  * [Business apps related containers](#business)
  * [Communication apps related containers](#communication)
  * [IoT Containers](#iot)
  * [Media Containers](#media)
  * [Security and Privacy related Containers](#security)
  * [Web related Containers](#Web)
  * [Ways to Contribute](#contribute)

## Why Docker?

[Docker is a tool](https://fossengineer.com/docker-first-steps-guide-for-data-analytics/) designed to make it easier to **create, deploy, and run applications by using *containers*.**

Containers allow us to **package up an application with all of the parts it needs to work properly** -  such as libraries and other dependencies, and deploy it as one package.
By doing this, the application will run on any other Linux machine (also windows or ios) regardless of any customized settings that machine might have that could differ from the machine used for writing and testing the code.

Containers remain lightweight by sharing the OS they run on while isolating processes within user space.
 
Everything needed to run a software application successfully can be stored in a container to make development and deployment more efficient. For this reason, containers are perfect for running microservices.

## Docker and your favourite Apps

I have been collecting the config files to install with Docker several Apps and consolidated it on this repository for anyone that might find it helpful.

<details>
  <summary>Click to know which Apps</summary>
  &nbsp;

### [Backups:](https://github.com/JAlcocerT/Docker/tree/main/Backups)
  * Duplicati :heavy_check_mark:
  * Duplicity
  * Urbackup
  * Filerun :heavy_check_mark:
  * Nextcloud
    * [RPI](https://jalcocert.github.io/RPi/posts/selfhosting-nextcloud/) :heavy_check_mark:
    * Recommended apps: cospend (moneybuster android)
  * Photos: 
    * LibrePhotos
    * Lychee 
    * Photonix
    * Photoprism
    * [Photoview :page_with_curl:](https://fossengineer.com/selfhosting-Photoview-docker/) :heavy_check_mark: -> file system friendly
    * Piwigo
  * RClone :heavy_check_mark:
  * RSync
  * RSnapshot
  * [Samba](https://fossengineer.com/selfhosting-samba/) :heavy_check_mark:
  * Seafile
  * Syncthing :heavy_check_mark:
    
### [Business:](https://github.com/JAlcocerT/Docker/tree/main/Business)
   * ERPs:
      * ERPNext
      * Dolibarr :heavy_check_mark:
      * Odoo (ex- OpenERP) :heavy_check_mark:
    * Invoicing:
      * Crater Invoices
      * Invoice Ninja
      * Solid Invoice (x86 only)
    * Management:
       * Vikunja :heavy_check_mark:
       * Leantime (x86 & ARM, :heavy_check_mark:)
### [Communication:](https://github.com/JAlcocerT/Docker/tree/main/Communication)
   * Chats:
       * Discourse 
       * Jitsi
       * [Matrix with Synapse :page_with_curl:](https://fossengineer.com/selfhosting-matrix-synapse-docker/) :heavy_check_mark:
       * Revolt
       * RocketChat
   * Mail:
       * iRedMail
       * Mailcow
       * Mailinabox
       * Mailserver
       * Mailu (rspamd)
       * Poste
       * Postfix
   * FreshRSS :heavy_check_mark:
### [Dev](https://github.com/JAlcocerT/Docker/tree/main/Dev)
* [Gitea](https://fossengineer.com/selfhosting-Gitea-docker/) :heavy_check_mark:
* [Gogs](https://fossengineer.com/selfhosting-Gogs-with-Docker/)
* Gitlab CE
* VSCode Server
* [Jenkins](https://fossengineer.com/selfhosting-jenkins-ci-cd/)
* Airflow
* Gitbucket
* OneDev #includes kanban board
* SnippetBox :heavy_check_mark:
* [Python DASH Apps :page_with_curl:](https://fossengineer.com/dash-docker-gcr/)
* [Shiny Dashboards](https://fossengineer.com/building-r-shiny-apps-container-image-with-docker/)   
### [IoT:](https://github.com/JAlcocerT/Docker/tree/main/IoT)
* Automations:
  * Domoticz
  * [Home Assistant](https://jalcocert.github.io/RPi/posts/rpi-iot-dht11-influxdb/#how-can-i-install-home-assistant) :heavy_check_mark:
  * Home Bridge
  * OpenHab
* [Internet speed tracker](https://jalcocert.github.io/RPi/posts/self-internet-monit/#speedtest-tracker) :heavy_check_mark:
* [OpenSpeedTest](https://jalcocert.github.io/RPi/posts/self-internet-monit/#openspeedtest) :heavy_check_mark:
* GPIO
  * TIO: https://github.com/tio/tio
* BI:
  * [Metabase](https://jalcocert.github.io/RPi/posts/rpi-iot-dht1122-mongo/#metabase)
  * [Apache Superset](https://jalcocert.github.io/RPi/posts/rpi-gps-superset/#apache-superset-setup)
  * Redash
* Dashboards:
  * [NetData](https://fossengineer.com/selfhosting-server-monitoring-with-netdata-and-docker/) :heavy_check_mark:
  * Grafana with Prometheus (internet speed) :heavy_check_mark:
  * Grafana with Prometheus (internet + device with node exporter)
  * Grafana with Graphite StatsD
  * Grafana with InfluxDB (Temperature measuring)
  * Grafana with Proxmox and InfluxDB
  * Grafana with Proxmox and Graphite
  * Grafana with Node-Red
  * Grafana + cAdvisor
  * EFK stack for logs(Elastic search, Fluentd, Kibana)
  * ELK stack (ES, Logstash, Kibana)
  * GOtify
  * Ntfy (notify)
  * [Uptime Kuma :page_with_curl:](https://fossengineer.com/selfhosting-uptime-Kuma-docker/) :heavy_check_mark:
  * Flame :heavy_check_mark:   
  * Homerr
    
### [Media](https://github.com/JAlcocerT/Docker/tree/main/Media)
* E-Books/Podcasts
  * Calibre :heavy_check_mark:
  * Kavita
  * Koodo reader
  * Audiobookshelf :heavy_check_mark:
  * Podgrab :heavy_check_mark:
* Photos: 
  * PiGallery :heavy_check_mark: -> Photo location, GPX support & file system friendly friendly (no DB required) :rocket:
* Entertainment  
  * Jellyfin :heavy_check_mark:
  * Kodi
  * Plex
  * Emby
  * Couchpotato :heavy_check_mark:
  * Jacket :heavy_check_mark:
  * Mylar3
  * Midarr      
  * Calibre :heavy_check_mark:
  * Readarr
  * P2P
    * Transmission :heavy_check_mark:
    * rTorrent :heavy_check_mark:
    * [Qbittorrent](https://fossengineer.com/selfhosting-qBittorrent-with-docker-and-VPN) :heavy_check_mark:
    * Radarr :heavy_check_mark:
    * Sonarr :heavy_check_mark:
    * Bazar :heavy_check_mark:
    * JDownloader
* ArchiveBox
* Music
  * Ampache
  * Supysonic :heavy_check_mark:
  * Navidrome :heavy_check_mark:
* Mumble

### [Security:](https://github.com/JAlcocerT/Docker/tree/main/Security)
* Authelia  
* Blocky
* [Cloudflare - Zero Trust Tunnel :page_with_curl:](https://fossengineer.com/selfhosting-cloudflared-tunnel-docker/) :heavy_check_mark:
* Crowdsec 
* DNS:
  * CoreDNS
  * Unbound :heavy_check_mark:
  * [Pihole :page_with_curl:](https://fossengineer.com/selfhosting-PiHole-docker/) :heavy_check_mark: 
  * PiHole + Cloudflare (DNS over HTTPs)      
* EndleSSH
* Fail2ban 
* LAN:
  * [Watchyourlan](https://fossengineer.com/selfhosting-WatchYourLAN-docker/) :heavy_check_mark:
  * Wireshark :heavy_check_mark:
  * Pi-Alert  
* Privacy:
  * [Whoogle :page_with_curl:](https://fossengineer.com/selfhosting-whoogle-docker/) :heavy_check_mark:
  * SearX :heavy_check_mark:
* Proxies
  * Caddy 
  * [NGINX + SSL + DuckDNS :page_with_curl:](https://fossengineer.com/selfhosting-nginx-proxy-manager-docker/) :heavy_check_mark:
  * NGINX + SSL + Fail2ban
  * NGINX + SSL + Fail2ban + Authelia
  * Traefik
  * Traefik + failban
* VPN's
  * [Gluetun :page_with_curl:](https://fossengineer.com/using-bard-selfhosting-firefox-with-vpn-docker/)
  * OpenVPN
  * [Tailscale]()
  * Headscale
  * Wirehole
  * Wireguard :heavy_check_mark:
* Watchtower :heavy_check_mark:
    
###  Others:
* Management:
  * Bookstack
  * [Focalboard](https://fossengineer.com/focalboard-docker/) :heavy_check_mark:
  * Joplin (x86 only)
  * Kanboard :heavy_check_mark:
  * Logseq
  * OpenProject (Asana alternative)
  * [Leantime :page_with_curl:](https://fossengineer.com/selfhosting-Leantime-docker/) :heavy_check_mark:
  * [Timtelite](https://fossengineer.com/selfhosting-timelite-free-tracking-tool-with-docker/)
  * Personal management system
  * [Trilium](https://fossengineer.com/selfhosting-Trilium-docker/) :heavy_check_mark:
  * Tiddlywiki
  * Wecan (Kanban board)
* Youtube
  * MeTube :heavy_check_mark:
* Grocy :heavy_check_mark:
* [Firefox :page_with_curl:](https://fossengineer.com/using-bard-selfhosting-firefox-with-vpn-docker/)
* [WebTops](https://fossengineer.com/selfhosting-webtops-with-docker/)
* Libretranslate
* Design
  * Penpotapp
  * [Drawio](https://fossengineer.com/selfhosting-drawio-with-docker/)


### [Web](https://github.com/JAlcocerT/Docker/tree/main/Web)
* Analytics
  * Matomo
  * Plausible
  * Posthog <https://posthog.com/docs/self-host>
  * Umami :heavy_check_mark:
* Comment Engine
  * remark42
  * Isso
  * Giscus
* Dynamic DNS
  * DuckDNS :heavy_check_mark:
  * No-IP
* CMS/Sites
  * Bludit
  * [HUGO :page_with_curl:](https://fossengineer.com/web-guide-Hugo/) 
  * [Wordpress :page_with_curl:](https://fossengineer.com/selfhosting-wordpress-docker/) :heavy_check_mark:
  * [Ghost :page_with_curl:](https://fossengineer.com/selfhosting-ghost-docker/)
* Forms (HTML)
  * Alpaca
  * Drupal
  * OhMyForm
* Instagram alternatives
  * [Chevereto](https://fossengineer.com/selfhosting-chevereto-docker/)
  * Pixelfed
  * Vero
* Static Web Server
  * [Apache :page_with_curl:](https://fossengineer.com/Selfhosting-Static-Webs-with-Apache-in-Docker/) 
  * NginX
* Subscriptions
   * Keila
   * Mailtrain
   * Moodle

**Legend:**
  * :heavy_check_mark: -> Self-hosting instructions available in this repository
  * :page_with_curl: -> Detailed instructions available in [my tech blog](https://fossengineer.com/).

</details>

### AI-Gen

* [Ollama with Docker](https://fossengineer.com/selfhosting-llms-ollama/)
* [PrivateGPT with Docker](https://fossengineer.com/selfhosting-local-llms-with-privateGPT/)
* [TextGenWebUI with Docker](https://fossengineer.com/Generative-AI-LLMs-locally-with-cpu/)


## Powered Thanks To :heart:

* Markdown
* The fantastic community on the internet from where I've learnt the basis to put together all of this.

## :loudspeaker: Ways to Contribute 

Please feel free to fork the repository - try it out the guide for yourself and improve or add other config files.

If you enjoy self-hosting any of the apps listed, I would show appreciation directly to their creators. Please check the specific project for more details on that.

* If any of the docker-compose files or associated tutorials was helpful and you want to show gratitude:
 * Consider leaving feedback if you found some improvement / something can be explained better
 * Support additional weekends of self-hosting tinkering to bring new services to the list

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/FossEngineer)