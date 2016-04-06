TwistedProject Github
===================
Build sources for Twisted Rom Shamu and Hammerhead devices

Setting up Build Environment
---------------------------
- Official build environment as per Google and AOSP [Android source page](http://source.android.com/source/index.html)
- XDA user guides [Ubuntu 14.04 Trusty LTS](http://forum.xda-developers.com/showthread.php?t=2639611) , [Ubuntu 14.10 Utopic](http://forum.xda-developers.com/chef-central/android/howto-setup-ubuntu-14-10-utopic-unicorn-t2862442)
- [Arch Linux](https://wiki.archlinux.org/index.php/android#Building_Android)

Initializing the Source
-----------------------
(Assuming you have a valid build environment setup)
- mkdir aosp (or whatever you want to name the source folder)
- cd ~/aosp
- repo init -u https://github.com/TwistedProject/platform_manifest.git -b arm

Sync the Source
---------------
- repo sync -jx -f (x being however many cpu jobs, you can also use -c to sync only the current branch specified by repo init)

Getting Ready to Build
----------------------
- . build/envsetup.sh

Choose Supported Device to Build
--------------------------------
- lunch twisted_hammerhead-user
- lunch twisted_shamu-user

Now Build it
------------
- mka otapackage

For Quick Dirty Rebuilds
------------------------
- cd ~/aosp
- repo sync -jx -f (x being however many cpu jobs, may also use -c as above)
- lunch and pick the right device (refer to above for choosing right device to build)
- mka dirty
- mka otapackage

Credits
-------
- Google for AOSP
- Rascarlo and RastaPop
- Altaf-Mahdi and Euphoria-OS
- DariosF and Purity ROM
- Paranoid Android (AOSPA)
- AOSPAL
- CyanogenMod
- Dirty Unicorns
- LiquidSmooth
- AOKP
- SlimROMS
- Project D.I.S.C.O. Team
- PartimusPrime for bootanimations
- OmniROM
- Lichti1901 and Terminus
- Sykopompos
- Team Horizon and XenonHD
- Chet and OptiPop
- VanirAOSP
- PurifiedROM
- The-Ancile-Project
- AOD-Lollibeans
- Android Open Development
- Dhacker29
- beanstown106
- Ayysir
- BitSyko Development
- Others we may have missed
