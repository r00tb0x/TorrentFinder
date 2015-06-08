## TorrentFinder
TorrentFinder.sh is a "simple" bash script that uses wget, grep, etc. to list the top 5 torrents found on each of the 8 sites based on the search you made. tested and working on archlinux TorrentFinder should work on any other linux distro, i've seen problems when using OSX. I have  tested it in cygwin and it's working just fine
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
    
### Cygwin
when you have installed wget and git in cygwin you can make program automaticly launch TorrentFinder when launched
    
     cd; git clone "https://github.com/m3k4/TorrentFinder"; mv TorrentFinder/TF.sh /usr/local/bin; cd; echo "printf '\e[8;34;230t'" >> .bashrc; echo "for (( ; ; )) do bash TF.sh; done" >> .bashrc; exit

    
## Demo

https://asciinema.org/a/ahp6bvx8jdaae6a4q9wkdemzs

## INFORMATION TO THE USER!
i'm not responsable if you download any illigal torrents using this script!
and big thanks to http://unbanthe.org/ for providing a proxy.
