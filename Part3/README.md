# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > Concurrency: two or several tasks runs virtually at the same time. It is based on CPU time-slicing, where only one works while the others are in a waiting state.
Parallelism: several tasks or a task that is divided into smaller tasks runs at the exact same time by using a multi-core structure.


 ### Why have machines become increasingly multicore in the past decade?
 > We are starting to reach the limit for the clock speed for one processor, but we can increase the number of tasks by introducing several cores and operate them at the same time.

 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > We can solve multiple independent tasks simultaneously.

 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > It gets more complicated as you control several things at the same time.

 ### What are the differences between processes, threads, green threads, and coroutines?
 > 

 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > threading.Thread() will create a thread, while go create a coroutine.

 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > It synchronizes the execution of threads so that only one native thread can execute at a time.  

 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *Your answer here*

 ### What does `func GOMAXPROCS(n int) int` change?
 > It sets the maximum number of CPUs that can be executing simultaneously.
