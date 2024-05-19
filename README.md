# CackalackaBadgy 2024

After [CackalackyCon 2024](https://cackalackycon.org/index.html) finishes up, we'll post the developers version of the firmware that was used for debugging and testing as well as more information about the badge.

## Badge Stats from the conference 
- 164 users built the badge **and** registered them
- 619 scores were logged
- The average alcohol reading over the weekend was 771 (meaning on avg, the con collectively was slightly intoxicated)
- We recorded 22hrs and 30 mins of gameplay across all games on all badges
- Badge bot tagged @sq33k a total of 40 times

## Serial Port things in the Conference Firmware 0.9.13

### Acheivements and Unlocks
- Winning Circle Jerk unlocks Labyrinth
- Using the breathalyzer unlocks Breakout
- Using <HELLOWORLD> on Serial
- Submitting secret flag in AP webapp to the badge form unlocks asteroids
- Getting rickrolled

### Unlocking asteroids
**Spoiler alert**

[Here is a short writeup](https://github.com/lockfale/cackalackabadgyfirmware2024/blob/main/AccessPointChallenge.md) on how to unlock asteroids, if you are stumped. 

### Default Serial commands
```
<HELP> - What it says...
<STATUS> - Gives you an idea of what is going on. Progress and such.
<HELLOWORLD> - Command that gives user an idea of how to use the commands and unlocks HelloWorld acheivement.

<WE> - Draws Wave Emoji
<TE> - Draws Taco Emoji
<MFE> - Draws Middle Finger Emoji

<RESETWIFI> - resets the wifi settings back to badgenet
<SETSSID> - sets the ssid
<SETPASS> - sets the wifi password

<DELPROG> - deletes their progress on the badge. Locks games
<RID> - shows the badge's real id
<UUID> - shows the badge's UUID
```

## Those responsible
* [@melvin2001](https://github.com/melvin2001)
* [@nutcrunch](https://github.com/persinac)
* [@pandatrax](https://github.com/pandatrax)
