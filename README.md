This filter list was created 2015 and is under MIT license by CHEF-KOCH and contains all the advertising domains which are hard-coded within Spotify (free account). <br/>

The project is unofficial and not in any relationship with [Spotify AB](https://en.wikipedia.org/wiki/Spotify). <br/>

Current Spotify Release: [Spotify 1.1.237](https://download.scdn.co/SpotifyFullSetup.exe), see [here](https://github.com/CHEF-KOCH/Spotify-Ad-free/releases/tag/2.3) for mod infos.

# Project is closed and merged within [CK's-FilterList](https://github.com/CHEF-KOCH/CKs-FilterList)!


[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/fold_left.svg?style=social&label=Follow%20%40CHEF-KOCH)](https://twitter.com/CKsTechNews)
[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/CHEF-KOCH)
[![Discord](https://discordapp.com/api/guilds/418256415874875402/widget.png)](https://discord.me/CHEF-KOCH)

You can easily import the list into any Adblocker.


### Bypass ToS (?)

* The current ToS (see link below) only affects America and Europe, Swiss is not affected. My advice is to setup a Proxy/VPN for Spotify which connects to Swiss in order to _bypass_ (needs confirmation) the ToS in case you're account get banned you can then win this case and the swiss server in general have less ads (needs confirmation).

An additional advice is to set this:

- Edit - Preferences (CTRL + P) - Privacy _Block all cookies..._ (enable it)
- Edit - Preferences (CTRL + P) - Advertisement - Change advertising preferences (disable everything here on the Spotify website)

This helps to getting tracked by cookie leftovers and reduces the chance to see banner ads (it does not remove them). 


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


### Release & RePack information

I do not officially maintain the project which means every work I still do is for the community only and for free, no one is forced to download something from the [release tab](https://github.com/CHEF-KOCH/Spotify-Ad-free/releases) nor do I support something illegal stuff here. Repacking the installer is not illegal, however modifing the files itself is because it's against ToS (which I respect) but including several additional patches and a hosts file seems okay to me.


### Other Resources

* [abertschi/ad-free (github.com)](http://adfree.abertschi.ch) A modularized Ad Blocker for Spotify on Android.  
* [BlockTheSpot](https://github.com/master131/BlockTheSpot/) Spotify injection (for the Desktop version only) which blocks video, audio & banner
* [Spotify Terms and Conditions of Use](https://www.spotify.com/us/legal/end-user-agreement/#s9)

