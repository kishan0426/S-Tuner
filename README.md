# S-Tuner
A shell script to tune the sql by pinning the best plan available for a sql from AWR 
Often, there is a complaint from client regarding performance issue on a specific SQL. 
Optimizer dynamically change the plan unexpectedly. 
It is hard to predict the change of an execution plan for some reason. 
It can be a bug or expected behavior or due to physical design changes or lack of statistics or adaptive settings etc.. 
Even real time tool cannot easily report the run time execution plan in a poorly performing database proactively. 
This script does not proactively accomplish anything but will check for changes in the plan and pin the best plan available. 
Note: AWR license is required to use this script. 

Note: coe_xfr_* scripts are needed for this script to work. Please download the scripts and stage it in script directory before use.
