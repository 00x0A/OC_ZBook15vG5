# Hackintosh HP ZBook 15vG5 (OpenCore)

Disclaimer: You do this at your own risk, I will not be held responsible for any issues during this process. If you have some issues open an issue and I will take a look at it.

Everything I’ve tired works out of the box except for airdrop functionality as it’s not natively supported with the built in wifi card.

For sdcard functionality + thunderbolt functionality enable IOElectrify and Sinetek-rtsx, I haven’t tested those as I don’t use those functions.

Edit itlwm.kext > info.plist to use your specific wifi(s)

Generate USBMap specific to your laptop or use the premade one. Should some USB port not work you’ll need to map it yourself.

Sleep works fine but needs around 30 seconds to initiate.

Turbo boost has been disabled by the kext “DisableTurboBoostBattery” as my laptop have thermal and battery problems, even with a newly installed replacement battery.

If you plan to dual boot Linux you’ll need appropriate drivers, dual booting Windows was not tested but should work out of the box.

Opencore will work best with a better compatible SSD, the default Samsung one on the laptop will have its own issues from what I’ve read.

Lastly, GENERATE YOUR OWN SMBIOS, this is to make sure you’re not using anyone else’s SMBIOS or the default one which might get your Apple account terminated!

Big thanks to Corpnewt for helping with this install and route66 for their setup of OpenCore which I took inspiration from.
