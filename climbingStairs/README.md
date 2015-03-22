 #Data Structure:
 
    Arrays
    
 #Algorithm:
 
    n=1; 1
    n=2; 2
    n=3; 3
    n=4; 5
    n=5; 8
      .
      .
      .
      
     Recursion: (not good)
     
      if(n==1) return 1;
      if(n==2) return 2;
      return func(n-1)+func(n-2);
      Time consuming and exceed time limit.
      
     Create an int array and log # of ways for each extra step, and return element at end of array
     
 #Pseudocode
      
    create new int array with larger length between 2 and n ;
    element at 0 equals 1;
    element at 1 equals 2;
    for(each element from 2 to end){
       element=pre+pre's pre;
    }
    return (n-1)th element of array
    
