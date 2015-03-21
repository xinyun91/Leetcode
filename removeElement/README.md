 #Data Structrue:
 
    Arrays
  
 #Algorithm:
 
    Very similar to remove duplicates from sorted array.
    log the length of array,
    Two indexes, suppose a, b,
    if element at a is different from the given value,
    overwrite element at a with b, and a increases its index by 1
    else if element at b is same from the given value, 
    decrease length of array by 1
    
 #Pseudocode:
 
    log length of array;
    for(each element in the array,b++){
       compare with given value:
        if(same) length--;
        else A[a++]=A[b];
    }
    return length;
