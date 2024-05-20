# Badge firmware used during CackalackyCon 2024

## Flashing the badge
Flash the badge and **NOT** overwrite the FFS
```
esptool -b 921600 --chip esp8266 write_flash 0x0 firmware-0.9.13.bin
```

## Default Serial commands in this version
```
<HELP> - What it says...
<STATUS> - Gives you an idea of what is going on. Progress and such.
<HELLOWORLD> - Command that gives user an idea of how to use the commands and unlocks HelloWorld acheivement.

<WE> - Draws Wave Emoji
<TE> - Draws Taco Emoji

<RESETWIFI> - resets the wifi settings back to badgenet
<SETSSID> - sets the ssid
<SETPASS> - sets the wifi password

<DELPROG> - deletes their progress on the badge. Locks games
<RID> - shows the badge's real id
<UUID> - shows the badge's UUID

<APSTART> - Starts the access point when Access Point has been unlocked
<APSTOP> - Stops the access point when Access Point has been unlocked
```
