# Technical Guide

This documents provides a technical description of how Pickflix operates. All of
the source for Pickflix is open to view on GitHub at
[wyomatthew/pickflix](https://github.com/wyomatthew/pickflix).

## Service Architecture

Below is a diagram describing the architecture and software stack of Pickflix:

<img src="images/diagram.svg" alt="Pickflix Architecture Diagram" stroke="none" fill="none"/>

### Reverse Proxy

[nginx](https://nginx.org/) is used as a reverse proxy to route the incoming
traffic.

### Jellyseerr

[Jellyseerr](https://github.com/Fallenbagel/jellyseerr) allows users to make
media requests from a media metadata store.

### Wizarr

[Wizarr](https://github.com/wizarrrr/wizarr) handles all user onboarding,
including generating user invitation links.

### Jellyfin

[Jellyfin](https://jellyfin.org/) provides a user-friendly streaming platform
available across a wide range of devices.

### Radarr

[Radarr](https://radarr.video/) processes user requests for movies. It receives
requests from [Jellyseerr](#jellyseerr), searches for a corresponding .torrent
file in its indexers, and passes the torrent to [qBittorrent](#qbittorrent).

### Sonarr

[Sonarr](https://sonarr.tv/) process user rqeuests for series. It receives
requests from [Jellyseerr](#jellyseerr), searches for a corresponding .torrent
file in its indexers, and passes the torrent to [qBittorrent](#qbittorrent).

### Prowlarr

[Prowlarr](https://prowlarr.com/) acts as an index manager for [Radarr](#radarr)
and [Sonarr](#sonarr). It provides a unified interface for administrators to
select what indexers to search and keeps them synced.

### qBittorrent

[qBittorrent](https://www.qbittorrent.org/) is the torrent client used to
download the actual media content.

### Bazarr

[Bazarr](https://www.bazarr.media/) is a subtitle manager for [Radarr](#radarr)
and [Sonarr](#sonarr). It maintains its own set of subtitle indexers and grabs
missing subtitles for downloaded releases.

### PIA VPN

[PIA VPN](https://www.privateinternetaccess.com/), or Private Internet Access,
proxies all intranet traffic to anonymize internet activity.

## Deployment Environment

All self-hosted services (ie all applications within the "PICKFLIX" box in the
[service architecture](#service-architecture)) are hosted as Docker containers
on a custom-built home server. The server contains **26TB** of storage for
storing media ready to be streamed.
