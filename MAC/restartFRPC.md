# step to restart frpc in MAC

## step 1 : go to directory /Library/LaunchAgents
    cd /Library/LaunchAgents
## step 2 : check frpc status
    launchctl list | grep fr
  
## step 3 : stop frpc service
    launchctl stop frpc
    launchctl unload frpc.plist

## step 4 : start frpc service
    launchctl load frpc.plist
