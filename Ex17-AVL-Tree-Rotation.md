# Ex17 AVL Tree – Rotation
## DATE:
## AIM:
To write a C function to perform right rotation in an AVL Tree.

## Algorithm
1. Start 
2. Set y to the left child of x. 
3. Set the left child of x to be the right child of y. 
4. Set the right child of y to be x. 
5. Update the height of x and y. 
6. Return y as the new root after rotation. 
7. End 
## Program:
```
/*
Program to perform right rotation in AVL Tree
Developed by: Nandhika P
RegisterNumber:  212223040125
*/

typedef struct node 
{ 
int data; 
struct node *left,*right; 
int ht; 
}node; 
node *insert(node *,int); 
//node *Delete(node *,int); 
void preorder(node *); 
//void inorder(node *); 
int height( node *); 
node *rotateright(node *); 
node *rotateleft(node *); 
node *RR(node *); 
node *LL(node *); 
node *LR(node *); 
node *RL(node *); 
*/ 
node * rotateright(node *x) 
{ 
node *y; 
y=x->left; 
x->left=y->right; 
y->right=x;  
x->ht=height(x); 
y->ht=height(y); 
return(y); 
} 
```

## Output:

![image](https://github.com/user-attachments/assets/26298e3f-7e55-4882-875e-9a017855fb5c)



## Result:
Thus, the function to perform right rotation in an AVL Tree is implemented successfully.
