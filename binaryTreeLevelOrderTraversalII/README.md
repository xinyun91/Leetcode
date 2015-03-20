 #Data Structure:
 
    Binary Tree, List (ArrayList)
    
 #Algorithm:
 
    Tree Traverse (BFS--pre-order)
    
 #Pesudocode:
 
    addLevel(List<List<Integer>> l, int level, TreeNode root):
    if(root is null) return;
    if(list size=level) l.add(new ArrayList);
    l.get(size-level-1).add(root.val);
    addLevel(l,level+1,root.left);
    addLevel(l,level+1,root.right);
    
    levelOrderBottom(TreeNode root):
    new list;
    addLevel(l,0,root);
    return l;
    
    
