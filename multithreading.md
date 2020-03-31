## yield(), sleep(), join()
   yield() :- tell thread runner that if any threrad with high or similar priority is waiting, provide the cpu to that thread
              and put it to runnable state.
   sleep() :- we know
   join() :- wait for the particular thread to join, like counter prog, 1000 times and after thread.start(), we print the
             count. Its variable coz the main thread runs, so if we use thread.join(), main thread is gonna wait for the 
             thread to join.
             
             
## Thread safe
   A class is called thread safe if multiple threads cannot access the same block at the same time.(synchronised keyword)

## Start method
   We call start instead of run coz, the start method creates a separate call stack for the current thread running.
   The result of this method is two threads that are running concurrently: the current thread (which returns from the call to      the start method) and the other thread (which executes its run method)
