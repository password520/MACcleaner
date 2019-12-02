# MACcleaner/ghostmac
README:

concept by righttoprivacy@tutanota.com; 

REQUIREMENTS:
bash.
Runs on any Linux distribution. 
Requires the OUI.final file. Make sure it is in same directory or put full path to file.

INSTRUCTIONS:
chmod +x maccleaner
./maccleaner

OR

follow instructions at bottom of this README for how to add a simple button for easy click access.

Why maccleaner?

MAC address tracking is one of the most pervasive/constant forms 
of surveillance abuse out there. Passive sniffers are constantly 
gobbling up our mac address broadcasts, tracking us as we pass 
by them, along with access points. This occurs even if you just have
wifi on. Even if you do not connect. This is a solution with an
anonymous mode to change your mac at constantly changing randomized
times/addresses. To "ghost" your hardware address & drop the trackers.

Even dept stores track your MAC, linking it to your identity/broadcast, as
you bring your items to a cash register. MAC addresses are the permanent 
hardware address tied to your computer WIFI/Ethernet card etc. In fact,
these are one of the biggest ties to your identity/movements. This small 
bash script changes your wifi card to a random MAC address every few minutes at 
random time intervals. 

Drones also collect MAC addresses to track identities, violating 
UN Declaration of Human Rights: #12 is privacy. Privacy is a basic
Human Right.

Why change MAC at random time intervals? Because analysis depends on recognizing 
patterns. If your MAC were to change exactly every 5 minutes one could 
correlate the new MAC address detections every minutes to your identity. 
So this script makes the mac address change at completely random times. 
You can adjust the lowest -> highest time differences in the script variables.

Using random intervals ensures you are not creating a pattern. All tracking
is based on predicable patterns.

Also solves a common issue in mac address changing where MAC address resets to permanent
(original/identity) MAC address upon disconnect from a network/wifi driver
issues. By running this script you shorten the time between mac changes. I ran
KISMET for 6 hours straight to test it. Not a single real MAC address leak. Also
adds many more mac addresses to the mix giving a sort of needle in a haystack 
strategy & constantly moving address.

Works great alongside Parrot OS's AnonSurf/Tor to route traffic, but nothing outside 
this script is required for it to work (outside bash). This script (maccleaner)
changes your device address & KISMET functions well while using it (for ethical
purposes)

-=-=-=-=-=-=-=-=-=--=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-


Add button for maccleaner/ghostmac at top of MATE desktop:

Save the script to a file in text editor (or download from github).

Open terminal.

`chmod +x maccleaner`. 

Move to command path directory:
'mv scriptname /usr/bin' (this puts it in path for command execution)

Rightclick top panel, click "Add To Panel". 

Then "Create Application launcher". 

Select Application and change it to "Application in terminal." 

Command for the launcher: "sudo maccleaner" (or ghostmac, whatever
you name it; also make sure you change from "Application" to 
"Application in Terminal")

Now just clicking the panel button will launch a terminal displaying status
of MAC changes including seconds from last MAC change (in case
you want a status window to keep an eye on MAC address history/timing.

This script was created with ethical intentions to fight predatory MAC address tracking.

If you want to contact/have ideas/questions email: righttoprivacy@tutanota.com


