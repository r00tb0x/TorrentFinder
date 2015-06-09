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

### aliases
if you have added the 2 aliases to your .bashrc just type TF to run the script and UTF to update it

    alias UTF="cd /usr/local/bin; sudo rm -rf TorrentFinder; sudo git clone https://github.com/m3k4/TorrentFinder; sudo rm TF; sudo mv TorrentFinder/TF.sh /usr/local/bin/TF; sudo chmod +x TF; cd"
    alias TF="bash TF"
    
### OSX
To get it working on osx you need homebrew installed and the more up to date software and you need to complie sed form source 

    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    brew tap homebrew/dupes; brew install wget bash grep cmake
    wget https://ftp.gnu.org/gnu/sed/sed-4.2.tar.gz; tar -xvf sed-4.2.tar.gz; cd sed-4.2; ./configure; make; sudo make install
    
### Cygwin
When you have installed wget and git in cygwin you can make cygwin automatically launch TorrentFinder when launched
    
     cd; git clone "https://github.com/m3k4/TorrentFinder"; mv TorrentFinder/TF.sh /usr/local/bin; cd; echo "printf '\e[8;34;230t'" >> .bashrc; echo "for (( ; ; )) do bash TF.sh; done" >> .bashrc; exit

    
## Demo

https://asciinema.org/a/ahp6bvx8jdaae6a4q9wkdemzs

## INFORMATION TO THE USER!
i'm not responsable if you download any illigal torrents using this script!
and big thanks to http://unbanthe.org/ for providing a proxy.
