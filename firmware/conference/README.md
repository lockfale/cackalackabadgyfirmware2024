# Badge firmware that was used during CackalackyCon 2024

Flash the badge and **NOT** overwrite the FFS
```
esptool -b 921600 --chip esp8266 write_flash 0x0 firmware-0.9.13.bin
```
