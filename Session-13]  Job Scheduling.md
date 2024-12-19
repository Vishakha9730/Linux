# Job Scheduling in Linux-
- Job scheduling is a feature that allows a user to submit a command or program for execution at a specified time in the future.
-  On a Linux server, it is important that certain tasks run at certain times the execution of the command or program could be one time or periodically based on a pre-determined time.

# 'at' command-
- The at command in Linux is used for scheduling one-time tasks to be executed at a specified time.
- Users can submit commands or scripts, and the atd daemon manages the execution of these scheduled jobs.
- The scheduled jobs are managed by the atd (at daemon) service, which runs in the background and executes the queued tasks at the specified times.
#### Syntax-
-  at “time date” (Only provide Hrs and min)
      -  Press Ctl+D to save and quit the job. 
- atq- Lists jobs
- atrm- Remove jobs

# 'cron' command-
- Cron command is used to schedule repetative task.
- Crontab job scheduling technique is very useful for creating backup, scanning system, performing jobs with daily, weekly, monthly basis, etc.
-  A daemon called crond runs in the background and check its configuration every minute to examine configuration files in order to execute commands or shell scripts specified in the crontab if the
  time matches with specified time.
- Crontab can executes job repeatedly in specified time interval.

  ![image](https://github.com/vishakhadhonde9/Linux-Second-half-/assets/97825776/3df2b18c-f69d-4227-9b32-b24ac444b5bb)

#### Syntax-
- crontab <option>
##### Options-
- -e Edit/Create cron table
- -l List cron table
- -r Remove crontable
  
