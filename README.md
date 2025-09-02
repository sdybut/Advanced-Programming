# Programming Assignment 1

## 1. Alphabet Soup Problem
   This function works by taking a word first, then sort its letters alphabetically, and then formatting the result back into a clean string.

      def alphabet_soup (a):   #create a function and label it as alphabet_soup
      
      srtd = sorted (a)   #sort the letters alphabetically

      return str (srtd).replace("'", "").replace("[", "").replace("]", "").replace(", ", "")   #return as a string then format the output
                                                                                               #when the output is not formatted the result will be "['e','h','l','l','o']"
                                                                                               #so to remove the "'" "," "[" "]" i used the syntax .replace

   **Output**
   
      alphabet_soup ("hello")   #arrange from hello to ehllo
         'ehllo'   #output

      alphabet_soup ("hacker")    #arrange from hacker to acehkr
         'acehkr'   #output
 
   To conclude, I created a function called alphabet_soup that takes a word first, then sorts its letters in alphabetical order using the syntax sorted(a), and then formats the result into a string. Since sorted() produces an output with a list (for example, ['e','h','l','l','o'] for "hello"), I converted the list into a string and used the syntax .replace() method to remove the brackets, commas, and quotes, resulting only the alphabetically arranged letters that are joined together. In this way, the function outputs only an arranged string like "ehllo" instead of showing the list format.

   
## 2. Emoticon Problem
   This function works by taking a sentence first, then replacing specific words (smile, grin, sad, mad) with their corresponding emoticon:
   
| Word | Emoticon |
| --- | --- |
| Smile | :) |
| Grin | :D |
| Sad | :(( |
| Mad | >:( |      

      def emotify(s):   #create a function and label it as emotify
      
      s = s.replace("smile", ":)")    #replace "smile" -> ":)"  
      s = s.replace("grin", ":D")     #replace "grin" -> ":D"
      s = s.replace("sad", ":((")     #replace "sad" -> ":(("
      s = s.replace("mad", ">:(")     #replace "mad" -> ">:("
      
      return s   #return into modified output

   **Output**
   
      emotify("Make me smile")   #print Make me smile -> Make me :)
         'Make me :)'   #output
   
      emotify ("Give me a grin")   #print Give me a grin -> Give me a :D
         'Give me a :D'   #output

      emotify ("Don't be sad")   #print Don't be sad -> Don't be :((
         'Don't be :(('   #output

      emotify("I am mad")    #print I am mad -> I am >:(
         'I am >:('    #output

   In conclusion, I created a function called emotify that takes a sentence and replaces certain words with their corresponding emoticons. Using the .replace() method, the function substitutes "smile" with ":)", "grin" with ":D", "sad" with ":((", and "mad" with ">:(". In this way, whenever these words will appear in a sentence, they are automatically transformed into their specific emoticons I set.


## 3. Unpacking List Problem
   This function works by unpacking a list into three parts: the first element, the middle elements, and the last element.

      writeyourcodehere = [1, 2, 3, 4, 5, 6]    #set the list of the values

      print ("first:", writeyourcodehere[0], " middle:", writeyourcodehere[1:-1], " last:", writeyourcodehere[-1])   #print the output as:
                                                                                                                     #first: index 0 (first element)
                                                                                                                     #middle: slice elements between the index 0 and -1 (elements between first and last element)
                                                                                                                     #last: index -1 (last element)

   **Output**

         first: 1  middle: [2, 3, 4, 5]  last: 6    #output

   In conclusion, this program unpacks a list into three separate parts: the first element, the middle elements, and the last element. By using indexing, as writeyourcodehere[0] retrieves the first element, writeyourcodehere[1:-1] which slices everything between the first and last elements, and lastly, writeyourcodehere[-1] retrieves the last element. In this way, the list is divided and displayed as three components.
