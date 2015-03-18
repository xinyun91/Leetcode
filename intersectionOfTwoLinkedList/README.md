#Solution1:
  
 #Data Structure:
 
    Linked List
    
 #Analyze:
 
    for each linked list, create a pointer
    
    length of 2 linked lists might be same:
    ex. a1
          \
            c2->c3->c4
          /
        b3
    pointers move until 2 pointers point to the intersection node.
    
    length of 2 linked lists might be different:
    ex.     a1->a2
                   \
                     c1->c2->c3->null
                   /
        b1->b2->b3 
    two pointers move in the same pace, when one becomes null, one moves to head of the other linked list, 
    until 2 pointers point to the intersection node.
    
  #Pseudocode:
  
    *a=headA; *b=headB;
    while(a not null and b not null and a not equal b){
        *a=a.next;
        *b=b.next;
        if(a==b) return a or b;
        if(a==null) *a=headB;
        if(b==null) *b=headA;
    }
    if(a==b) return a or b;
    return null;

