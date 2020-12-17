# Anagram-Jumble Solver
It is a fun brain exercise to take a group of scrambled letters and attmept to rearrange them into a word.<br>

Examples:<br>
loehl = hello<br>
prcmoae = compare<br>
uoehs = house<br>

It is intriguing to think how the brain can solve these puzzles. For a computer, hashing seems like the most efficient way to retrieve the solution in seconds. 

The class 'CreateHashMap' takes each word of an English dictionary and sorts its characters to use as the Key in the map. A list is created to store the untouched word as the Value. Words with duplicate hashes are simply added to the list. This may be done once, as the values are stored in the file 'hashmap' which is read by the next class.

KEY: ehllo -> VAL: [hello]<br>
KEY: adel  -> VAL: [lead,deal,...]<br>

'Anagram' takes an arguement of jumbled letters and sorts the letters to query the mathcing words in the hash map. When run by itself, it returns the solution very quickly. 

I've seen many functions that compare two words and return their status as an anagram. The common solution for this method is to simply sort the words and directly compare. I used this as the basis for my Anagram algorithm which takes the concept one step further. There are several websites that offer this type of service for games like scrabble, but do not have details on their algorithm. This was a fun little project that turned out to have a simple solution with roughly 50 lines of code.<br>:)<br>

To run on the command line:<br>
javac CreateHashMap.java<br>
touch hashmap
java CreateHashMap > hashmap
javac Anagram.java
java Anagram <i>jumbledWord,</i>

   
