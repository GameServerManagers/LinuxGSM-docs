# Killing Floor 2

## Ports

* **Game Port** Default: 7777 UDP Handled by: `LinuxServer-KFEngine.ini` 
* **Query Port** Default: 27015 UDP Handled automatically or handled by parameters. Formula for finding query port assigned automatically is 19238 + assigned game port. 
* **Web Admin** Default: 8080 TCP Handled by: `KFWeb.ini` 
* **Steam Port** Default: 20560 UDP Handled automatically. Formula for finding steam port is 12783 + assigned game port.

## Resources

[Killing Floor 2 Official Server Wiki](https://wiki.tripwireinteractive.com/index.php?title=Dedicated_Server_%28Killing_Floor_2%29)

[Killing floor 2 Official Forums](https://forums.tripwireinteractive.com/index.php?categories/killing-floor-2.25/)

## Server Config Information

Default LinuxGSM installs have `configSubDir=servername` set in the command line which will set your priority config files to be in `/home/user/serverfiles/KFGame/Config/kf2server` directory, use these files to change settings on your server.

## Workshop Content

Killing Floor 2 supports [Steam Workshop](../steamcmd/workshop.md).

### High disk IO using Steam Workshop

Killing Floor 2 will check workshop files at server start and when map changes occur.

There is a potential problem with Killing Floor 2 servers using the steam workshop that causes server disk usage to read/write at 100% and could damage hardware.

To avoid this problem keep the amount of workshop content as low as possible. 

Disk IO can be monitored with the `ioptop` command.

**References:**

[TWI you destroyed my SSD forum post](https://forums.tripwireinteractive.com/index.php?threads/twi-you-destroyed-my-kf2-servers-ssd.2334936/)

[Server is going disk drive crazy forum post](https://forums.tripwireinteractive.com/index.php?threads/server-is-going-disk-drive-crazy.2333489/)

[Workshop map disk thrashing forum post](https://forums.tripwireinteractive.com/index.php?threads/workshop-map-disk-thrashing-is-back.2335275/)









