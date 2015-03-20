 #Data Structure:
  
     Arrays
     
 #Analyze: 
 
     ex.      [1,2,3,4,5,6,7] n=7, k=3 

     1st loop [7,5,6,1,2,3,4] n=3, k=2

     2nd loop [6,5,7,1,2,3,4] n=2, k=1
     
     3rd loop [5,6,7,1,2,3,4] loop ends
     
 #Algorithm:
 
     range=n-k;
     n=k;
     k=n-range%k;

 Pseudocode:
 
     k=k%n;  
     range=n-k;
     while(k%n!=0){
        for(index from 1 to range){
           temp=element at n-index;
           element at n-index=element at n-index-k;
           element at n-index-k=temp;
        }
        n=k;
        k=n-range%k;
     }
