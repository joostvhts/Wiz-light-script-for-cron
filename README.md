My own version, in Bash script form, of the 'rhythm' function in Wiz's Android app due this function's very limited customizability.

This script is intended to be run by cron every x minutes (I use 30). It's basically a wrapper for the node/bash commands developed by <WHO AGAIN?> (available from npm) <LINK> and calls commands that integrate the time of day. The script grabs the current time, looks up the appropriate light temperature (K) and brightness (0-255) then runs `wizlight` along with those calculated values.
