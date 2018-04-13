# ps

Show memory and pid for every program run by user fhsu

    ps -u fhsu -o rss,etime,pid,command
    
RSS stands for Resident Set Size and indicates how much memory in RAM is being allocated to a process. [See this for details](https://stackoverflow.com/questions/7880784/what-is-rss-and-vsz-in-linux-memory-management).
