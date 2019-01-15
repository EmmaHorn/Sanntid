# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > Concurrency is when the execution of processes are precieved to be running at the same time. Parallelism is when they are running at the same time.
 
 ### Why have machines become increasingly multicore in the past decade?
 > Multicores improves overall processor performance. Clock speed improvements have decayed over the last decade.
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > Concurrent execution makes it possible to run ultiple tasks in parallell. 
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > *Your answer here*
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > A thread is a part of the operating system. A green thread is scheduled by a virtual machine or runtime library. Threads run in a shared memory space, processes run in separate memory space. Threads and processes are OS-managed. Coroutines are a form of sequential processing (like functions). Only one is executing at a given time. 
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > threads
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > The Python GIL is a lock that allows only one thread to hold the control of the Python interpreter. This means that only one thread can be in a state of execution at any point in time.
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > GIL leaves the thread scheduling to the operating system. 
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > The maximum number of CPUs that can be executing simultaneously.
