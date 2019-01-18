# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > *Concurrency: Multiple task that run overlapping time periods with no specific order. Parallelism: Multiple tasks or parts of a task run at the same time. One splitt up tasks and run different parts, while one run multipeltasks at thesametime.*

 ### Why have machines become increasingly multicore in the past decade?
 > *More parallelism. Run more tasks at the same time. Approachinglimit on speed.*

 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > *Many users on websites.
Server queue
Graphic backgrounds*

 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > *Both, can be easier to make a program work fast enough, but can be hard to impliment propperly.*

 ### What are the differences between processes, threads, green threads, and coroutines?
 > *Process: OS-managed, truly concurrent, own address space.
Thread: OS-managed, parents address space.
Green-Thread: Not OS-managed threads.
Coroutines:Not truly concurrent tread.Not OS mannaged, Co-operatively multitasking*

 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > *Threads, Threads, coroutines*

 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > *Only allows one thread to control the Python interpreter.*

 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *Use multi-processing instead of multi-threading.*

 ### What does `func GOMAXPROCS(n int) int` change?
 > *Controls the number of operating systems threads allocated to goroutine.*
