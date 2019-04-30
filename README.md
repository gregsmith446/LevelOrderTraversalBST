# LevelOrderTraversalBST
23 - Use a queue to perform a breadth-first-traversal on the BST, printing the traversal to the console.

A level-order traversal, also known as a breadth-first search, visits each level of a tree's nodes from left to right, top to bottom.   
You are given a pointer, "root", pointing to the root of a binary search tree.  
Complete the levelOrder functionso that it prints the level-order traversal of the binary search tree.

Sample Input  
6  
3  
5  
4  
7  
2  
1  

Sample Output    
3 2 5 1 4 7 

Steps used:  
1.)Create a queue that holds the Node Data type.  

Queue<Node> queue = new Queue<Node>();

2.)Add the root node of the BST to the just created queue.  

3.)While there are still nodes in the BST --> using queue.Dequeue(),  
travel through the nodes, writing to the console after each node is added to the queue.  

4.)Determine whether the left or right nodes on the current node are empty. If they are not we add them to the queue.

This will always print the most recently added node in the queue.

