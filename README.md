# Module-11
# 19CS301-Module3
### Register No - 212222020008
### Name - Harini B

# ExNo: 11.1 Singly Linked List (Traversal, Search and Delete)
### Aim: To Write a function to traverse the linked list and display it in the following format.
### Algorithm:

1. Start
2. Create a Node class:
Contains two attributes:

data: stores the value of the node

next: points to the next node (initially None)

3. Create a SinglyLinkedList class:
Contains two attributes:

head: points to the first node (initially None)

tail: points to the last node (initially None)

4. Define a method addNode(data):
If the list is empty (i.e., tail is None):

Create a new node and set both head and tail to it

Else:

Create a new node

Link the current tail to this new node

Update tail to the new node

5. Define a method display():
Start from the head

While the current node is not None:

Print the data

Move to the next node

6. Main Program:
Create an object of SinglyLinkedList

Read an integer n (number of nodes)

Repeat n times:

Read node data

Add the data to the linked list using addNode(data)

Call the display() method to print the linked list

7. End

### Program:
```
class Node:
    def __init__(self, data):
       self.data = data
       self.next = None
 
class SinglyLinkedList:
    def __init__(self):
        self.head = None
        self.tail = None
 
#Creating addNode() to add newly created nodes.
    def addNode(self, data):
        if self.tail is None:
            self.head = Node(data)
            self.tail = self.head
        else:
            self.tail.next = Node(data)
            self.tail = self.tail.next

 #Creating display() to print newly created nodes via traversing.
    def display(self):
        current=self.head
        while current is not None:
            print(current.data,end=" ")
            current=current.next
            
 
s = SinglyLinkedList()
n = int(input())
for i in range(n):
    data=input()
    s.addNode(data)
s.display()
```
### OUTPUT:

![image](https://github.com/user-attachments/assets/a61bf8f9-da12-411a-8c12-905abbd4a15a)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 11.2 
### Aim: To Write a python program to insert an element at the starting of the singly linked list.

### Algorithm:

STEP 1: Start.

STEP 2: Define a Node class to hold data and a reference to the next node.

STEP 3: Define a CreateList class to manage the linked list with a head pointer.

STEP 4: In the addAtStart method, create a new node, link it to the current head, and update the head to this new node.

STEP 5: In the display method, traverse from the head and print each node's data; if the list is empty, print a message.

STEP 6: Create an object of the CreateList class and call addAtStart multiple times to add data to the front of the list.

STEP 7: Call the display method after each insertion to show the current state of the list and stop.

### Program:
```
class Node:    
  def __init__(self,data):    
    self.data = data   
    self.next = None   
     
class CreateList:    
  def __init__(self):    
    self.head = None   
     
        
  def addAtStart(self,data):    
    new_node =Node(data)
    new_node.next=self.head
    self.head=new_node
     
  def display(self):    
    current = self.head    
    if self.head is None:    
      print("List is empty")  
      return
    else:    
        print("Adding nodes to the start of the list: ")   
        print(current.data) 
        while(current.next != None):    
            current = current.next  
            print(current.data)   
        
     

cl = CreateList()  
      
cl.addAtStart(1)    
cl.display()    
     
cl.addAtStart(2)    
cl.display()    
     
cl.addAtStart(3)    
cl.display()    
      
cl.addAtStart(4)    
cl.display()    
```
### OUTPUT:
![image](https://github.com/user-attachments/assets/5cc5d231-d1fd-40ab-bf3d-739d3f7a654c)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 3.3 List
### Aim: To write a non parameterized function to print the list in descending order that is entered by the user.
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Define a function `sortlist()`.

**STEP 3:** Inside the function:
- Get a list input from the user using `eval(input())` and store it in variable `a`.

**STEP 4:** Sort the list `a` in descending order using `a.sort(reverse=True)`.

**STEP 5:** Print the sorted list.

**STEP 6:** Call the function `sortlist()`.

**STEP 7:** Stop.

### Program:
```
def sortlist():
     a = eval(input())
     a.sort(reverse=True)
     print(a)

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/f5457e85-36de-4142-890d-717d2dc1ec7c)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 3.4 Tuples
### Aim: To write a python program to create the tuple by the multiples of 5 up to N. Get the N value from the user.
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Create a variable `a`.

**STEP 3:** Get the value of `a` from the user.

**STEP 4:** Create an empty list `l`.

**STEP 5:** Use a `for` loop to iterate from 5 to `a` (exclusive) in steps of 5:
- Append each number to the list `l`.

**STEP 6:** Convert the list `l` to a tuple `x`.

**STEP 7:** Print the tuple `x`.

**STEP 8:** Stop.

### Program:
```
def sortlist():
     a = eval(input())
     a.sort(reverse=True)
     print(a)

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/60fa3c68-0f59-4bc5-bfc1-3629fefff45b)

### Result: Thus, the given program is implemented and executed successfully .
