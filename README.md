## TorrentFinder
TorrentFinder.sh is a "simple" bash script that uses wget, grep, etc. to list the top 5 torrent based on the search you made. tested and working on archlinux TorrentFinder should work on any other linux distro, i've seen problems when using OSX. I have not tested it in cygwin
### Sites it scans
    
    Kickass
    The piratebay
    1337x
    Iso Hunt
    Torrent Hound
    seedpeer
    Lime Torrents
    YTS 
    
## Installation and usage

    git clone https://github.com/M3K4/TorrentFinder
    cd TorrentFinder
    bash TF.sh
    
### OSX
to get it working on osx you need homebrew installed and the more up to date software

    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    brew tap homebrew/dupes; brew install bash grep gnu-sed
    
## Demo

https://asciinema.org/a/ahp6bvx8jdaae6a4q9wkdemzs

## INFORMATION TO THE USER!
i'm not responsable if you download any illigal torrents using this script!
and big thanks to http://unbanthe.org/ for providing a proxy.
