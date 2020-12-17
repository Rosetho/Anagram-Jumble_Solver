# Anagram-Jumble Solver
It is a fun brain exercise to take a group of scrambled letters and rearrange them into a word.

Example:

loehl = hello

prcmoae = compare

uoehs = house

It is intriguing to think how the brain can solve these puzzles. For a computer, hashing seems like the most efficient way to retrieve the solution in seconds. 

The class 'CreateHashMap' takes each word of an English dictionary  and sorts its characters to use as the Key in the map. A list is created to store the untouched word as the Value. Words with duplicate hashes are simply added to the list. This may be done once, as the values are stored in the file 'hashmap' which is read by the next class.
'Anagram' takes an arguement of jumbled letters and sorts the letters to query the mathcing words. When run by itself, it returns the solution very quickly. 

I've seen many functions that compare two words and return their status as an anagram. The common solution for this method is to simply sort the words and diretly compare. I used this as the basis for my Anagram algorithm that takes it one step further. There are several websites that offer this type of service for games like scrabble, but do not have details on their algorithm. This was a fun little project that turned out to have a simple solution with less than 100 lines of code.

:) 

   
