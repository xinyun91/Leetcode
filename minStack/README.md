 #Analyze:
 
    to return min element, might need 2 stack, one for all pushed data, one for storing min value
    ex. 2,0,3,0
    min: 0       pop:0
    min: 0       pop:3
    min: 0       pop:0
    min: 2       pop:2
    stack        minstack (min val of stack is peek element)
    0
    3            0
    0            0
    2            2
    while peek of two stacks hava same value, then remove both, else remove peek val of general stack
    
 #Pseudocode:
 
    push:
    push x to stack
    if(minstack is empty or x is less than peek val of minstack) push x to minstack
    
    pop:
    pop peek element of stack
    if(peek element of stack and minstack equals) pop also peel element of minstack
    
 #Notice:
   
    diffrent between ".equals()" and "=="
    "==" is reference comparison, 2 objects point to the same memory location.
    ".equals" is value comparison. 
    here ".equals" is used as 2 peek val are in different stack
    http://stackoverflow.com/questions/7520432/java-vs-equals-confusion
