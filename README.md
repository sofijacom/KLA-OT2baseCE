# KLA-OT2baseCE

![2023-08-21_750x422-thumb](https://github.com/sofijacom/KLA-OT2baseCE/assets/107557749/45ea5dae-f396-438b-a08f-12ad56edceb2)

# Assembly of KLA-OT2baseCE

1) Create a folder `KLA-OT2baseCE` typing in the terminal `mkdir -p KLA-OT2baseCE`

2) Open a terminal in the created folder `KLA-OT2baseCE` or go to the folder by typing in the terminal

   - `cd KLA-OT2baseCE`

3) Place the build script  `KLbuild_Arch_Openbox_KLA-OT2baseCE.sh` in the created folder.
   
4) Make it executable.`chmod +x KLbuild_Arch_Openbox_KLA-OT2baseCE.sh`

5) Enter in terminal `./KLbuild_Arch_Openbox_KLA-OT2baseCE.sh`

6) Wait for the build to finish.

7) After the build is complete to package `07firstrib_rootfs` into `07KLA-OT2baseCE-x.x.sfs` where x.x is your build number.

8) Type in terminal.

```
mksquashfs 07firstrib_rootfs 07KLA-OT2baseCE-x.x.sfs -noappend -comp xz -b 512k
```
  - where x.x is your build number.

9) Delete the `07firstrib_rootfs` folder.

##

FirstRib-KLA build script. 

```
./KLbuild_Arch_Openbox_KLA-OT2baseCE.sh
```
FirstRib-KLA build script PLUG file.

Example of using a .plug file:

```
./build_firstrib_rootfs.sh arch default amd64 f_00_Arch_amd64-openboxBASE_jgmenu_600r5.plug
```

***f_00_Arch_amd64-openboxBASE_jgmenu_600r5.plug***  builds a  ***(root filesystem)***  for the Arch Linux-based Openbox desktop operating system, similar to **KLA-OT2baseCE**.

To create a complete distribution, all other utilities, tools and configurations are downloaded from a centralized repository and installed as a .tar.gz file.
