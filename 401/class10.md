# Read: Stacks & Queues

## What is the Stack ?

A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Data_stack.svg/1280px-Data_stack.svg.png)


### terminology for a stack

* ** Push ** - Nodes or items that are put into the stack are pushed
* ** Pop ** - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
* ** Top **- This is the top of the stack.
* ** Peek ** - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
* ** IsEmpty ** - returns true when stack is empty otherwise returns false.


## Stacks  concepts:

### *** FILO ***

** First In Last Out **

This means that the first item added in the stack will be the last item popped out of the stack.


### *** LIFO ***

** Last In First Out **

This means that the last item added to the stack will be the first item popped out of the stack.


![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG)

### Why it is always be O(1) operation when you push to the stack ?

This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.



### What is the pseudocode of  push a value onto a stack ?





          ALOGORITHM push(value)

          // INPUT <-- value to add, wrapped in Node internally

          // OUTPUT <-- none

            node = new Node(value)

            node.next <-- Top
            
          
            top <-- Node




### What is the pseudocode of  pop a value from a stack ?



                ALGORITHM pop()

                // INPUT <-- No input

                // OUTPUT <-- value of top Node in stack

                // EXCEPTION if stack is empty


                  Node temp <-- top

                  top <-- top.next

                  temp.next <-- null
                  
                  return temp.value







### What is the pseudocode for a peek ?



        ALGORITHM peek()

        // INPUT <-- none

        // OUTPUT <-- value of top Node in stack

        // EXCEPTION if stack is empty



          return top.value




### what is the pseudocode for isEmpty

          ALGORITHM isEmpty()
          
        // INPUT <-- none

        // OUTPUT <-- boolean

        return top = NULL




 # What is a Queue ?

 A Queue is a linear structure which follows a particular order in which the operations are performed

 ![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2014/02/Queue.png)


* Enqueue - Nodes or items that are added to the queue.

* Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.

* Front - This is the front/first Node of the queue.

* Rear - This is the rear/last Node of the queue.

* Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.

* IsEmpty - returns true when queue is empty otherwise returns false.        

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Queue.PNG)


### Enqueue O(1)
When you add an item to a queue, you use the enqueue action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n); it takes the same amount of time to perform the operation.

### Dequeue O(1) :

When you remove an item from a queue, you use the dequeue action. This is done with an O(1) operation in time because it doesn’t matter how many other items are in the queue, you are always just removing the front Node of the queue.

Typically, you would check isEmpty before conducting a dequeue. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.


### Peek O(1)
When conducting a peek, you will only be inspecting the front Node of the queue.

Typically, you want to check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.


[reference](https://www.geeksforgeeks.org/queue-data-structure/)