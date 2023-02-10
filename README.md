# perf_log

perf_log               - creat and log output of top,ps,pmstat,vmstat and free
<br>ps_ram             - parsing ps_mem logs for finding RAM diff  
<br>ps_ram_classic     - parsing ps logs for finding RAM diff  

EXAMPLE:<br>

![alt text](https://raw.githubusercontent.com/ruslansvs2/ps_ram/main/doc/ps_mem_output.JPG)
<br>
example:
perf_log/2023-02-10/13# ls -sl
total 69
 1 -rwxrwx--- 1 root vboxsf   204 Feb 10 13:28 28_free
 4 -rwxrwx--- 1 root vboxsf   646 Feb 10 13:28 28_mpstat
 4 -rwxrwx--- 1 root vboxsf  2991 Feb 10 13:28 28_ps
36 -rwxrwx--- 1 root vboxsf 35774 Feb 10 13:28 28_ps_classic
24 -rwxrwx--- 1 root vboxsf 22228 Feb 10 13:28 28_top
 1 -rwxrwx--- 1 root vboxsf   244 Feb 10 13:28 28_vmstat

