 #Data Structure:
 
    Java collection framework: Map(HashMap),String
    
 #Analyze:
    
    to find integer corresponding to roman, we create roman to integer mapping using hashmap;
    convert each char of string to integer and decides its sign, and sum them, end 
    
    how to decide sign of each char? 
    ex. XXIX (10 10 1 10) +10+10-1+10=29
    ex. XIX (10 1 10) +10-1+10=19
    so, while current char<next char, sign=-1 
    
 #Time Complexity:
 
    O(n) (convert each char within string)
   
 #Pseudocode:
 
    sum=0;
    for(each char in string){
       if(cur<next) sum=+(-1)*cur;
       if(cur>=next) sum=+cur;
    }
    return sum;
   
 
