# tmux-mpd
 🎵 A dead simple script for MPD status in your tmux bar
## Requirements
The requirements are nothing you shouldn't already have - bash, sed, grep, cut, and mpc - chances are if you're on any modern Linux distribution, you'll only need to install mpc to get this functioning.
## Installation and Usage
Move the bash script to your path, make sure it's executable (`chmod +x tmux-mpd`) and congratulations - you've got the module installed.

For usage in tmux, it's as simple as adding `#(tmux-mpd)` to your status bar lines in your tmux config. Make sure there's no detatched sessions running (aka "restart" tmux), and you've got your tunes in every window pane you go to!

## Side Note
Yes, I know this is janky - I built it to work for me, not to be the prettiest piece of shell script I've ever wrote. The semicolon parsing is for Mopidy-spotify support when a track has multiple artists, but if you're just using traditional MPD/Mopidy with local files exclusively, it'll likely just be redundant parsing.
