Carefully read this README before proceeding, Whatever happens to you OR your laptop is NOT my responsibility and it is your own. do NOT use a dsdt of other Laptop Models or even same model of different bios, well if you do you would get an ACPI error in BSOD which can be easily fixed by selecting windows in boot manager and avoiding clover .. go and delete the dsdt.aml YOU WILL SEE SOME MODELS HAVING UNKNOWN BIOS BECAUSE IT WASNT REPORTED TO ME YET.. IF I GOT THE VERSIONS ILL UPDATE ASAP. 

This repo is still work in progress meaning it will be updated periodically to add new laptop models or remove some files which are obsolete, or even giving issues. 

HOW TO: INSTALL CLOVER BOOTLOADER ON HDD https://www.youtube.com/watch?v=qhSciG2SKu4
paste the downloaded dsdt.aml file to \EFI\CLOVER\ACPI\WINDOWS\  if you dont see windows folder create it and paste. Reboot to clover and then to windows to load the dsdt.aml EVERYTIME

Report Your issues in our discord server if you can or in the github itself if you know how to do that.. if not communicate with me/us through our glorious discord server here https://discord.gg/qEAfkuA

DSDT (Differentiated System Description Table) is a part of the ACPI specification. It supplies information about supported power events in a given system. ACPI tables are provided in firmware from the manufacturer.

What we are doing is we edit the ACPI Tables(dsdt) to give us the STAPM limit or TDP limit or even Temperature limit we want. and inject the patched dsdt with CLOVER BOOTLOADER on every boot. so if you reboot and go directly into windows you will see only default values and no edited values. for the patched dsdt to load in windows you have to first boot into CLOVER BOOTLOADER and then to WINDOWS
Tutorial For STAPM/TDP  https://www.youtube.com/watch?v=Jre0QfLdJ5A
Tutorial For Temperature  https://www.youtube.com/watch?v=w_vV_xpwiho
for text tutorial to edit your own values into your dsdt Can be found here https://pastebin.com/3wB2k7Ei first 3 lines would be understood when you see the video combined

The purpose of the github is to provide different edited/patched dsdts for a hassle free experience to just downlaod-paste-boot-enjoy  

the DSDT files are generally at Compiled format in .aml files which we cant edit without DECOMPILING them to .dsl which makes it easier to edit even with a notepad or some other text editor but recommended dsdt editor is linked in the video description.

After editing and compiling the EDITED/PATCHED dsdt.aml, paste as mentioned in the text tutorial or video and boot into clover then to windows from there and

VOILA

as already mentioned.. this is a work in progress. if you have any doubts/errors/ideas feel free to do contact us in the discord server https://discord.gg/qEAfkuA
