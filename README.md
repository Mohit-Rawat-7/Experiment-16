# Experiment-16

## AIM
To use linked list in c++.

## Problem Statement
1.) To create a node in c++.

2.) To add node in c++.

# Theory
In C++, a linked list is a type of data structure that lets you store data in separate memory locations instead of in a single block. It’s made up of a series of nodes, where each node contains two parts: a value (the data it holds) and a pointer that tells you where the next node is located. In this article, we’ll explore what a linked list is, how to implement it, and some practical uses for it.


## Program Codes
1)
```javascript
//Mohit Singh Rawat
//23070123086
#include<iostream>
using namespace std;
class Link {
    public:
    int data;
    Link* next;

    Link(int num){
        data= num;
        next= NULL;
    }
};
void insert_head(Link* &head, int data){
    Link* new_node= new Link(data);
    new_node->next= head;
    head= new_node;
}
void disp(Link* head) {
    Link* temp= head;
    while(temp!=NULL){
        cout<<temp->data<<"->";
        temp= temp->next;
    }
    cout<<"NULL"<<endl;
    }
int main() {
    Link* head= NULL;
    insert_head(head, 30);
    disp(head);
    insert_head(head, 32);
    disp(head);
    insert_head(head, 35);
    disp(head);
    //l1.disp();
    }
```
2)
```javascript
//Mohit Singh Rawat
//23070123086
#include<iostream>
using namespace std;
class Link{
    public:
    int data ;
    Link* next;
    Link(int num){
        data = num;
        next = NULL;
    }
};
int main(){
    Link* l1 = new Link(6);
    cout << l1->data<<"   "<<l1->next;

}
```

## Output
1) <img width="297" alt="Screenshot 2024-10-11 at 10 04 20 AM" src="https://github.com/user-attachments/assets/d0e0e1e6-b856-413e-92ca-07c8461fa6fb">
2) <img width="298" alt="Screenshot 2024-10-11 at 10 07 00 AM" src="https://github.com/user-attachments/assets/c294e430-2a1f-42ea-a47c-7eb9b65a07c6">

## Conclusion
In summary, linked lists offer a flexible way to manage collections of data with dynamic memory allocation. Their unique structure allows for efficient insertions and deletions, making them useful in various applications where such operations are common.

