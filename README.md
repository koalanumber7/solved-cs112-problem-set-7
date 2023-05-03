Download Link: https://assignmentchef.com/product/solved-cs112-problem-set-7
<br>
<strong>Problem Set 7</strong>

<strong>AVL Tree</strong>

<ol>

 <li><strong>*</strong> Each node of a BST can be filled with a height value, which is the height of the subtree rooted at that node. The height of a node is the maximum of the height of its children, plus one. The height of an empty tree is -1. Here’s an example, with the value in parentheses indicating the height of the corresponding node:</li>

</ol>

P(3)

/   

M(1)  V(2)

/     /  

A(0)  R(1) X(0)



S(0)

Complete the following recursive method to fill each node of a BST with its height value.

public class BSTNode&lt;T extends Comparable&gt; {

T data;

BSTNode&lt;T&gt; left, right;        int height;

…

}




// Recursively fills height values at all nodes of a binary tree    public static &lt;T extends Comparable&gt;     void fillHeights(BSTNode&lt;T&gt; root) {        // COMPLETE THIS METHOD

…

}

<ol start="2">

 <li>In the AVL tree shown below, the leaf “nodes” are actually <strong>subtrees</strong> whose heights are marked in parentheses:</li>

</ol>

—— D ——-

/                 

B                    F

/                  /       

A         C          E         G

/        /         /        /   

T1   T2   T3   T4    T5   T6   T7   T8

(h-1) (h) (h-1) (h-1) (h+1) (h) (h)   (h)

<ol>

 <li>Mark the heights of the subtrees at every node in the tree. What is the height of the tree?</li>

 <li>Mark the balance factor of each node.</li>

</ol>

<ol start="3">

 <li>Given the following AVL tree:</li>

</ol>

—J—

/        

F         T

/        /    

C    H     N     X

/         /    /

B  E       L   Q  V

/ 

O   S




<ol>

 <li>Determine the height of the subtree rooted at each node in the tree.</li>

 <li>Determine the balance factor of each node in the tree.</li>

 <li>Show the resulting AVL tree after each insertion in the following sequence: (In all AVL trees you show, mark the balance factors next to the nodes.)</li>

</ol>

Insert Z

<ol start="4">

 <li>Starting with an empty AVL tree, the following sequence of keys are inserted one at a time: 1, 2, 5, 3, 4</li>

</ol>

Assume that the tree allows the insertion of duplicate keys.

What is the total units of work performed to get to the final AVL tree, counting only key-to-key comparisons and pointer assignments? Assume each comparison is a unit of work and each pointer assignment is a unit of work. (Do not count pointer assignments used in traversing the tree. Count only assignments used in changing the tree structure.)

<ol start="5">

 <li><strong>*</strong> After an AVL tree insertion, when climbing back up toward the root, a node x is found to be unbalanced. Further, it is determined that x’s balance factor is the same as that of the root, r of its taller subtree (Case 1). Complete the following rotateCase1 method to perform the required rotation to rebalance the tree at node x. You may assume that x is not the root of the tree.</li>

</ol>

public class AVLTreeNode&lt;T extends Comparable&lt;T&gt;&gt; {        public T data;

public AVLTreeNode&lt;T&gt; left, right;

public char balanceFactor;   // ‘-‘ or ‘/’ or ‘’        public AVLTreeNode&lt;T&gt; parent;        public int height;

}

public static &lt;T extends Comparable&lt;T&gt;&gt;     void rotateCase1(AVLTreeNode&lt;T&gt; x) {

// COMPLETE THIS METHOD

}