 #Data Structure:
 
    Strings, Arrays
       
 #Analyze:
 
    Versions type is string, ex. 0.1, 1,1, 1.2, 13.37, 13.37.2
    split string by ".", convert each string to int and compare them
    length of 2 versions might be different, and fill by '0'
    
 #Pseudocode:
 
    String arrays v1=split version1;
    String arrays v2=split version2;
    if(v1 length>=v2 length) length=v1;
    if(v2 length>v1 length) length=v2;
    for(each string in v1 and v2 arrays){
       if(String1>String2) return 1; //note: index of string larger than the length, value of string=0
       else if(String1<String2) return -1;
    }
    return 0;
    
 #Time Complexity:
 
    worst: O(n);
