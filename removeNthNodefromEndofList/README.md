 #Data Structure:
 
     Linked List
     
 #Analyze:
    
     to remove the nth node from end of list, so create 2 pointers (ListNode has function of pointer).
     one pointer move n steps in advance, and then 2 pointers move in same pace until end of list.
      ex. 1 2 3 4 5  (n=2)           =>   1 2 3 4 5       =>  b.next=b.next.next    =>   return head
          |   |                           |   |   |
    (head)b   a(2 steps in advance)     head  b   a
    
      ex. 1 null(n=1) => return head.next (or b.next)
          |  |
    (head)b  a
    
 #Time complexity:
   
     O(n)
     
 #Pseudocode:
 
     ListNode a; ListNode b;
     while(n>0) a=a.next;
     if(a==null) return head.next or b.next;
     while(a.next!=null) {a=a.next; b=b.next;}
     b.next=b.next.next;
     return head;
 
