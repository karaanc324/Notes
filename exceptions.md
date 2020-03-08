## Stack overflow error: 
  - Best example is a never ending recursion.
  - Cyclic classes, like constructor calling another constructor.
  
   When a function call is invoked by a Java application, a stack frame is allocated on the call stack. 
   The stack frame contains the parameters of the invoked method, its local parameters, and the return address 
   of the method. The return address denotes the execution point from which, the program execution shall continue 
   after the invoked method returns. If there is no space for a new stack frame then, the StackOverflowError is 
   hrown by the Java Virtual Machine (JVM).
