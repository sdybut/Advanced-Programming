# Programming Assignment 1

1. Alphabet Soup Problem
   This function works by taking a word first, then sort its letters alphabetically, and then formatting the result back into a clean string.

   #create a function and label it as alphabet_soup
   def alphabet_soup (a): 

      #sort the letters alphabetically
      srtd = sorted (a)

      #return as a string then format the output
      #when the output is not formatted the result will be "['e','h','l','l','o']"
      #so to remove the "'" "," "[" "]" i used the syntax .replace
      return str (srtd).replace("'", "").replace("[", "").replace("]", "").replace(", ", "")

   #arrange from hello to ehllo
   alphabet_soup ("hello")
      #output
      'ehllo'

   #arrange from hacker to acehkr
   alphabet_soup ("hacker")
      #output
      'acehkr'
    
   To conclude, I created a function called alphabet_soup that takes a word first, then sorts its letters in alphabetical order using the syntax sorted(a), and then formats the result into a string. Since sorted() produces an output with a list (for example, ['e','h','l','l','o'] for "hello"), I converted the list into a string and used the syntax .replace() method to remove the brackets, commas, and quotes, resulting only the alphabetically arranged letters that are joined together. In this way, the function outputs only an arranged string like "ehllo" instead of showing the list format.
   

3. Emoticon Problem


4. Unpacking List Problem
   
