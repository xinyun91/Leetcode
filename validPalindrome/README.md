 #Data Structure:
 
     String
    
 #Analyze:
 
     A=a, so str.toLowerCase() or str.toUpperCase.
     Compare only digit and letter, no punctuation.
    
 #Time Complexity:
 
     O(n)
    
 #Pseudocode:
 
     converst string to lower case or upper case
     create 2 pointers, one points to beginning, and one points to end of string
     while(begin<end){
        while(end>=0&&char is not letter&&char is not digit) end--;
        while(begin<length of string&&char is not letter&&char is not digit) begin++;
        if(begin<end&&char at begin not equal to char at end) return false;
     }
     return true;
