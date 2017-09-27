--RPG-Terminal--
A terminal utility for rolling dice.

--How To Use--
 -When script runs, a prompt requesting the number of dice to roll will display. Enter the number and size of dice as NdD. For example, if rolling 3 six-sided dice, enter 3d6. If rolling 2 eight-sided dice, enter 2d8. If rolling 1 100-side die, enter 1d100. Entering any text not in NdD format will exit the script.

-- Things that work right now--
 -Prompt requesting the number and size of dice to roll, and displaying the result of that roll. Displays if no working switches are used (and no switches work yet, so it will display).
 -Displays the results of all dice rolled as well as a sum of each die.

--Things that will be working later--
   (Not in order of priority)
 -logging and easy display of log
	-switch -h or --history for displaying the log of previous rolls to terminal. Providing no input will default to the last ten entries. Specifying a number will provide that number of entries upward from end of the log file. Specifying a date will provide all entries from that date. Specifying two dates and times will provide entries between those dates and times.
	-switch -l or --logfile to specify log file to use. If not used, a default log-file will be generated as RPG-Logfile-YYYY-MM-DD-HH-MM.log
 -switch -d or --dice
	Input number and type of dice to roll in NdD format, such as RPG-Terminal -d 2d6 to roll two six-sided dice.
 -switch -c or --comment
	Input a comment about the roll being made, which will be tied to it in the log. Prompt for comment will also be added to the interactive method.
 -switch --bestof 
	The die roll with the highest value will be presented instead of the sum of all dice results.
 -switch --worstof 
	The die roll with the lowest value will be presented instead of the sum of all dice results.
 -switch --resultonly
	By default, the result of each die roll is displayed and then the end result is displayed. This switch will indicate only the end result.
 -RPG Specific options
	As an example --adv and --disadv will be added switches to allow for 5th edition style rolling of 2d20s, and indicating the higher or lower roll, respectively
	Other examples are fudge dice for FATE, special dice for the FFG SW RPG system, and exploding dice for various systems, and percentile die using a d10 labeled 0-10 and another labeled 10-100.
	Also will add an option to count number of specific results, eg, count all results of 6 on a roll of 10d6.
 -Conversion to Python 3
	This will allow for more correct rolls using more cryptographically secure options available in Py3.
 -Looping
	If using interactive method, once results are presented, user is presented with option to roll additional dice or quit the program.
 -History view from interactive method
	Using the interactive method, have menu for accessing the history using same functions defined above for the -h or --history switch.