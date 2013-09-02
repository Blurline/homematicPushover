CUxD muss installiert sein

Aufruf im homematic Programm:
string nachricht = "<Text>";
dom.GetObject("CUxD.CUX2801001:1.CMD_EXEC").State("LD_LIBRARY_PATH=/usr/local/addons/cuxd /usr/local/addons/cuxd/curl -s -k -d token=<Application Token> -d user=<User/Groupkey>  -d message='"#nachricht#"' -d priority=1 -d sound=none https://api.pushover.net/1/messages.json");
