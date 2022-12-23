# ps_ram

ps_ram_log - creats ps,top,free output logs
<br>ps_ram     - parsing ps logs for finding RAM diff  

EXAMPLE
./ps_ram 2022-12-15/23/34_ps 2022-12-15/23/35_ps 


processes only in FILE 1: 2022-12-15/23/34_ps
                 MEM   PRIV_MEM SHARED_MEM        PID        COM
                 1.3      236.0        1.1      99999       arpa
               366.5      344.0       22.5      76220       grep
               549.5      448.0      101.5      76213       bash
count processes: 3
MEM sum for all processes: 917.3


processes only in FILE 2: 2022-12-15/23/35_ps
                 MEM   PRIV_MEM SHARED_MEM        PID        COM
               368.5      348.0       20.5      76268       grep
               555.5      452.0      103.5      76261       bash
count processes: 2
MEM sum for all processes: 924.0


DIFF MEM between the files. MEM file 2022-12-15/23/34_ps - MEM file 2022-12-15/23/35_ps by process
 DIFF: MEM   PRIV_MEM SHARED_MEM        PID COMMAND
      -1.0          0       -1.0        696 chronyd
      -1.0          0       -1.0       3708 gnome-session-ctl
      -5.0          0       -5.0        695 chronyd
      -1.0          0       -1.0        554 acpid
     -17.0          0      -17.0       2460 master
      -2.0          0       -2.0       3877 gsd-a11y-settings
      -1.0          0       -1.0       3864 ibus-portal
      -1.0          0       -1.0       3710 indicator-bluetooth-service
      -1.0          0       -1.0       7112 xdg-permission-store
      -1.0          0       -1.0       3856 ibus-memconf
      -1.0          0       -1.0       3796 at-spi-bus-launcher
      -1.0          0       -1.0        572 irqbalance
      -1.0          0       -1.0       3532 gvfs-goa-volume-monitor
      -1.0          0       -1.0       3954 ibus-engine-simple
      -1.0          0       -1.0       3893 gsd-usb-protection
      -1.0          0       -1.0       3651 VBoxClient
      -2.0          0       -2.0        594 switcheroo-control
      -5.0       -4.0       -1.0      16222 gvfsd-metadata
      -1.0          0       -1.0       2682 VBoxClient

