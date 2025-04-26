# Ex 3C Expression Tree
## DATE:17-03-2025
## AIM:
To write a C function to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

## Algorithm
1. 	Start
2.	Print node data in preorder then traverse left then right
3.	Traverse left in inorder then print node data then traverse right
4.	Traverse left in postorder then traverse right then print node data
5.	Recursive approach is used for all three traversal methods
6.	Functions handle each tree node using tree->d, tree->l, tree->r
7.	End

## Program:
```
/*
Program to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.
Developed by: ETTA SUPRAJA
RegisterNumber: 212223220022 
*/
/*
struct n { char d; struct n*l; struct n*r;
};*/
voidpreOrder(struct n*tree)
{
if(tree)
{
printf("%c",tree->d); preOrder(tree->l); preOrder(tree->r);
}
}
void inOrder(struct n*tree)
{
if(tree)
{
inOrder(tree->l); printf("%c",tree->d); inOrder(tree->r);
}
}
voidpostOrder(struct n*tree)
 
{
if(tree)
{
postOrder(tree->l); postOrder(tree->r); printf("%c",tree->d);
}
}

```

## Output:

![WhatsApp Image 2025-04-26 at 16 21 30_61a12824](https://github.com/user-attachments/assets/78e9f36b-6261-4141-80f2-70a84b63f4bf)


## Result:
Thus, the C program to display the Expression Tree in the format of In-order ,Pre-order and Post-order traversal.
