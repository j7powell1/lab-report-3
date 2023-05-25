## Researching Commands
# Four Alternative ways to use the grep command:
# Method one: recursive seraching
***
Using the command $ grep -r "item" directory; we will be able to search for an item recursively in all files within a directory and its subdirectories. 
*Examples:* 
***
Ex:1 
grep -r "medical" techincal
This finds all instances of the word medical in the dircetory techinical.
***
grep -r "research" techincal will find all the words "research" in the technical directory.
***
# Method two: Inverse searching
Using the command $grep -v "item" file; we are able to display all the lines that do not contain our item.

***
# Method three: Case-insensitive search
Using the command $ grep -i "item" file we are able to ignore distinction based on capitals to find any instance of the word we are looking for.
Ex1: grep -i "Medical" technical
***
This will show us all the instances of the word medical even if it is capital or not which in theory should return more than using the normal grep form. 
Ex2: grep-i "oanc"  biomed
***
This will show us all the instances of oanc. This is useful in our case as the word is normall all caps so we are guranteed to find all instances even if at one point the word isn't fully capped.
***
# Method four: finding the line number of searched word
Using the command $ grep -n "item" file; we are able to add line numbers to the output telling us where the item is located. 
***
EX1: grep-n "OANC" biomed;
***
This is useful becuase we can now see the line number that our previuos uses of grep gave us making it easier to find in the doc.
***
CREDIT: I used chatGPT to find the alternate forms of grep as it was mostly online searching. The prompt I gave was "can you 4 interesting command-line options or alternate ways to use the command grep" I for the most part only took the examples it gave me as well as the information to use as genreral understand it, but described it mysdelf.
