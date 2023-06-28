# VIRTUAL BOX CONFIGURATION (UBUNTU)

**We are creating a virtual Machine for Ubuntu Desktop**
---

***Note : Desktop and Server are two diffrent types of VM's***

---

    Step 1 : Open your Oracle virtual Box Wizard

    Step 2 : Click on "New" on the top of the screen for creating a new VM

    Step 3 : A Pop-up will open, add Name for your VM eg: Ubuntu-Desktop
             In Folder input let the default path be set and don;t change the path of VM
             In Type Select Linux
             In Version You can select Ubuntu 64 BIT

    Step 4 : Click on Next and a Memory size Panel will pop up
    Step 5 : Allocate 4096 MB RAM and click next
    Step 6 : Hard disk Panel will open. Choose create a virtual hard disk now option and click Create
    Step 7 : Now Hard disk file type panel will open. Here choose VDI(VirtualBox Disk Image) and click Next 
    Step 8 : Now Storage on physical hard disk will panel will pop up choose dynamically Allocated anc click Next 
    Step 9 : In File location and size add 20.00 GB space to Virtual hard disk size
    Step 10 : Now you have created a Ubuntu Desktop VM !!!!

---

**Configuring The Desktop VM**
---

Right click on the Created VM and click on settings.

>> System settings

    * MotherBorad Panel 
    -------------------------
    > In boot order Optical at first , then harddisk and after that Floopy
    > In Pointing Device choose : USB Multi-Touch Tablet 
    
    * Processor Panel
    -------------------------
    > In Processors Choose 2 CPU

>> Display settings

    * Screen Panel
    -------------------------
    > Add 128 MB to Video Memory 

>> Storage setting 

    > In Controller: IDE click on the small disk icon and choose/create a Virtual optical Disk.
    > In the panel click on add and choose your Ubuntu Disk image file in your PC
    >Now you have set Optical drive ckick ok and done


>> Network setting

    > Let Adapter 1 be NAT
    > click on Adapter 2 and click on enable Network adapter
    > Choose Bridged Network and done click on ok.

> Click On Sart to start.

---
END OF UBUNTU DESKTOP INSTALLATION

---

**We are creating a virtual Machine for Ubuntu Server**
---

***Note : Desktop and Server are two diffrent types of VM's***

---

    Step 1 : Open your Oracle virtual Box Wizard

    Step 2 : Click on "New" on the top of the screen for creating a new VM

    Step 3 : A Pop-up will open, add Name for your VM eg: Ubuntu-Desktop
             In Folder input let the default path be set and don;t change the path of VM
             In Type Select Linux
             In Version You can select Ubuntu 64 BIT

    Step 4 : Click on Next and a Memory size Panel will pop up
    Step 5 : Allocate 2096 MB RAM and click next
    Step 6 : Hard disk Panel will open. Choose create a virtual hard disk now option and click Create
    Step 7 : Now Hard disk file type panel will open. Here choose VDI(VirtualBox Disk Image) and click Next 
    Step 8 : Now Storage on physical hard disk will panel will pop up choose dynamically Allocated anc click Next 
    Step 9 : In File location and size add 15.00 GB space to Virtual hard disk size
    Step 10 : Now you have created a Ubuntu Desktop VM !!!!

---

**Configuring The Server VM**
---

Right click on the Created VM and click on settings.

>> System settings

    * MotherBorad Panel 
    -------------------------
    > In boot order Optical at first , then harddisk and after that Floopy
    > In Pointing Device choose : USB Multi-Touch Tablet 
    
    * Processor Panel
    -------------------------
    > In Processors Choose 2 CPU

>> Display settings

    * Screen Panel
    -------------------------
    > Add 128 MB to Video Memory 

>> Storage setting 

    > In Controller: IDE click on the small disk icon and choose/create a Virtual optical Disk.
    > In the panel click on add and choose your Ubuntu Disk image file (SERVER )in your PC
    >Now you have set Optical drive ckick ok and done


>> Network setting

    > Let Adapter 1 be NAT
    > click on Adapter 2 and click on enable Network adapter
    > Choose Bridged Network and done click on ok.

> Click On Sart to start.