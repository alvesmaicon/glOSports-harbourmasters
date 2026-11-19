Ship of Harkinian (Ocarina of Time) and 2 Ship 2 Harkinian (Majora's Mask) for goodluckOS, as apps for its App Installer or to install by hand. The zips are the ports only, with nothing of the games in them: each one plays your own ROM.

**You need** a GA36-MB with goodluckOS and your ROM: for Ship of Harkinian a version it takes (N64 1.0 to 1.2 or PAL, GameCube or Master Quest), for 2 Ship 2 Harkinian the N64 USA version (1.0) or the GameCube USA one.

1. Copy `ShipOfHarkinian-*.zip` and/or `2Ship2Harkinian-*.zip` to the `apps` folder of the console's HOME (over USB, where the console shows up as a drive, or with the card in a card reader) and install them in the App Installer, in the launcher's row with the restart and power off buttons. They show up in the launcher. Without the App Installer, see below.
2. Copy your ROM to HOME, as a `.z64`, `.n64` or `.v64` file or a zip of one.
3. Open the game. The first time, it finds your ROM and makes its assets from it, in a window that shows how far it has got; then the game starts, and from then on it starts straight away.

**Without the App Installer** (it is not in every goodluckOS image yet): unzip each zip into the `apps` folder of HOME, so that there is `HOME/apps/ShipOfHarkinian` or `HOME/apps/2Ship2Harkinian`, add the game to `HOME/apps.puppy` as below and restart the console, since the launcher reads that file when it starts; it shows up among the games. Steps 2 and 3 are the same.

```ini
[ENTRY]
CATEGORY=Games
NAME=Ship of Harkinian
COMMAND=cd /home/player/apps/ShipOfHarkinian && sh soh.sh
ICON=/home/player/apps/ShipOfHarkinian/icon.png

[ENTRY]
CATEGORY=Games
NAME=2 Ship 2 Harkinian
COMMAND=cd /home/player/apps/2Ship2Harkinian && sh 2ship.sh
ICON=/home/player/apps/2Ship2Harkinian/icon.png
```

SELECT opens the port's menu, with all of its settings: the D-pad moves, A picks, B goes back and SELECT closes it; the game takes no buttons while it is open. SELECT+START still closes the game. Aiming in first person is inverted, as on the N64: Settings > Controls > Invert Aiming Y Axis in Ship of Harkinian, Enhancements > Camera > Invert Y Axis in 2 Ship 2 Harkinian.

Saves, settings and the assets made from your ROM stay in `HOME/.config/soh` and `HOME/.config/2ship`, apart from the apps: a newer zip updates a port the same way, and uninstalling one keeps them. A port installed by hand before (`HOME/ports/soh`, `HOME/ports/2ship`) hands its assets, settings and saves to the app on its first start, without the ROM. So far it has been tested on one console.

Both are HarbourMasters' ports with this repository's patches: [Ship of Harkinian](https://github.com/HarbourMasters/Shipwright) 9.3.0 and [2 Ship 2 Harkinian](https://github.com/HarbourMasters/2ship2harkinian) 5.0.1, which is CC0. Ship of Harkinian has no license file: its code is theirs, and this build is offered as a port of their work, to be taken down if they ask. Get the official Ship of Harkinian from their repository.

How it works, how to build it, and the credits: [README](https://github.com/alvesmaicon/glOSports-harbourmasters#readme).
