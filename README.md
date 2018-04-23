# myGNS3junosOliveAppliance
A "per image" GNS3 QEMU appliance to avoid JunosOlive in VirtualBox. 
I have created it using https://github.com/GNS3/gns3-registry/blob/master/new_appliance.py, setting resources (arch, RAM, vCPU...) as the ones stated in original Virtual Box .OVA appliance... the disk image ("JunOSolive-disk1.vmdk" in my case) comes from the .OVA as well.

Of course this is a highly custom appliance (that's why I called it "per image" in the first sentence): because there isn't a unique, official, standard Junos Olive release, instead many self-created ones; nevertheless it's the proof that the idea works, you can stop setting up Junos Olive in Virtual Box with all the nightmares regarding linked-base and stuff like that (check [my unleashed notes about GNS3](https://github.com/baro77/myGNS3notes) to have an idea.

So:
1 Take notes about resources assigned in Virtual Box to your JunosOlive VM
2 Extract the disk image from your appliance (as easy as copying a file if it's a folderized appliance, otherwise first just rename the appliance file as .zip and uncompress it)
3 Feel free to modify my appliance to fit it to your parameters and image file
4 Have fun using Junos Olive as a QEMU appliance
