## trees

* In computer science, a tree is a widely used abstract data type that simulates a hierarchical tree structure, with a root value and subtrees of children with a parent node, represented as a set of linked nodes.

* A tree data structure can be defined recursively as a collection of nodes (starting at a root node), where each node is a data structure consisting of a value, together with a list of references to nodes (the "children"), with the constraints that no reference is duplicated, and none points to the root

### Traversals
1. Depth First : is where we prioritize going through the depth (height) of the tree first
- methods for depth first traversal: Pre-order: root >> left >> right In-order: left >> root >> right Post-order: left >> right >> root
- most common way to traverse through a tree is to use recursion

2. Breadth First: iterates through the tree by going through each level of the tree node-by-node.
- Traditionally, breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree.
- Dequeue the front node, enqueue that node’s left and right nodes, and move to the next new front of the queue.

### Depth First
*Depth first traversal is where we prioritize going through the depth (height) of the tree first*

### Breadth First
*Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.*

### Big O
* The Big O time complexity for inserting a new node isO(n). Searching for a specific node will also be O(n).
*Because of the lack of organizational structure in a Binary Tree, the worst case for most operations will involve traversing the entire tree. If we assume that a tree has n nodes, then in the worst case we will have to look at n items, hence the O(n) complexity.*