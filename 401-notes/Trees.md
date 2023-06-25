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


![preorder](/401-notes/assets/pre8.png) 

`E` will output the console. Since `E` is a leaf, it willcomplete the method code block, and pop `E` off of the call stack and make its way back up to `B`

![preorder](/401-notes/assets/pre9.png) 

In the function call, `B` has already checked for `root.left` and `root.right`. There are no further lines of code to execute, so `B` will poppped off the call stack, so that we can resume execution `A` 

![preorder](/401-notes/assets/pre10.png) 

Following the same pattern as we did with the other nodes, `A`'s call stack frame pick up where it left off, and check out `root.right`. `C` will be added to the call stack frame, and it will become the new functions's `root`

![preorder](/401-notes/assets/pre11.png) 

`C` will be outputted to the console and `root.left` will evaluated. Because `C` has a left child, `preOrder` will called, with paramter `root.left`.

![preorder](/401-notes/assets/pre12.png) 

At this point, the program will find that `F` does not have any children and it will make its way back up the call stack up to `C`

![preorder](/401-notes/assets/pre13.png) 

`C` does not have `root.right`, so it will op off the call stack and return to `A`

![preorder](/401-notes/assets/pre14.png) 

Pre order-traversal is completed

**Traversal Pseudocode**

![preorder](/401-notes/assets/prein.png) 

![preorder](/401-notes/assets/post.png) 


The biggest difference between each of the traversals is **when you are looking at the root node**


### Breadth first traversal iterates throught he tree by going through each level of tree node-by-node. So, given our starting tree one more time:  

![preorder](/401-notes/assets/bread.png) 


Our output using breadth first traversal is now:

Output: `A, B, C, D, E, F`

Traditionally, breadth first traversal uses a queue(instead of a call stack via recursion) to traverse width/breadth of the tree. Let's breadk down the process

Given our starting tree shwon above, let's start by putting the `root` into the queue:

![preorder](/401-notes/assets/bread1.png) 

Now that we have one node in our queue, we can `dequeue` it and use that node in our code.


![preorder](/401-notes/assets/bread2.png) 

From our dequeued node `A`, we can `enqueue` the `left` and `right` child (in that order)

![preorder](/401-notes/assets/bread3.png) 

This leaves us with `B` as the new front of our queue. We can repeat the process we did with `A`: Dequeue the front node, enqueue the node's `left` and `right` nodes, and move to the next new front of the queue

![preorder](/401-notes/assets/bread4.png) 

Now our front is `C`, so we repeat the dequeue + enqueue children process:

![preorder](/401-notes/assets/bread5.png) 

And we continue onwards. when we reach the node that doesn't have children, we just dequeue without any fruther enqueue 

![preorder](/401-notes/assets/bread67.png) 


![preorder](/401-notes/assets/bread8.png) 


**Pseudocode**

Here is the pseudocode, utilizing a built-in queue to implement a breadth first traversal


![preorder](/401-notes/assets/breadth.png) 

### Binary Tree Vs K-ary Trees  

In all of our examples, we've been using a Binary Tree. Trees can have any nuber of children per node, but Binary Trees restrict the number of children to two (hence our `left` and `right` children) 


There is no specific soriting order for binary tree. Nodes can be added into a binary treee wherever space allows. Here is what a binary tree looks like: 


![preorder](/401-notes/assets/binary.png) 


### K-ary Trees

If Nodes are able to have more than 2 child nodes, we call the treee that contains them a K-ary Tree.
In this type of tree we use `K` to refer to the maximum number of children that each Node is able to have 


#### Breadth First Traversal 


Traversing a K-ary tree requires a similar approach to the breadth first traversal. We are still pushing nodes into a queue, but we are not moving down a list of children of length k, instead of checking for the presence of a left and right child. 

![preorder](/401-notes/assets/k-ary.png) 


If we traversed this tree Breadth First we should see the output:


Output: `A,B,C,D,E,F,G,H`

We will start at the `root` Node, and we will add it to our `queue`:

![preorder](/401-notes/assets/kary1.png) 

Much like before, as long as we have a node in our `queue` we can `dequeue`:

![preorder](/401-notes/assets/kary2.png) 

Once these are queueed, can move on to Node `B` at the front of the `queue`, which we can `dequeue` followeding by `enquing` Node `B`'s children:


![preorder](/401-notes/assets/kary34.png) 


This process of `dequeuing` and processing the Nodes at the front of the `queue`, followed by`enqueing` the current Node’s children continues until our `queue` is empty of child Nodes:

![preorder](/401-notes/assets/kary56.png) 


![preorder](/401-notes/assets/kary89.png) 


![preorder](/401-notes/assets/kary10.png) 

#### Pseudocode 

This process is very similar to our binary tree traversal, but now we check a list of children of a left and right child properties. It should look something like this 


![preorder](/401-notes/assets/kpseu.png) 


#### Adding a node. 

Because there are not structural rules for where nodes are "supposed to go" in a binary tree, it really doesn't matter where a new node gets placed.

One strategy for a dding a new node to a binary tree is to fill all "child" spots from the top down. To do so, we would leverage the use of breadth first traversal. During the traversal, we find the first node that does not have all its children filled, and insert the new node as a child. We fill the child slots from left to right.

In the event you would like to have a node placed in a specifc location, you need to reference both the new node to create and the parent node which the child is attached to.

##### Big O

The Big O time complexiity for inserting a new anode is `O(n)`. Searching for a specifc node will also be `O(n)`. Because of the lack of organizational structure in a Binary Search Tree, the worse case for most operations will involve traversing the entire tree. If we assum that a tree has `n` nodes, then the worse case we will have to look at `n` items, hence the `O(n)` complexity. 

The Big O space complexity for node insretion using breadth first insertion will be `O(w)`, where `w` is the largest width of the tree. For example, in the above tree, `w` is 4.

A "perfect" binary tree is one where every non-leafnode has exactly two children. The maximum width for a perfect binary tree, is `2^(h-1),` where `h` is the hieght of the tree. Height can be calculated as `log n`, where `n` is the number of nodes.

### Binary Search Tree

A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST nodes are organized in a manner where all values are smaller than the `root` are placed to the left, and all values that larger than the `root` are placed to the right.

Here ishow we could change our Binary Tree example into a Binary Search Tree:


![preorder](/401-notes/assets/search.png)

Searching a BST can be done quickly, because all you do is compare the node you are searching for against the root of the tree or sub-tree. If the value is samller, you only traverse the left side. If the value is larger, you only traverse the right side. 



Let’s say we are searching 15. We start by comparing the value `15` to the value of the root, `23`.

`15 < 23`, so we traverse the left side of the tree. We then treat 8 as our new “root” to compare against.

`15 > 8`, so we traverse the right side. 16 is our new root.

`15 < 16`, so we traverse the left side. And aha! 15 is our new root and also a match with what we were searching for.

![preorder](/401-notes/assets/search1.png)

The best way to approach a BST search is with a `while` loop. We cycle through the while loop until we hit a leaf, or until we reach a match with what we’re searching for

Big O

The Big O time complexity of a Binary Search Tree’s insertion and search operations is `O(h)`, or `O(height)`. In the worst case, we will have to search all the way down to a leaf, which will require searching through as many nodes as the tree is tall. In a balanced (or “perfect”) tree, the height of the tree is `log(n)`. In an unbalanced tree, the worst case height of the tree is n.

The Big O space complexity of a BST search would be `O(1)`. During a search, we are not allocating any additional space.