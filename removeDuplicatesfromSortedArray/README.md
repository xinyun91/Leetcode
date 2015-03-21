 #Data Structure:
 
    Array
    
 #Algorithm & Analyze:
 
    Note that the array have been sorted，
    log the length of array, while find duplicated one, length decrease,
    while find element to be unduplicated, 
    ovewrite the duplicate one
    
 #Pseudocode:
 
    log length of array;
    j=0
    for(index from 1 to end of array){
       if(int at index diffrent from that at j) {j++; overide j with element at i;}
       else length--
    }
    return length;
 
