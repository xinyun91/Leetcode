 #Data Structure:
 
     Binary Tree
     
 #Algorithm:
 
     DFS (post-order)
     
 #Analyze:
 
     calculate depth of left and right branch, and find their diffrence, is larger than '1', then invalid balanced BT
     
 #Pseudocode:
 
     calculate depth: (depth(TreeNode root))
     if(root is null) return 0;
     left=f(root.left);
     right=f(root.right);
     if(|left-right|>1 or left==-1 or right==-1) return -1;
     return 1+Math.max(left,right);
     
     if depth(root)==-1 return false;
     return true;
