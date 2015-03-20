 #Data Structure:
 
    Binary Tree
    
 #Algorithm:
 
    Tree Traversal(BFS--pre-order)
    
 #Analyze:
 
    visit each level by left and right branch
    
 #Pseudocode:
 
    addLevel(List<List<Integer>> l, int level, TreeNode root):
      if(root is null) return;
      if(l.size()==level) l.add(new ArrayList<Integer>());
      l.get(level).add(root.val);
      addLevel(l,level+1,root.left);
      addLevel(l,level+1,root.right);
      
    levelOrder(TreeNode root):
      List<List<Integer>> l=new List<List<Integer>>;
      addLevel(l,0,root);
      return l;
