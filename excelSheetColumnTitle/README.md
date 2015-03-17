#Solution1:

 #Using Package Class StringBuilder

 #Analyze:
 
   ex. 1;
   
    1%26=1 => (char)('A'+1-1) => A      => A
   
   ex. 731; 
   
    731%26=3 => (char)('A'+3-1) => C
    731/26=28
    28%26=2 => (char)('A'+2-1) => B     => ABC
    28/26=1
    1%26=1 => (char)('A'+1-1) => A
    1/26=0
   
   ex. 26; 
   
     6%26=0 => Z
     26-26=0                            => Z
     0/26=0
   
   ex. 702;
   
     702%26=0 => Z
     702-26=676
     676/26=26                          => ZZ
     26%26=0 => Z
     26-26=0
     0/26=0
     
 #Psuedocode:
 
     while(n not zero){
        carry=n%26;
        if(carry==0){n=n-26; StringBuilder.insert(0, Z);}
        else StringBuilder.insert(0, (char)('A'+carry-1))
        n/=26;
     }
  
#Solution 2 & 3
 
  #Analyze:
 
   ex. 1;
   
    1-1=0
    0%26=0 => (char)('A'+0) => A      => A
   
   ex. 731; 
   
    731-1=730
    730%26=2 => (char)('A'+2) => C
    730/26=28
    
    28-1=27
    27%26=1 => (char)('A'+1) => B     => ABC
    27/26=1
    
    1-1=0
    0%26=0 => (char)('A'+1-1) => A
    0/26=0
    
 #Psuedocode:
 
    while(n not zero){
       n=n-1;
       StringBuilder.insert(0, (char)('A'+n%26));}
       n/=26;
     }
    
 #Time Complexity:
 
    O(n)
 
