# perf_log 

create cron job and &#9749;
perf_log               - creat and log output of top,ps,pmstat,vmstat and free
<br>ps_ram             - parsing ps_mem logs for finding RAM diff  
<br>ps_ram_classic     - parsing ps logs for finding RAM diff  

EXAMPLE:<br>

![alt text](https://raw.githubusercontent.com/ruslansvs2/ps_ram/main/doc/ps_mem_output.JPG)
<br>
example:<br>
perf_log/2023-02-10/13# ls -sl<br>
total 69<br>
 1 -rwxrwx--- 1 root vboxsf   204 Feb 10 13:28 28_free<br>
 4 -rwxrwx--- 1 root vboxsf   646 Feb 10 13:28 28_mpstat<br>
 4 -rwxrwx--- 1 root vboxsf  2991 Feb 10 13:28 28_ps<br>
36 -rwxrwx--- 1 root vboxsf 35774 Feb 10 13:28 28_ps_classic<br>
24 -rwxrwx--- 1 root vboxsf 22228 Feb 10 13:28 28_top<br>
 1 -rwxrwx--- 1 root vboxsf   244 Feb 10 13:28 28_vmstat<br>
 
 
<br>
then you can add this script to crontab<br>
example:<br>

\* \* \* \* \*  root /opt/scripts/perf_log <br>

To change the log path please change value of Dir in the perf_log file



