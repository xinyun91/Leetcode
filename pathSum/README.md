 #Data Structure:
 
    Binary Tree
    
 #Algorithm:
 
    Recursion (trace left branch and right brach respectively)
    
 #Analyze:
 
    Note that if node is null, return false (ex.null,sum=0).
    While visit a node, sum=sum-node.val.
    while reach leaf, sum==0, return true, else false.
    
 #Pseudocode:
 
    to check if a node is leaf: (isLeaf(TreeNode node))
    if(node.left and node.right are both null) true;
    others fasle;
    
    if(node is null) return false
    sum=sum-node.val;
    if(isLeaf(node)&&sum==0) return true;
    return hasPathSum(node.left,sum)||hasPathSum(node.right,sum);
    
