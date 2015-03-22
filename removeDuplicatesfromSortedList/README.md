 #Data Structure:
 
    Linked List
    
 #Analyze:
 
    Consider 3 classified examples:
    
      1. can be return directly: [], [1]
      2. [1,1]
      3. [1,1,2]
      
    Store head, and create 2 pointers, a and b.
    
    While(either one pointer is not null), go to loop,
    
    loop:
    (if(b is null) a.next=b and return head,
    if(b's next not null and b is diffrent from b's next) a.next=b.next and a=a.next;
    else b=b.next;)
    
    return head
    
