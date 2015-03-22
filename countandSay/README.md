 #Data Structure:
 
    String
   
 #Algorithm:
 
    nth string => first think about recursion
    Observing the pattern:
     1: "1"
     2: "11"
     3: "21"
     4: "1211"
     5: "111221"
     6: "312211"
        .
        .
        .
    we find nth string depends on (n-1)th String,
    so we need store (n-1)th string as reference to calculate the nth one
    
    and yes! here we use recursion
    
 #Pseudocode:
 
    countAndSay(int n):
       return helper(n, "1");
    
    helper(int n, String s):
       if(n==1) return s; 
       if(n>1){
          int j=0;
          for(int i=0;i<s.length();i++){
             if(element at i is diffrent from that at j) append (i-j) and elem at j to string and j=i;
             if(i==index at end of string) append (i-j+1) and elem at j to String;
             
             /* at first I want to use a variable (count) to help recording the duplicated element,
             I choose (i-j) to take place of count. */
             
          }
       }
       return helper(n-1, sb.toString());
