 #Data Structrue:

     Binary Tree
   
 #Algorithm:

     DFS(pre-order), recursion(call back to compare if two nodes are same)
   
 #Analyze:

     trace left and right branch respectively, and compare if it's equal
   
 #Pseudocode:

     if(a is null&&b is null) return true;
     if(a is null||b is null||a.val!=b.val) return false;
     return isSame(a.left,b.left)&&isSame(a.right,b.right);
