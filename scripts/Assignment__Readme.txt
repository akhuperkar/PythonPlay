Programmer: Abhijit Khuperkar
Email: akhuperkar@yahoo.com

Notes:
* The enclosed python notebooks (.ipyb files) contain solutions for the four questions namely Q1, Q3, Q4, and Q5
* Recommend opening the solution files in ipython notebook to view the contents appropriately  
* Each python notebook file starts with the question statement followed by the markdown readme text of program description. It also includes links to the online resources that were refered to write the code
* The code follows the readme text. Explanatory comments are included for easy navigation of the code. 
* To run the code, place cursor in the code box and press ctrl+enter.  This follows the code output
* The text file of McKinsey Global Institute's Big Data report is enclosed.  This is used as example for Q4 to extract 10 most and least occuring words.

Q1. Kindly write python code in minimal words to create this dictionary (25%)

--> Main dictionary dictMain{} is created by iterating elements of alphabetical and numeric dictionary over the sub-dictionary dictSub{} of counts and results dictionary. The nested for loop pulls all the elements of sub-dictionary into the main dictionary.

Q3. A queue is a data structure where the first element inserted is the first element out (FIFO). Create a class called Queue and define the following attributes – value, id. Write functions input(x) and output() that would imitate the data structure of a queue. Also define functions height() which returns the number of elements in the stack and isempty() which returns true if the stack is empty. (20%)

--> Implemented a queue data structure that handles input and output as FIFO. Initializd class Queue with attributes 'value' and 'id'. Wrote input(), output()  functions to interact with the queue class. 

References:
http://code.activestate.com/recipes/210459-quick-and-easy-fifo-queue-class/ 
https://pymotw.com/2/Queue/ 

Q4. Write a program that reads a text document file and lists down the ten most used words and the ten least used words, along with their count. In the final list, if there is a tie, the clash should be sorted by dictionary preferences. Eg. Aroma will have preference over Brownie if both words occur the same number of times. Kindly use standard file input techniques. Words should at least have a length of 4. (35%) 

--> I have written the wordCounter() function to achieve the required ask. The function takes path of the text document as argument. The document is read and text is split into lower case words using lower() and split() functions. The 'punctuation' package helps to get rid of all punctuation marks. The for loop iterates all words over the file and creates a set of unique words with minimum length of 4 characters. The loop also maintains a count of all unique words. Finally, 10 words are filtered from the list sorted in ascending and descending order of their counts. 

I have used the McKinsey Big Data report as example. We can see that words like 'value', 'productivity', 'health' are top-3 most frequently cited words in the McKinsey report.

To run this program for another text document, call the function wordCounter() and pass the path of the text document. Press Ctrl+enter to run the program, which prints the output of ten most and least occurring words in the document.

References: 
http://stackoverflow.com/questions/27327303/10-most-frequent-words-in-a-string-python 

Q5. Write a program, which will create a list of all unique characters used in a string sentence. The sentence can consist of alphabets, numbers and commas only. (20%) 

--> I have written this program using two approaches. In the first approach, I am appending  characters to an empty list. I append all the characters that are not present in the list, which ensures the list contains only unique characters. In the second approach, I have used the set() function to filter unique characters from the list of all characters of a string. The identical outputs of both programs confirm the accuracy of the two approaches. 

To run this program, call the two functions - uniqueCharList1() OR uniqueCharList2() and pass the string argument. Press Ctrl+enter to run the program, which prints the output of unique characters of the string.
