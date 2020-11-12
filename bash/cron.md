#-#
#-# Job Scheduling
#-#

#-# Crontab command

Command                                    Description
-------                                    -----------
crontab -e <file>                          Edit a crontab, or create it if it doesn’t exist.
crontab -u <user> -e <file>                Edit a crontab as the specified user.
crontab -l <file>                          Display crontab on standard output.
crontab -r <file>                          Remove crontab.
crontab -v <file>                          Display the last time the crontab was edited.


#-# Syntax

* * * * * <command-to-be-executed>
│ │ │ │ │
│ │ │ │ └─ day of the week (0-6) (sunday = 0)
│ │ │ └─ month (1-12)
│ │ └─ day of month (1 - 31)
│ └─ hour (0 - 23)
└─ min (0-59)


#-# Special characters

Character             Example              Description
---------             -------              -----------
*                     *                    Specify any occurrence of the field.
,                     0,15                 Specify 2 or more times of execution.
-                     0-59                 Specify any time within a range.
/                     */15                 Can be used with a range or wild card to run at a specified interval.


#-# Examples

Crontab                                    Description
-------                                    -----------
* * * * *             <command>            Every minute of every day.
*/15 * * * *          <command>            Every 15 minutes of every day.
03-59/5 02 * * *      <command>            Every 5 minutes of the 2 am hour starting at 2:03.
0 * * * *             <command>            Every day at midnight.
0 */12 * * *          <command>            Twice a day.
02 * * * 1-5          <command>            Every weekday at 2 am.
02 * * * 6,7          <command>            Weekends at 2 am.
0 02 15 * *           <command>            Once a month on the 15th at 2 am.
0 02 */2 * *          <command>            Every 2 days at 2 am.
0 02 1 */2 *          <command>            Every 2 months at 2 am on the 1st.


[reference](https://github.com/vrachieru/cheatsheet)
