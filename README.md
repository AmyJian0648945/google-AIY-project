Setting up the raspberry pi
===========================

    * SSH to the raspberry pi to connect to the wifi:
        - Get the SD card of the rpi, and create the following files
            Empty file ".ssh"
            "wpa_supplicant.conf" (with usrname/pwd)
        - Once you can ssh to rpi (get IP from router), do:
            `sudo raspi-config` to enable ssh and vncserver, basic config
            Suggestion: change hostname so you don't clash with other rpi
    * Setup packages:
        `sudo apt update && sudo apt upgrade && sudo apt-get update`
        `sudo apt-get install tmux`
    * Camera streaming will not work on vnc (needs to be directly connected).
