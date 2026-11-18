Ocarina of Time (Ship of Harkinian) and Majora's Mask (2 Ship 2 Harkinian) for goodluckOS, as apps for the App Installer. The zips are the ports only, with nothing of the games in them: each one plays your own ROM.

**You need** a GA36-MB with a goodluckOS that has the App Installer (System Settings > System > App Installer) and your ROM: for Ocarina of Time a version Ship of Harkinian takes (N64 1.0 to 1.2 or PAL, GameCube or Master Quest), for Majora's Mask the N64 USA version (1.0) or the GameCube USA one.

1. Copy `ShipOfHarkinian-*.zip` and/or `2Ship2Harkinian-*.zip` to the `apps` folder of the console's HOME (over USB, where the console shows up as a drive, or with the card in a card reader) and install them in the App Installer. They show up in the Games tab.
2. Copy your ROM to HOME, as a `.z64`, `.n64` or `.v64` file or a zip of one.
3. Open the game. The first time, it finds your ROM and makes its assets from it, in a window that shows how far it has got; then the game starts, and from then on it starts straight away.

SELECT opens the port's menu, with all of its settings: the D-pad moves, A picks, B goes back and SELECT closes it; the game takes no buttons while it is open. SELECT+START still closes the game. Aiming in first person is inverted, as on the N64: Settings > Controls > Invert Aiming Y Axis in Ocarina of Time, Enhancements > Camera > Invert Y Axis in Majora's Mask.

Saves, settings and the assets made from your ROM stay in `HOME/.config/soh` and `HOME/.config/2ship`, apart from the apps: a newer zip updates a port the same way, and uninstalling one keeps them. A port installed by hand before (`HOME/ports/soh`, `HOME/ports/2ship`) hands its assets, settings and saves to the app on its first start, without the ROM. So far it has been tested on one console.

Ocarina of Time is built from HarbourMasters' [Ship of Harkinian](https://github.com/HarbourMasters/Shipwright) 9.3.0 with this repository's patches. Ship of Harkinian has no license file: its code is theirs, and this build is offered as a port of their work, to be taken down if they ask. Get the official Ship of Harkinian from their repository. Majora's Mask is built from [2 Ship 2 Harkinian](https://github.com/HarbourMasters/2ship2harkinian) 5.0.1, which is CC0.

How it works, how to build it, and the credits: [README](https://github.com/alvesmaicon/glOSports-harbourmasters#readme).
