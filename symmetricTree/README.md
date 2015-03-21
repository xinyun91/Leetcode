 #Data Structure
 
    Binary Tree
    
 #Algorithm:
 
    DFS (pre-order)
    
 #Analyze:
 
    To check if a tree is mirror of oneself, check if left equals right,
    so we trace the left and right branch respectively. 
    If both left and right are null, tree is symmetric. (ex. 1)
    If left is not equal to right or one branch is null, tree is not symmetric. (ex. 1,2 or 1,2,3)
    
 #Pseudocode:
 
    isMirror(a, b):
      if(a is null and b is null) return true;
      if(a is null or b is null or a not equal to b) return false;
      return isMirror(a.left,b.right) and isMirror(a.right,b.left);
      
    isSymmetric(root):
      if(root==null) return true;
      return isMirror(root.left,root.right);
      
    
