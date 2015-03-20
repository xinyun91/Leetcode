 #Data Structure:
 
      Linked List
     
 #Analyze:
 
     List for merge:
     ex. 2,3,4,6  1,5,7,8 =>  2,3,4,6  1,5,7,8 =>  2,3,4,6  1,5,7,8 => 2,3,4,6  1,5,7,8 => 2,3,4,6  1,5,7,8 =>
         |        |           |          |           |        |            |      |              |    |              
         l1       l2          l1         l2          l1       l2           l1     l2             l1   l2            
         
         2,3,4,6  1,5,7,8 =>  2,3,4,6,null  1,5,7,8
               |      |                |        |
               l1     l2               l1       l2
               
               
       Merged List: 
       l2<l1           l1<l2                  l1<l2                      l1<l2 
         0->1 => 0->1 => 0->1->2 =>  0->1->2 => 0->1->2->3 => 0->1->2->3 =>  0->1->2->3->4 => 0->1->2->3->4 =>
         |       |  |       |        |     |          |       |        |     |        |       |           |
         l3(r)   r  l3      l3       r     l3         l3      r        l3    r        l3      r           l3
         
       l2<l1                                  l1<l2                                          
         0->1->2->3->4->5 => 0->1->2->3->4->5 =>  0->1->2->3->4->5->6 => 0->1->2->3->4->5->6 => 
         |           |       |              |     |              |       |                 |                      
         r           l3      r              l3    r              l3      r                 l3                     
       l1 is null
         0->1->2->3->4->5->6->7->8
         |                 |  |
         r                  l3 l2
         
 #Time Complexity:
 
     worst O(n)
     
 #PseudoCode:
 
     create ListNode l3;
     ListNode r=l3;
     while(l1 and l2 not null){
        if(l1<l2) {l3.next=l1; l1=l1.next;}
        else{l3.next=l2; l2=l2.next;}
        l3=l3.next;
     }
     if(l1 is null) l3.next=l2;
     if(l2 is null) l3.next=l1;
     return r.next;
         
