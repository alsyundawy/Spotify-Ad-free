### FAQ

A small FAQ and additional background info on certain things which are Spotify (ads) related.

### Official clients & download information

* [Android Alpha Google Group](https://groups.google.com/forum/#!forum/spotify-android-alpha/join)
* [Android Beta Google Group](https://groups.google.com/forum/#!forum/spotify-android-beta/join)
* [Android App Testing Page](https://play.google.com/apps/testing/com.spotify.music)
* [Official Play Store link](https://play.google.com/store/apps/details?id=com.spotify.music)
* [Unofficial Linux Mint Link](http://packages.linuxmint.com/search.php?release=any&section=any&keyword=spotify)
* [Official MacOS Link](https://download.scdn.co/Spotify.dmg)
* [Official Linux Link](https://www.spotify.com/de/download/linux/)
* [Microsoft Store Version] (UWP app)(https://www.spotify.com/us/download/other/)
* [Spotify Kids](https://www.spotify.com/ie/kids/)


I provide untouched official mirrors as they come, in case someone wants to manually up-/downgrade. Spotify itself in fact does keep backups of all their client releases but they don't post the links public.


### Bypassing ToS (_needs confirmation_)

* The current ToS (see link below) only affects America and Europe, Swiss is not affected. My advice is to setup a Proxy/VPN for Spotify which connects to Swiss in order to _bypass_ (needs confirmation) the ToS in case you're account get banned you can then win this case and the swiss server in general have less ads.


### How to capture ads on Windows?

* Flush your DNS cache `ipconfig /flushdns`, then run [DNSQuerySniffer](http://www.nirsoft.net/utils/dns_query_sniffer.html) and your Spotify Client
* After an audio Ads appears save domains list via DNSQuerySniffer. 
* In order to provide a useful _Pull request_ or _Bug report_ ensure you're use the latest Spotify version. 


### How to capture ads on Android?

* Install AdGuard, ensure HTTPS filtering is globally activated and enabled for the Spotify application. 
* Enable DNS filtering.
* Go to filter log and export the list. You can click on the domains and block them and export the list in order to provide a useful Pull Request.


### How to enable the Spotify Audio Routing function?

* Using _--enable-audio-graph_ at the end of the Spotify shortcut target address will enable the Playback device selection box!


### How to disable Spotify auto update (without blocking domains in HOSTS)?

```
// Open Command Prompt with Admin rights:
icacls "%localappdata%\Spotify\Update" /reset /T

del /s /q "%localappdata%\Spotify\Update"

mkdir "%localappdata%\Spotify\Update"

icacls "%localappdata%\Spotify\Update" /deny "%username%":W
```

### How to get Spotify premium for ~ 2 €/Dollars

- Use a VPN and use one of the following locations: Argentina, Vietnam, Philippine, Brazil
- The url is always the same `http://spotify.com/ph/signup` only the `/ph/` part changes which points to the location in this example it points to the philippines. 
- Some countries censorship the spotify content e.g. India, so don't use such countries.


### Spotify updating mechanism
The UWP Spotify app gets updates _quicker_ since they are automatically compiled (which explains the strange [versions scheme](https://en.wikipedia.org/wiki/Software_versioning) which means the Win32 apps are uploaded around 4-10 days later (depending how fast Spotify rolls them out).


### Preventing updates on MacOS (untested)
The user [julionc](https://github.com/julionc) wrote a small script to prevent updates on MacOS.

* Uninstall all old Spotify versions on your MacOS.
* Install a Spotify MacOS version [below 1.0.80](https://mac.filehorse.com/download-spotify/10400/). 
* Open and [copy the file](https://github.com/julionc/dotfiles/blob/9990859cf4de0536d0d2b4351c3f19dec9fdfd48/osx/doNotUpdateSpotify.sh) to `whatever.sh`. 
* Save the file on your desktop and open the MacOS terminal, enter `cd desktop` and then execute `sudo sh whatever.sh`.

The script will block Spotify from updating itself. Alternative _solutions_ are [Spotifree](https://github.com/simonmeusel/MuteSpotifyAds#alternatives) & [MuteSpotify Ads](https://github.com/simonmeusel/MuteSpotifyAds). If all of it fails, uBlock is still working (Spotify Web) on all systems without any need for installing third-party software on your OS.


### Block Spotify updates (on other systems)
* [spotify_version_keeper (github.com)](https://github.com/SrMordred/spotify_version_keeper) - A small app which prevents Spotify updates on Windows. 


### How to bypass Spotify's location data sharing on Android

The SPotify mobile apps requiring that you share your location, this is an privacy attack and (by default) there is no way to turn it off (except blocking the update itself which introduced the feature). However in order to deal with the new Spotify "gimmick" there are ways to protect your privacy without breaking the app and without downgrading to another Spotify version.


* Download a [GPS spoofing app](https://play.google.com/store/search?q=gps%20spoof) e.g. [Fake GPS location](https://play.google.com/store/apps/details?id=com.lexa.fakegps) (there are also bunch Magisk & Xposed based solutions in the official stores avbl.)
* Enable Developer options
* Select mock location app
* Spoof your location, choose and give the gps spoofing app your fake data


### Anti-debugger protection in Spotify 
* [Spotify vs OllyDbg (2009) (web.archive.org)](https://web.archive.org/web/20130417061130/http://www.steike.com/code/spotify-vs-ollydbg/) 

### [BlockTheSpot](https://github.com/mrpond/BlockTheSpot/commits/master)
Since Spotify 1.14+ the [".dll"-trick does not work anymore](https://github.com/master131/BlockTheSpot/issues/19), you have to downgrade to a lower Spotify version and prevent the update mechansim. Spotify will monitor such repos and add other protections in order to prevent such things, so at the end dowgrading is the best way to avoid getting ads. Please keep in mind that Spotify could force their users to use the latest clients, which then would mean that no such dll injection methods would work anymore (or break with another update). 

