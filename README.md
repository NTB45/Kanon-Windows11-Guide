# Kanon-Windows11-Guide
A guide on how to run kanon on windows 11 with the voicepatch

## Why am i doing this

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

then run ubuntu
update it with 
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
