# Experiment-16

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

## Output
1) <img width="297" alt="Screenshot 2024-10-11 at 10 04 20 AM" src="https://github.com/user-attachments/assets/d0e0e1e6-b856-413e-92ca-07c8461fa6fb">
