--RPG-Terminal--
A terminal utility for rolling dice.

--How To Use--
When initiating the script, the following switches can be used to input data. If no switches are used, then an interactive menu is started requesting the necessary information.

Things that work right now
 -Prompt requesting the number and size of dice to roll, and displaying the result of that roll. Displays if no working switches are used

Things that will be working later
 -logging and easy display of log
 -switch -d or --dice
   input number and type of dice to roll in NdD format, such as RPG-Terminal -d 2d6 to roll two six-sided dice
 -switch -c or --comment
   input a comment about the roll being made, which will be tied to it in the log
 -switch --bestof 
   only the die rolled with the highest result should be displayed
 -switch --worstof 
   only the die rolled with the lowest result should be displayed
 -switch --displayall
   do not sum rolled dice and instead display the result of each die