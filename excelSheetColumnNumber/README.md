 #DataStru: 

     Strings or Arrays

 #Analyze: 

        A: 1    
        1        
        
        A A: 26 * 1 + 1
        1 1
        
        A A A: 26 * (26 * 1 + 1) + 1
        1 1 1
        
        A B C D: 26 * (26 * (26 * 1 + 2) + 3) + 4
        1 2 3 4

 #Pseudocode: 

     result=0; for(eachchar){ eachchar = eachchar-'A'+1; result = 26*result+eachchar; }
