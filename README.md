# OSXH4CK

# README 

This repo wont contain any scripts or previews, It will just be a simple guide for how you will be able to take over root access of any Apple Device running MacOSX no matter wich version of OSX. (iMac, Macbook devices etc)

I have created this repository as an reminder for myself. With below commands you will gain 100% full control of all users data and take over root access of any OSX device aslong root partition has not been encrypted.

# HOWTO 

Boot your osx device to Single-User Mode by pressing:

    MacOSX Keyboard:  Command (⌘)—S:
    Windows Keyboard: Windows Button + S
    
### When system have booted, mount root:

    /sbin/mount -wu /
  
### Take over root account by changing root password:

    passwd 
     Enter Password:
     Re-Type Password: 
     Successfully changed root password.
    rm /var/db/.AppleSetupDone
    reboot

When you first start using a brand-new Mac or performed a clean install of OS X, you are presented with Setup Assistant, allowing you to create the first user account and specify some initial information, such as keyboard layout 
and locale. Under certain circumstances, it can be advantageous to re-run the Setup Assistant for take over root account ;) Using some command-line trickery, we can do just this without having to erase and reinstall OS X.

### What Setup Assistant Does
Setup Assistant is designed to run on the first boot of a fresh install of OS X, which is why you'll only see it when booting up a a brand-new Mac or one that has been erased and had OS X reinstalled.

### Change current users password:
     passwd 'username'

After password has been updated you will be able to login as the user from login screen and have full access to the users data, pictures, documents, music etc etc..

If you're smart, asap you have logged in on the user(s) account open all web browsers that is installed and head over to settings and grab all passwords that hopefully is stored (if there is any) and save them in plain-text before 
the owner MIGHT sync the settings and all passwords will be gone. Also before you will run the reboot command from single user mode backup ALL web browser settings to an usb or something in case the owner 
already has synced the data. Usually all such settings is stored in ~/.config/google-chrome and ~/.mozilla etc etc.. 

![Screenshot](https://nr1.nu/archive/images/hqdefault.jpg)

#### REQUIREMENTS

A macosx device

#### CONTACT 

If you have problems, questions, ideas or suggestions please contact
us by posting to wuseman@nr1.nu (NEW MAIL)

#### WEB SITE

Visit our homepage for the latest info and updated tools

https://github.com/wuseman

#### END!

