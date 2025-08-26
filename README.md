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
    
   To conclude, 

3. Emoticon Problem


4. Unpacking List Problem
   
