# PHP_Templating
PHP Templating task for WallStreetDocs

Initial design tests were created before coming to the presented solution.
These included deciding upon how to handle the initial XML and then furhter parse through the data.
json_encode() was also implemented early on to give a comparison on the final result.

The final solution made use of switch cases which I have had experience with in other languages and could manipulate comfortably.
This enabled me to handle each data type that may be present within the XML through recursively calling the function. 

Creating the final output was via a foreach loop and appending the necessary data. 
During this, addslashes() was used to handle any characters that may cause issues and santify the input.
implode() would then be finally used to join the elements with comma seperation and then returned within {} parentheses.
