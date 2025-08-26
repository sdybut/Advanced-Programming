# Programming Assignment 1

## 1. Alphabet Soup Problem
   This function works by taking a word first, then sort its letters alphabetically, and then formatting the result back into a clean string.

      #create a function and label it as alphabet_soup
      def alphabet_soup (a): 

      #sort the letters alphabetically
      srtd = sorted (a)

      #return as a string then format the output
      #when the output is not formatted the result will be "['e','h','l','l','o']"
      #so to remove the "'" "," "[" "]" i used the syntax .replace
      return str (srtd).replace("'", "").replace("[", "").replace("]", "").replace(", ", "") '

   Output
      
      #arrange from hello to ehllo
      alphabet_soup ("hello")
         #output
         'ehllo'

      #arrange from hacker to acehkr
      alphabet_soup ("hacker")
         #output
         'acehkr'
 
   To conclude, I created a function called alphabet_soup that takes a word first, then sorts its letters in alphabetical order using the syntax sorted(a), and then formats the result into a string. Since sorted() produces an output with a list (for example, ['e','h','l','l','o'] for "hello"), I converted the list into a string and used the syntax .replace() method to remove the brackets, commas, and quotes, resulting only the alphabetically arranged letters that are joined together. In this way, the function outputs only an arranged string like "ehllo" instead of showing the list format.

   
## 2. Emoticon Problem
   This function works by taking a sentence first, then replacing specific words (smile, grin, sad, mad) with their corresponding emoticons:
      smile   ->    :)
      grin    ->    :D
      sad     ->    :((
      mad     ->    >:(

      #create a function and label it as emotify
      def emotify(s):  
      
      #replace "smile" -> ":)" 
      s = s.replace("smile", ":)")  
      #replace "grin" -> ":D"
      s = s.replace("grin", ":D")  
      #replace "sad" -> ":(("
      s = s.replace("sad", ":((")  
      #replace "mad" -> ">:("
      s = s.replace("mad", ">:(")  

      #return into modified output
      return s

   Output
   
      #print Make me smile -> Make me :)
      emotify("Make me smile")
         #output
         'Make me :)'
   
      #print Give me a grin -> Give me a :D
      emotify ("Give me a grin")
         #output
         'Give me a :D'

      #print Don't be sad -> Don't be :((
      emotify ("Don't be sad")
         #output
         'Don't be :(('

      #print I am mad -> I am >:(
      emotify("I am mad")
         #output
         'I am >:('

   In conclusion, I created a function called emotify that takes a sentence and replaces certain words with their corresponding emoticons. Using the .replace() method, the function substitutes "smile" with ":)", "grin" with ":D", "sad" with ":((", and "mad" with ">:(". In this way, whenever these words will appear in a sentence, they are automatically transformed into their specific emoticons I set.



## 3. Unpacking List Problem
   This function works by unpacking a list into three parts: the first element, the middle elements, and the last element.

      #set the list of the values
      writeyourcodehere = [1, 2, 3, 4, 5, 6]

      #print the output as:
      #first: index 0 (first element)
      #middle: slice elements between the index 0 and -1 (elements between first and last element)
      #last: index -1 (last element)
      print ("first:", writeyourcodehere[0], " middle:", writeyourcodehere[1:-1], " last:", writeyourcodehere[-1])

   Output

         #output
         first: 1  middle: [2, 3, 4, 5]  last: 6


   In conclusion, this program unpacks a list into three separate parts: the first element, the middle elements, and the last element. By using indexing, as writeyourcodehere[0] retrieves the first element, writeyourcodehere[1:-1] which slices everything between the first and last elements, and lastly, writeyourcodehere[-1] retrieves the last element. In this way, the list is divided and displayed as three components.
