# NOTICE
Carefully read this README before proceeding, Whatever happens to you OR your laptop is NOT my responsibility and it is your own. do NOT use a DSDT from other laptop models or even the same model of different BIOS. If you do you would get an ACPI error in BSOD which can be easily fixed by selecting Windows in boot menu to avoid clover and delete the dsdt.aml.

You will see some models having unknown BIOS because it hasn’t been reported to me yet. If I got those BIOS version, I’ll update it ASAP.

# About DSDT

DSDT (Differentiated System Description Table) is a part of the ACPI specification. It supplies information about supported power events in a given system. ACPI tables are provided in firmware from the manufacturer.

This repo is still work in progress, meaning it will be updated periodically to add new laptop models or remove some files which are obsolete, or even giving issues. 

# HOW TO 

1. Install Clover Bootloader https://www.youtube.com/watch?v=qhSciG2SKu4

2. Paste the downloaded dsdt.aml file to `\EFI\CLOVER\ACPI\WINDOWS\`. If you dont see Windows folder, create it and paste inside the folder. Reboot to Clover and then to Windows to load the dsdt.aml EVERYTIME

The purpose of the Github is to provide different edited/patched dsdts for a hassle-free experience to just downlaod-paste-boot-enjoy  

EDIT DSDT.AML ON YOUR OWN
Report Your issues in our discord server if you can or in the github itself if you know how to do that.. if not communicate with me/us through our glorious discord server [here](https://discord.gg/qEAfkuA)

Some dsdt.aml files are decompiled to dsl and errors are fixed so people can edit the dsl and compile to aml as shown in [video here](https://www.youtube.com/watch?v=Oerq0w140EI) so you will see "fixed dsdt dsl" files .. ignore if you are just here for aml

What we are doing is we edit the ACPI Tables(dsdt) to give us the STAPM limit or TDP limit or even Temperature limit we want. and inject the patched dsdt with CLOVER BOOTLOADER on every boot. so if you reboot and go directly into windows you will see only default values and no edited values. for the patched dsdt to load in windows you have to first boot into Clover Bootloader and then to Windows

[Tutorial For STAPM/TDP](https://www.youtube.com/watch?v=Jre0QfLdJ5A)
[Tutorial For Temperature](https://www.youtube.com/watch?v=w_vV_xpwiho)

Text tutorial to edit your own values into your dsdt can be found [here](https://pastebin.com/3wB2k7Ei) first 3 lines would be understood when you see the video combined

the DSDT files are generally at Compiled format in .aml files which we can't edit without DECOMPILING them to .dsl which makes it easier to edit even with a notepad or some other text editor but recommended dsdt editor is linked in the video description.

After editing and compiling the EDITED/PATCHED dsdt.aml, paste as mentioned in the text tutorial or video and boot into clover then to windows from there and voila.

This is a work in progress. if you have any doubts/errors/ideas feel free to do contact us in the [Discord server](https://discord.gg/qEAfkuA)
