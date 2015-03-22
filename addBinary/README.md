 #Data Structure:
 
    String
    
 #Algorithm:
 
    Log length of 2 binary strings and carry.
    Add element in 2 string and carry,
    module by 2 is bit after addition,
    divide by 2 is carry,
    fill before short string with '0'.
    
 #Pseudocode:
 
    create a new string;
    m's length m;
    n's length n;
    carry=0;
    if(m or n or carry larger than zero){
        if(m>0) integer m1=char at index --m-'0',
        else m1=0;
        if(n>0) integer n1=char at index --n-'0',
        else n1=0;
        insert (m1+n1+carry)%2 in beginning of string;
        carry=(m1+n1+carry)/2;
    }
    return string;
