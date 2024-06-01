# Voron 2 Tall

<!-- <div align="center">
  <img src="./images/placeholder.JPEG" width="500px">
</div> -->

Collection of files for building custom Voron 2.4 with a build volume of 350 mm
x 350 mm x 930 mm (13.78 in x 13.78 in x 36.61 in) modified from the base LDO
Voron 2.4 Kit. 

## Mods
- [Cable Port Flush Mount Skirt](https://mods.vorondesign.com/details/3vEc5I965u0puzAmz9DqvA) - [ppak10](https://github.com/ppak10)
- [Enclosed Z-Chain Guide](https://mods.vorondesign.com/details/4mSRcdfNCvSq6nsRHETw) - [ppak10](https://github.com/ppak10)
- [Nevermore Micro](https://github.com/nevermore3d/Nevermore_Micro) - [nevermore3d](https://github.com/nevermore3d)
- [Purge Bucket](https://github.com/VoronDesign/VoronUsers/tree/main/orphaned_mods/edwardyeeks/Decontaminator_Purge_Bucket_%26_Nozzle_Scrubber) - [edwardyeeks](https://github.com/edwardyeeks)
- Umbilical Mount (Choose One) 
  - [Rear Umbilical](https://mods.vorondesign.com/details/ho9WEyf6msbGKhTbtM59mQ) - [Minsekt](https://github.com/Minsekt)
  - [PG7 Umbilical Mount](https://www.printables.com/model/312008-voron-24-a-drive-pg7-umbilical-mount) - [jphalip](https://www.printables.com/@jphalip)

- [Y Endstop Relocation](https://mods.vorondesign.com/details/ho9WEyf6msbGKhTbtM59mQ) - [Minsekt](https://github.com/Minsekt)

## Canbus Setup

![Canbus Direct Diagram](images/canbus_direct_diagram.PNG)

I mostly followed the steps outlined in this [forum post](https://www.teamfdm.com/forums/topic/672-how-to-use-can-toolhead-boards-connected-directly-to-octopus-octopus-pro-on-canboot/?do=findComment&comment=9911) to connect EBB directly to
Octopus.

More specifically, I followed the guide this guide that was attached.

[**How to Use CAN Toolhead Boards Connected Directly to Octopus / Octopus Pro on CanBoot**](Manuals/Canbus/How%20to%20Use%20CAN%20Toolhead%20Boards%20Connected%20Directly%20to%20Octopus.pdf)

### Notes
1. CanBoot has updated name to Katapult but instructions in manual should still work.
2. If `can0` doesn't automatically show up in `ifconfig` so this command should solve that:
    ```bash
    sudo ip link set up can0 type can bitrate 500000
    ```

### Troubleshooting 
- [CANBus_Query.py not returning EBB36’s UUID. Setup: Pi 4, Octopus v1.1, EBB36 v1.2](https://klipper.discourse.group/t/canbus-query-py-not-returning-ebb36s-uuid-setup-pi-4-octopus-v1-1-ebb36-v1-2/8464)
- [EBB_CAN](https://github.com/EricZimmerman/VoronTools/blob/main/EBB_CAN.md)

## Other Useful Links


### LDO Docs
- [Wiring Guide](https://docs.ldomotors.com/en/voron/voron2/wiring_guide_rev_c)
- [Printed Parts](https://docs.ldomotors.com/en/voron/voron2/printed_part_guide_rev_c)

### Mods
- [Nevermore Micro](https://github.com/nevermore3d/Nevermore_Micro)
- [Rear Umbilical](https://github.com/VoronDesign/VoronUsers/tree/main/printer_mods/Minsekt/Rear_Umbilical)
- [PG7 Umbilical Mount](https://www.printables.com/model/312008-voron-24-a-drive-pg7-umbilical-mount)

### Extruder
<img src="https://www.orbiterprojects.com/wp-content/uploads/2021/11/Orbiter_F2.85-e1636623721217.png" width="250px">

- [Orbiter F2.85 mm Project](https://www.orbiterprojects.com/orbiter-f2-85/)
- [Orbiter F2.85 mm Files](https://www.thingiverse.com/thing:4860182)

### Hotend
- [How To: Successfully Assemble an E3D v6 All-Metal HotEnd](https://www.matterhackers.com/articles/how-to-assemble-an-e3d-v6-all-metal-hotend)
