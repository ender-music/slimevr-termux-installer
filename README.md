# The official docs are more up to date; please follow them.

Follow https://docs.slimevr.dev/tools/termux-installation.html

# slimevr-termux-installer

This is the home of the installer and launcher for the SlimeVR server with Termux.

Credit goes to Butterscotch! for making this work, I just made an installer.

# INSTALLATION - QUEST 2

1. Download Termux (quest 1/2 is arm64) from here: https://github.com/termux/termux-app/releases

2. Install the .APK file using either Sidequest, ADB, or an already installed file explorer.

3. Open Termux, and run the following command:

```
bash <(curl https://raw.githubusercontent.com/SlimeVR/SlimeVR-Termux-Installer/main/install.sh)
```

4. Go to https://slimevr-gui.bscotch.ca/ on the device with the server if it doesn't auto open.

## If you want to start the server again after closing, DO NOT run the setup commands again. Run:

```
./start.sh
```

# INSTALLATION - ANDROID PHONES

1. Enable developer mode on your phone. You can do this by opening settings, going to about phone, and finding the "Build Number" and tapping it seven times.

2. Download Termux (most phones are arm64, you can google what yours is) from here: https://github.com/termux/termux-app/releases
   **DO NOT INSTALL FROM GOOGLE PLAY.**

3. Click the APK, and allow it to be installed.

4. Open Termux, and run the following command:

```
bash <(curl https://raw.githubusercontent.com/SlimeVR/SlimeVR-Termux-Installer/main/install.sh)
```

5. Go to [https://slimevr-gui.bscotch.ca/](https://slimevr-gui.bscotch.ca/) on the device with the server if it doesn't auto open.

## If you want to start the server again after closing, DO NOT run the setup commands again. Run:

```
./start.sh
```

# Updating

On both Android and Quest, to update, all you need to do is start it, it automatically checks for update.

# Remote GUI Access

The first step is enabling this on whatever browser you use: https://www.damirscorner.com/blog/posts/20210528-AllowingInsecureWebsocketConnections.html
Enable it for https://slimevr-gui.bscotch.ca/
Now that you have done this, you can go to `https://slimevr-gui.bscotch.ca/?ip=[QUEST OR PHONE IP]&port=21110` and access the site. Substitute `[QUEST OR PHONE IP]` with your Quest's or phone's IP address, without the brackets.

Credit goes to Butterscotch!#2066 for making all of this work and Bagel#6705 for the documentation, idea, and motivation.
