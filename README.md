# HomeAutomation
My home automation files

These are for my dual zone climate control. I have two Ecobee thermostats and sometimes where I live it gets hot enough that my A/C barely keeps up with the main floor. 
In here are 4 yaml automations and two toggle entities. 

One entity is to set which thermostate is the priority thermostat. The other is a toggle switch for when we have extra hot days.

Delayed start:
  This file delays the stopping the nonpriority zone if the non priority is cooling. This allows for the cooling zone to switch to the priority and then after two minutes it will shut off the nonpriority.

Priority Thermostat continues cooling:
  This file is for when the priority zone is cooling and the nonpriority wants to cool. It will turn the nonpriority to off until the priority reaches its cooling setpoint.

8 pm switch:
  The normally non priority zone is my son's bedroom so at 8 pm we switch it over so that it can cool down up there so he can sleep.

Hot day cooling routine:
  This checks everyday at 5 am if the hot day routine is toggled on. if it is, it cools the mainfloor down, then the bedroom and then turns off cooling for the upstairs. This needs to be configured a little better.
