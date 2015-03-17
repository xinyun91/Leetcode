#Solution1:

 #Analyze: the majority element is the one appears more than n/2 times
 
 #Psuedocode: 
 
    sort Arrays;
    count=0;
    for(each int i in num Arrays){
    if(i==previous) {
       count++; 
       if(count>=n/2) return i;
       }
    else count=0;
    }

#Solution2:

 #Pseudocode:

    count=0;
    majorityElement=0;
    for(each int i in num Arrays){
    if(count==0) {majorityElement=i; count++;}
    else {
          if(majorityElement==i) count++; 
          else count--;
         }
    }
