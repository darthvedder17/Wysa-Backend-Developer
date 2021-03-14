# Wysa-Backend-Developer
// Perform inorder traversal and check that each node is greater than the previous 
// Does not work if equal nodes are allowed
// Time: O(n) Space : O(n) logn if balanced
class TreeNode(object):
      self.val = x
      self.left = None
      self.right = None
class Solution(object):
      def isValidBST(self,root):
            self.correct = True
            self.prev = float('-inf')
            self.inorder(root)
            return self.correct
      def inOrder(self,node):
            if not node or not self.correct :
                    return 
            if node.val <= self.prev:
                    self.correct = False
                    return  // Halt exploration
            self.prev = node.val
            self.inOrder(node.right)
