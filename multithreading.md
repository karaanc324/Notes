## yield(), sleep(), join()
   yield() :- tell thread runner that if any threrad with high or similar priority is waiting, provide the cpu to that thread
              and put it to runnable state. 
   sleep() :- we know
   join() :- wait for the particular thread to join, like counter prog, 1000 times and after thread.start(), we print the
             count. Its variable coz the main thread runs, so if we use thread.join(), main thread is gonna wait for the 
             thread to join.
             
             
## Thread safe
   A class is called thread safe if multiple threads cannot access the same block at the same time.(synchronised keyword)

## start()
   We call start instead of run coz, the start method creates a separate call stack for the current thread running.
   The result of this method is two threads that are running concurrently: the current thread (which returns from the call to      the start method) and the other thread (which executes its run method)

## why synchronised bock?
   Since java is multithreaded language, synchronization is a good way to achieve mutual exclusion on shared resource(s).

## Thread pool
   A thread pool reuses previously created threads to execute current tasks and offers a solution to the problem of thread        cycle overhead and resource thrashing. Since the thread is already existing when the request arrives, the delay introduced      by thread creation is eliminated, making the application more responsive.

## CountDownLatch
   CountDownLatch is used to make sure that a task waits for other threads before it starts. To understand its application,      let us consider a server where the main task can only start when all the required services have started.

## volatile keyword in Java
   When we use volatile keyword with a variable, all the threads read it’s value directly from the memory and don’t cache it
   owever, use of volatile is limited to very restricted set of cases as most of the times atomicity is desired. For example    a simple increment statement such as x = x + 1; or x++ seems to be a single operation but is s really a compound read-        modify-write sequence of operations that must execute atomically.

## Atomic
   Atomic provides wrapper classes for Integer and Long. eg: private AtomicInteger count = new AtomicInteger();                  count.incrementAndGet(); count.get();
   
## Lock for same purpose:
   Lock lock = new ReentrantLock();
   lock.trylock(10, TimeUnit.SECONDS); lock.unlock();
