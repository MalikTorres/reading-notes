### Trees

### Common Terminology

- Node: A Tree node is a component which may contain its own values, and references to other nodes

- Root: The root is the node at the beginning of the tree

- K: A number that specifies the maximum number of children any node may have in a kary tree. In a binary tree, `k = 2`.

- Left: A reference to one child node, in a binary tree

- Right: A reference to the other child node, in a binary tree

- Edge: The edge in a tree is a the link between a parent and a child node

- Leaf: A leaf is a node that does not have any children

- Height: The height of a tree is the number of edges from the root to the furthest leaf

#### Sample Tree

![Sample Tree](/401-notes/assets/sampletree.png)

### Traversals

Traversing a tree allows us to search for a node, print out the contents of a tree, and more.

- **Depth First**
- **Breadth First**

#### Depth First

Depth first traversal is where we prioritize going through the depth(height) of the tree first. There are multiple ways to carry out depth first traversal, each method changes the order in which we search/print the `root`. Here are three methods for depth first traversal:

- Pre-order: `root >> left >> right`
- In-order: `left >> root >> right`
- Post-orderL `left >> right >> root`

![Example Tree](/401-notes/assets/example.png)


Given the sample tree above, our traversal would result in different paths:

- Pre-order: `A,B,D,E,C,F`
- In-order: `D, E, B, F,C, A`
- Post-order: `D,E,B,F,C,A`


The most common way to traverse through a tree is to use **recursion**. With these traversals, we rely on the call stack to navigate back up the tree when we have reached the end of a sub-path

#### Pre-order traversal

![preorder](/401-notes/assets/pre.png) 


Pre-order means that the `root` has to be looked at first. In our case looking at the root just means that we out its value. When we call `preOrder` for the first time, the `root will be added to the call stack`


![preorder](/401-notes/assets/pre2.png) 

Next, we start reading out `preOrder` functions code from top to bottom. The first line of code reads this 

![preorder](/401-notes/assets/pre4.png) 

This means that we will out the `root.value` pit tp tje console. Then, our next block of code instructs us to check if our `root` has a `left` node set. If the root does, we will then send the `left` node to our `preOrder` method recrusively. This means that we make another function, where `B` is our new `root`. 



The process continues until we reach a leaf node. Here's the state of our treee when we hit our first leaf `D`:


![preorder](/401-notes/assets/pre5.png) 

It's important to note a few things that are about to happen:

  - The program will look for both a `root.left` and `root.right`. Both will return null, so it will end the execution of that method call
  - `D` will pop off the call stack and the `root` will be reassigned back to `B`
    - This is the heart of recursion: when we complete a function call, we pop it off the stack and are able to continue execution through the preious function call 

![preorder](/401-notes/assets/pre7.png)  

The code block will now pick up where it left off when `B` was the root. Since it already looked for `root.left`, it will now look for `root.right`