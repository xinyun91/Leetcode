 #Data Structure:
 
    Arrays
    
 #Analyze:
 
    Fill from end of the array, compare two elements at end of both arrays,
    pick the larger one, and fill in m+n-1,
    note that when element from array was picked, index decrease by 1,
    note that when one array is null, just return the other array,
    repeat until beginning of arrays
    
 #Pseudocode:
 
    while(m or n being larger than zero){
       if(n is zero or element at m is larger than element at n){  
       
       //note: while compare, make sure that index (ex. m-1, n-1) not be out of bounds exception
          A[m+n-1]=A[--m];
       }
       else A[m+n-1]=B[--n];
    }
