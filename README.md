# Kanon-Windows11-Guide
A guide on how to run kanon on windows 11 with the voicepatch

## Why am i doing this

becuase no one else has done it and properly(this guide is definately not proper) documented it

Hey All, KuudereEnthusiast here

And your know what i hate the most
An operating system whose strong points are compatibility, but fails at it

After wanting to play kanon for like ages 
I finally decided to download it and install all the patches, English translation, voice over and stuff

English translation worked great

But the voice over, it didn't

So naturally I got to work trying to fix it.
After a few google searches and archived reddit posts later

I found that Kanon has doesn't work with windows 11 and the voiceover's provided w11.exe that is working, doesn't have the voiceover. Ironic

So
Like a maniac
I loaded up Ubuntu dual boot and tried to run the game on wine

It worked
well, looks like windows got beat by a translation layer.

So now, like a wreckless manic, i ran the game from bottles installed in wsl in windows 11

it worked


but it was laggy as FqUaCK.

i remembered that rlvm exists for real live visual novels

i installed that from the repo.


works perfectly

So
time for TLDR and commands

# TLDR

## here are the instructions on how to enable WSL in Windows 11 and install rlvm:
 Open the Start menu and type "Windows features".
Click on "Turn Windows features on or off".
Check the "Windows Subsystem for Linux" checkbox and press the "OK" button.
Restart your computer.

## Installing Ubuntu

Once WSL is enabled, you can install Ubuntu from the Microsoft Store.

I recommend the ubuntu 22.xx LTS 

but any distro should work if you know your stuff

(i used ubuntu stable for this guide)

then run ubuntu, update it with 

        sudo apt update

then

        sudo apt upgrade


## then install the ubuntu universe repo 
        sudo add-apt-repository universe

then install rlvm

        sudo apt install rlvm

then run rlvm by typing 

        rlvm

then pick your kanon files from there

then boom

thats kanon for ya



And now if for some reason it doesnt work
you can try installing flatpak on wsl
then install bottles and run the game exe through it

I'll put the rough instructions i made for installing it from wine and bottles in wsl, but its incomplete and i lazily made it go through an ai chatbot to do make it human readable

I would only recommend to follow that when in serious issues
RLVM should be prefered 99% of the time

# How to Play Kanon on Windows 11 with Wine and Bottles
## Warning, AI assisted stub below here, not 100% accurate, will only recommend people that know their shit try it.

## Instructions

Enable WSL on Windows 11.
Install Ubuntu 22.xx LTS on WSL.
Open a terminal in Ubuntu and run the following commands:

        sudo apt update

        sudo apt upgrade

        sudo apt install flatpak

        flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo

        flatpak install flathub com.usebottles.bottles


Once Flatpak and Bottles are installed, restart the pc,( or the explorer.exe if you feel adventurous )
and open bottles(ubuntu from the start menu)
    
Let the bottles setup do its job

then

Make a bottle

The challenging part might come when you open Ubuntu in File Explorer. It's probably docked on the left tree of Explorer.

Go to Ubuntu in File Explorer.
Navigate to         Ubuntu\home\user\.var\app\com.usebottles.bottles\data\bottles\bottles\bottlename\drive_c\Program Files
    Paste the Kanon folder there. (Bottles has this Flatpak containerization limitation.)

Add a shortcut

Go to Bottles and click Add shortcut.
Go the long way to the Kanon folder in Linux again.
Add the reallive.exe file.
Cross your fingers and run that .exe from the shortcut menu.

Congratulations!

If it runs with audio, you're good to go!
Click the Add shortcut button and select the reallive.exe file from the Kanon installation directory.
Run the shortcut.

Troubleshooting

    If you get a DirectSound with a bunch of bogus text error, restart your computer.
    If the game audio gets choppier over time, restart your computer.

Conclusion

This guide has shown you how to install Bottles from Flatpak and play Kanon on Windows 11. With these tools, you can play Kanon and other Windows applications on your Windows 11 system.

I hope you enjoy playing Kanon!
