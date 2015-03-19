 #Data Structure
 
    String; String arrays
    
 #Analyze:
 
    If string arrays is null, return "".
    
    To find longest common prefix, compare first string with other strings in string array.
    
    Two indexes, one points to each char of string, one points to each string.
    
    If char is different or char index exceeds length of other strings, return substring of 1st string.
    
    ex. ["aa","a"] ["aa","ab"]
          |    |
          i    j
    index i moves through each char, j moves through each string
    
 #Pseudocode:
 
    if(string arrays is null) return "";
    for(index1 of char in 1st string){
       for(index2 of other string){
          if(index1 exceeds length of string at index2
             or 
             char at index1 of 1st string is different from char at index1 of other string at index2)
          return substring of 1st string; 
       }
    }
    return substring of 1st string (from 0 to index1);
 
