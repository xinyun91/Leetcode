 #Data Structure:
 
     Binary Tree
     
 #Algorithm:
 
     Tree Traversal/ Tree Search
     Here: DFS (post-order)
     
 #Analyze:
 
     Recursion, and recurse from bottom to top
     
 #Pseudocode:
 
     if(node is null) return 0;
     left=func(node.left);
     right=func(node.right);
     if(Math.min(left, right) is zero) return 1+Math.max(left,right);
     return 1+Math.min(left,right);
