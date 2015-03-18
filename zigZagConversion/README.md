 #Data Structure:
 
    Strings

 #Analyze:
 
    ex. s=ABC  nRows=1  A B C
    ex. s=ABC  nRows=3  A           //Both output "ABC"
                        B
                        C
                        
    ex. nRows=2         0 2         //output order: 0, 2, 1, 3 
                        1 3
                        
    ex. nRows=3         0   4   8
                        1 3 5 7 9
                        2   6   10
                        
    ex. nRows=4         0     6      12
                        1   5 7   11 13
                        2 4   8 10   14
                        3     9      15
    for 1st row and last row, each step distance is 2*nRows-2
    for others between (1st, last), 2 diffrent step distance: 2*nRows-2*(i+1) 
                                                              2*i
                                                              
  #Pseudocode:
  
     for(each rows from 0 to nRows-1){
         key=true;
         while(index<lengthofString){
            get char at index and insert to string
            if(1st or last row) index=index+nRows*2-2;
            else{
              if(key) {index=index+nRows*2-2(i+1); key=false;}
              else {index=index+2*i; key=true;}
            }
         }
     }
    
                                                              
