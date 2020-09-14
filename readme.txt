Documentation:
    For a first time start run in a commandline:
        npm install
        npm run start
    or 
        npm cleanStart
		
	From the 2nd time onwards you can use the autostart.bat files or run npm run start.
		
Available commands:
    !servers list of all servers
    !serverStatus [server] prints whether a given server is up or down, if no server is given it'll print the status for all servers
    !playerCount [server] prints the number of players on a given server, if no server is given it'll print the player count for all servers
    !serverdetail [server]/!serverdetails [server] prints the server details of a given server, if no server is given it'll print the server details for all servers
    !players [server] prints the players connected to the current server.  Requires a server
    !ping replies pong
    !info/!version prints version number of this bot as well as contact information for my maintainer
    !botstatus prints uptime of the bot and number of queries handled by the bot
    !commands/!help this
    
Commands only available for admins:
    !rssAdd [link] adds an rss feed, specified by the link, in the channel the command is executed.
    !rssRemove [link] remove an rss feed, specified by the link.
    !rssList lists all the rss feeds in all the channels on server
    !changeNotifyStatus [on/off]/ !toggleNotify [on/off] toggles whether a notification will be send for the given server being down
    !reloadConfig reloads the config file
    !toggleLogging [server] toggles whether logs should be kept for a server
    !subscribeForDownPing/!unsubscribeForDownPing to subscribe/unsubscribe you from mentions when servers go down
    !saveconfig/!saveconf to save the config (it's strongly advised to run this after running ${prefix}subscribeForDownPing or ${prefix}unsubscribeForDownPing)
    !maintenance [server] [duration]/ !tempmute [server] [duration] to suspend down notifications for a given server for the given duration in minutes (10 minutes if no value is passed)
    !makeservervisible [server] to make a server visible for everyone
    !changedefaultmission [server] [missionName] to change the default mission of a server.  Mission name must be the exact file name.
    !listmissions [server] to list all missions for a given server
    !uploadmission [server] [file] to upload a mission to a given server.  File must be a PBO.
    !startserver [server]/!launchserver [server] to start a server (attention, no checks are done to ensure that the server isn't already started)
    !stopserver [server]/!killserver [server]to stop a server that was started using this bot
    !extendeddebug [on/off] to enable or disable extended debug information (in the console, not here) (if on or off isn't passed it'll select the other value
    !shutdownbot to gracefully shut down the bot.  Consider saving the config before doing this.
		
For auto start with windows:
	Make a copy of autostart.bat and put it in the following folder:
	C:\Users\*yourUser*\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup
	Make sure to replace the path in that file with the actual path where you've put that bot on your machine.