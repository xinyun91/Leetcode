 #Analyze:
    
    sign: '+' or '-'
    integer overflow: valid integer range -2,147,483,648 to 2,147,483,647
                      ex. 1,111,111,118 -> 8,111,111,111 (invalid integer)
                        
 #Algorithm: 
 
    carry=n%10
    reversed=reversed*10+carry
    n=n/10
    
 #Pseudocode:
    
    convert integer(n) to long to avoid overflow;
    reversed=0;
    while(n not zero){
       carry=n%10;
       reversed=reversed*10+carry;
       n/=10;
    }
    if(reversed<Integer.MIN_VALUE or >Integer.MAX_VALUE) return 0;
    return reversed (convert long to integer)
    
