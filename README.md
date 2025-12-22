# TJT Media Server

Welcome to TJT Media Server - your personal, all-in-one home media management and streaming solution.

## 🎯 What It Does

TJT Media Server is a comprehensive home media server that provides:

- **Media Streaming**: Watch your movies, TV shows, and listen to audiobooks from anywhere
- **Content Management**: Automatically organize, download, and manage your media library
- **Request System**: Family-friendly interface to request new content
- **Quality Control**: Automated monitoring and upgrading of media quality
- **Universal Access**: Stream to any device - phones, tablets, smart TVs, and computers

## 🏗️ How It Works

TJT Media Server integrates several specialized applications that work together to create a seamless media experience:

### Media Consumption

#### 📺 Jellyfin
Your personal streaming platform - think Netflix, but for your own content.
- Stream movies and TV shows to any device
- Automatic metadata and artwork fetching
- User profiles with watch history and recommendations
- Mobile apps for iOS and Android

#### 📚 Audiobookshelf
Dedicated audiobook and podcast server
- Beautiful interface for audiobook management
- Progress tracking across devices
- Sleep timer and playback speed controls
- Chapter navigation

### Content Management

#### 🎬 Radarr
Automated movie collection manager
- Searches for movies across multiple sources
- Monitors for new releases and upgrades
- Automatically organizes your movie library
- Quality profile management

#### 📡 Sonarr
TV series automation system
- Tracks your favorite shows
- Automatically downloads new episodes as they air
- Season pack management
- Missing episode detection

#### 🔍 Prowlarr
Indexer manager and proxy
- Centralized management of all your content sources
- Integrates with Radarr, Sonarr, and other tools
- Health monitoring and testing
- Automatic indexer syncing

### Infrastructure

#### 🌊 qBittorrent
Download client
- High-performance torrent client
- Web-based interface
- Bandwidth management
- Integration with Radarr and Sonarr

#### 🎭 Jellyseerr *(Coming Soon)*
Media request and discovery platform
- User-friendly interface for requesting movies and TV shows
- Integration with Radarr and Sonarr
- Request approval system
- Discover trending and popular content

## 🔄 The Workflow

Here's how everything works together:

1. **Discovery**: Browse content using Jellyfin or request new media through Jellyseerr
2. **Request**: When you want something new, Jellyseerr sends the request to Radarr (movies) or Sonarr (TV shows)
3. **Search**: Radarr/Sonarr searches through Prowlarr's indexers to find the content
4. **Download**: Once found, qBittorrent handles the download
5. **Organization**: After downloading, Radarr/Sonarr automatically organizes the files into your library
6. **Enjoyment**: The content appears in Jellyfin or Audiobookshelf, ready to stream!

## 🚀 Getting Started

### Accessing the Services

Each service is accessible through its own web interface:

- **Jellyfin**: Your main streaming interface
- **Audiobookshelf**: For audiobooks and podcasts
- **Jellyseerr**: Request new content *(coming soon)*

### For Administrators

- **Radarr**: Manage movie collection
- **Sonarr**: Manage TV shows
- **Prowlarr**: Configure indexers
- **qBittorrent**: Monitor downloads

## 🛠️ Technical Stack

- **Frontend**: Web-based interfaces for all services
- **Media Server**: Jellyfin (open-source)
- **Audiobook Server**: Audiobookshelf (open-source)
- **Automation**: Radarr, Sonarr, Prowlarr (*arr stack)
- **Download Client**: qBittorrent
- **Request Management**: Jellyseerr (pending implementation)

## 📋 Features

- ✅ Automatic media organization
- ✅ Multi-user support with individual profiles
- ✅ Cross-platform streaming (Web, iOS, Android, Smart TV)
- ✅ Quality monitoring and upgrades
- ✅ Metadata and artwork management
- ✅ Watch progress synchronization
- ✅ Mobile apps support
- 🔜 Media request system (Jellyseerr)

## 🔐 Privacy & Security

All services run locally on your home network, ensuring:
- Your data stays private
- No subscription fees
- Full control over your media
- No external dependencies for playback

## 📞 Support

For assistance with the TJT Media Server:
- Check individual service documentation
- Review logs for troubleshooting
- Contact your system administrator

---

**TJT Media Server** - Your media, your way. 🎬🎵📚