# Chapter VI - Concurrency:

- Concurrency is when the execution of two or more pieces of code act as if they run at the same time. **Parallelism** is when they do run at the same time
- Concurrent and parallel code used to be exotic. Now it is required.
- Time is an often ignored aspect of software architectures.
- We need to allow for concurrency and to think about decoupling any time or order dependencies.
- Remember the distinction: concurrency is a software mechanism, and parallelism is a hardware concern.
- Shared state is incorrect state
- A semaphore is simply a thing that only one person can own at a time.
- You can create a semaphore and then use it to control access to some other resource.
- Classically, the operation to grab the semaphore was called P, and the operation to release it was called V. Today we use terms such as lock/unlock, claim/release, and so on.
- A lot of attention is given to shared memory as a source of concurrency problems, but in fact the problems can pop up anywhere where your application code shares mutable resources.
- Whenever two or more instances of your code can access some resource at the same time, you’re looking at a potential problem.
- Random failures are often concurrency issues.
- Concurrency in a shared resource environment is difficult, and managing it yourself is fraught with challenges.
- Use actors for concurrency without shared state.
- In the actor model, there’s no need to write any code to handle concurrency, as there is no shared state.
- The Erlang language and runtime are great examples of an actor implementation, however they are called _processes_ instead.
- You can use blackboards to coordinate workflow, but they come with their own pitfalls.
