 #Data Structure:
 
    Binary Tree
    
 #Algorithm:
 
    DFS (pre-order)
    
 #Analyze:
 
    trace left and right branch of binary tree respectively
    
 #Pseudocode:
 
    if(root==null) return 0;
    left=func(root.left);
    right=func(root.right);
    return Math.max(left,right)+1;
