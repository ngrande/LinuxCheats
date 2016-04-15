# Cheat sheet!

## accidentally removed packages?
Run: `awk '!/^Start|^Commandl|^End|^Upgrade:|^Error:/ { gsub( /\([^()]*\)/ ,"" );gsub(/ ,/," ");sub(/^Install:/,""); print}' /var/log/apt/history.log` to get a list of you recently uninstalled packages.  
Copy and paste all needed packages and put them in `apt-get install {packages}`.

## Hardware information
### CPU
`cat /proc/cpuinfo`
