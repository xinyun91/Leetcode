 #Data Structure:
 
    Arrays: str.toCharArray();
    
 #Analyze:
 
    string is null
    +/-sign
    overflow
    while space 
    other character other than digit (unable to convert, return 0)
    
 #Pseudocode:
 
    if(string is empty) return 0;
    sign=1;
    index=0;
    result=0;
    /*white space*/
    while(char is null/empty) index++;
    /*sign*/
    if(char at index is '+') {sign=1; index++;}
    else if(char at index is '-') {sign=-1; index++;}
    /*char is not digit and overflow*/
    while(index<length of char array and char is digit){
       result=result*10+char at index;
       index++;
       if(result*sign>=Integer.MAX_VALUE) return MAX;
       if(result*sign<=Integer.MIN_VALUE) return MIN;
    }
    return r*sign;
