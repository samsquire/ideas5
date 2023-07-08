# ideas5
Welcome to the fifth batch page of my Ideas for Computing. This is a stream of my thoughts while working on computers with the theme of integration and improvement of how computers work.

 * See [100 Ideas for Computing](HTTPS://GitHub.com/samsquire/ideas), the first issue of this series.
 * See [ideas2, Another 85+ Ideas For Computing](HTTPS://GitHub.com/samsquire/ideas2)
 * See [ideas3, An Extra 100 Ideas for Computing](HTTPS://GitHub.com/samsquire/ideas3)
 * See [ideas4, Additional 100+ Ideas for Computing]([samsquire/ideas4: An Additional 100 Ideas for Computing https://samsquire.github.io/ideas4/](https://github.com/samsquire/ideas4))
 * [Follow me on Twitter](HTTPS://twitter.com/mrsamuelsquire)
 * Looking for business ideas? Checkout my [startups repository](https://github.com/samsquire/startups) where I list business ideas.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

# 1. Dynamic type crystallization

Any variable can contain any type of data, but once it is set to a type, its type cannot be changed to another type. Our adaptive or specialised compilation can flip to a specialised case with this rule and it never needs to hit a slow path except the first time.

# 2. Matrix multiplication on matrixes of movements of identities

Matrix multiplication is very useful, but what if matrix multiplication can be useful with the movement of identities through a program space? A matrix multiplication is similar to a breadth first search.

# 3. VLIW software

# 4. Orthogonality and nested placement relationships and rules

When we move things around, we may also want to move them according to a multiple rules simultaneously.

# 5. No matter how small or large the task, it composes and parallelises well

Imagine you're writing a web scraper, there are multiple steps in the procedure to scraping that need to be efficiently multitasked and scheduled. It would be nice if the unit of parallelization could be scaled up and down based on the characteristics of the calculation.

# 6. Internet triggered soft upgrade

Soft upgrade is a virtual upgrade but not an actual upgrade. In-place pauseless and synchronized upgrades

# 7. Code maps

A standardised syntax for describing behaviour, used as a comment to find code easily.



```
```

# 8. Can Graph thinking solve logic puzzles quicker?

# 9. Linux single sign in

# 10. Orthogonality of stacks and joins

`callCC` and delimited continuations.

# 11. GUI state container

What's a GUI container? A GUI container is similar to the active memory of a REPL. It interprets the objects in memory and tries to render them in an attractive way that makes sense.

We can use type systems to define what state the GUI should be in. The GUI container is an object area that receives collections of objects and decides how to render them. The behaviour of the application is defined by the types.

# 12. Beautiful API first

The beautiful API is more important than even efficiency, and in theory a properly designed API can have hints, for compiling for a more performant solution.

# 13. Data method calls

Data only, they insert data or associations with an object, not run code.

# 14. Dynamic compiled

In Ruby on Rails, methods are created automatically, at run time to provide features. Couldn't we generate these method calls at compile time.

# 15. Everything is brittle and breaks all the time

# 16. Imaginary framework

# 17. Custom patches part of the package manager

It should be easy to apply custom patches to code and package it easily, the build pipeline should support it.

# 18. Changing software is extremely painful

# 19. Non ASCII tokens direct parse-to-parse mapping

This idea is based on using assembly as an output language for a compiler. Using text output is extremely elegant API for code but is not very efficient due to the requirement to serialize and parse, especially for something such as a JIT compiler that needs to compile frequently and as fast as possible. It is inefficient to generate/emit streams of text that shall only be parsed again by the assembler.

What if we could skip the text component and communicate binary directly between the part that serialises and the part that deserialises but still maintain the textual API from the programmer's perspective? 

Instead we turn textual tokens into an compile time API, in other words the compiler encodes the tokens of the lexer into a binary protocol. This way the assembler can skip parsing because it has the data structure already in binary.

Rather than writing code that parses ASCII at runtime, we want to remove the code of the code that actually serialises and deserialises ASCII to tokens, instead our compiler accepts an assembly-like syntax at compile time, which is then turned into correct calls into the assembly runtime, skipping parsing of text.

What if there was a compile time API that looked like this but actually mapped to binary API at compile time, rather than runtime?

```
_loop:
	# yield to the coroutine
	YIELD
    sub $8, %rsp
    pushq %rax
    pushq %rcx
    pushq %rdx
    pushq %rbx
    pushq %rbp
	leaq	.LC9(%rip), %rax
	movq	%rax, %rdi
    movl    %edx, %esi
	movl	$0, %eax
	call	printf@PLT
	movl	$0, %eax
    popq %rbp
    popq %rbx
    popq %rdx
    popq %rcx
    popq %rax
	# i += 1
	inc %rax
	# move onto the next coroutine
	add $32, %rcx
	# Loop things
	cmp $10, %rax
	jl _loop
	jmp _exit

	# popq	%rbp
    ret
```



# 20. Snippet LISP

Break LISP into named blocks and compose them together, avoid nested LISP confusion.

I don't like seeing `))))))` in my LISP code because I don't know which one to insert between to insert into the right part of the AST tree. So I would combine my lisp with equal statements.

```
if_recur = (if (< i (count lines))
					(recur inext)
					-1)
					)

line_equal = (if (= (nth lines i) "ec2-18-130-242-27.eu-west-2.compute.amazonaws.com")
				 i
				if_recur)

find_host_index = (let [node_data (slurp "nodes") 
	 lines (str/split node_data #"\n") 
	 index (loop [i 0]
		(let [inext (+ i 1)]
			line_equal) ]
	(println index)
					)
					
try_block = (try 6
           (catch Exception e 
                  (println e)
                  nil))
                  
next = (loop []
  (or try_block
      (recur)))
```

# 21. Protocols are surprisingly complicated

# 22. Elegant protocols

# 23. Timing

# 24. Rich runtime applied to network protocols

The network protocol is essentially a set of processes, of state machines that are independently scheduled.

# 25 Expected things to do with a protocol

We should never get into a state where the server crashes or we get broken pipe.

# 26. Giant statemachine

The state of the remote server, the state of the active server and the state of the data being sent back and forth.

# 27. Common coding errors

Did you turn off the thing that isn't working? Did you shut down the server

Did you change the right object?

Did you do the thing inside or outside the loop?

is your loop try and except the right way round?

# 28. Distributed Match states, Connected everything, assert on anything



# 29. Search imports

# 30. Standard consideration mitigation

There's a batch of considerations to be considered when building a system, for example, is latency low even after continual usage?

# 31. Good targets

* 10,000 connections
* 1000MBs per second
* 100s of producers
* 100s of consumers
* 100s of applications on one container
* 600,000 requests per second
* Efficient with Billion records

# 32. Promises - When numbers are equal

We can implement promises and mutual exclusion with numbers that are either equal or not equal. Do this thing when these numbers are equal.

# 33. Bit mask scheduling

# 34. Statelines diagram

Draw statelines which show transit of values through system rather than progression of logic.

# 35. The pedanticness of a fair benchmark should be incorporated into product design

Many companies deny benchmarks of their software. 

# 36. Robust package management ideas

Package managers get into strange states.

# 37. Data defines the software

# 38. Breaking a computation across machines, chunk computation

How do you divide any arbitrary computation across boxes, for data sizes that are beyond any given box?

Threads, multithreading, sharding, and computation larger than a single machine

# 39. Language should have efficient automatic serialization

# 40. Data shipping home

Trivially easy data migration pipelines.

# 41. Markdown to crud website

# 42. Behavioural resources

Create resources similar to CRUD that have behaviours.

# 43. The Bottom Abstraction - Composing behaviours is a huge problem

When building a system, it is often helpful to have a bottom abstraction, that other things are based upon. What's the bottom abstraction anyway? How do you compose behaviours?

* I want data to be migratable easily from machine to machine, from a graphical user interface.
* I want IO and CPU computation to be parallelisable
* In LISP it is lists and trees.
* Instruction Set Architecture is instructions to do mathematical operations and move things around memory and move through instructions.

# 44. Reverse log to AST tree, state transition events to state machine

Log to reverse tree to work out logic order.

State machine code from events

# 45. Coordinated runtimes

After looking into liburing, it occurred to me that behaviours of systems should be generalised for the best possible performance.

# 46. It's impossible to segfault if we know the range of what is valid

Because you import what you use and what you expect to be where and what you expect each data structure to contain. It's not possible to dereference a value to an invalid piece of memory.

Parsing associated with blocking.

# 47. Can we infer the movement through instructions?

# 48. Monetisation system

Monetization doesn't need to ruin a website.

# 49. Complete program, separated into pieces, re-stitched together into new program

Imagine you have a complete program that does a task and we want to do a variation of what the existing program does. We can do a simple transformation to get the program into a form that we can extend:

* inline all internal methods until only platform calls exist
* label parameters that pass through the program through to these platform/system calls and give them a type
* accept, recv, send loop



can tweak relationships of the task, mix and match the code to do what we want.

For example, a simple uring program can act as a webserver and send data to clients.

Can add threading and cross thread communication to different pieces of code.



rich runtime can be used to distribute processing too

synchronization is just loops



# 50. Hierarchy of event loops

raise to previous event loop, state machine coordination

# 51. Render the code differently, simplified rendering of code

# 52. Complicated behaviour made easy

can think about raft and state machine futures easily

# 53. Graph inflection points

scheduling is an inflection point on a wave function

# 53. Structure of code references that are useful

What is the shape of the program?

# 54. Parameterless programming

Chain together methods, define relationships as links that pass through the program. The important thing is the chaining together of methods.

# 55. Roleplay language and pattern matching global state

Instantiate objects and create roles to play.

# 56. Stateful circle, programs on rails

With stateful programs, it can be difficult to reason about them when there are interactions between different actors or nodes. This idea is that we represent all actors in the systems as circles, which always progress forward. We define circles for each actor and circles for overall progress. We link states between circles together which form valid pathways of execution.

* We define a schema of the presence of facts and the progression through different facts.
* Any progression backwards is an invalid state, which means there is a bug in the program.
* An unexpected state change is a bug.
* You could say that state is montonically increasing at all times.
* No matter what interactions with other objects, all circles shall turn forwards.
* Can use logical clocks to identify causality.
* Numbers that increment are new states.
* When global state is checked, that is communication with a global actor, presumably under a lock.
* We can output logs of each thread periodically and analyse the logs to see if the schema was maintained.
* Trapped state detection: No path of state associations back to the global circle, so it's impossible for the circle to move forward.
* You must write a determine state function to determine the facts about the system at the current time. Concurrent events are represented.
* Can create incremental state machines which are snapshots of valid cases, which are stitched together.

For example, we want to schedule two actors, A 5 times and B 5 times and run them alternatedly. AAAAABBBBBAAAAABBBBBAAAAABBBBBAAAAABBBBBAAAAABBBBB,

The "dot" symbol is a "join" from one state to another state. State changes are atomic because processing is evaluated before scheduling time.

```
global = actor(A).scheduled actor(!A).not_scheduled | actor(B).scheduled actor(!B).not_scheduled | regenerate

actor(A-B) = scheduled submitted++ | submitted == total | completed reset submitted = 0 | not_scheduled
```

This can be read as the following:

```
When the actor(A) is scheduled, every actor that is not A is not_scheduled.
Actors that are scheduled are submitted++ until submitted == total and then submitted is set to 0 and they are not_scheduled.
```



Concurrent state changes

Must define a function for each actor and global state: 

Can write a test that tests state and then checks if the state is valid progression, according to the schema.

Guaranteed to make progress.

State explosion.

Desired outcome: alternated scheduling of ABABABAB

```
range submitted..locks

```

interactions between things, what happens next

```
a1 a2 a3 b1 b2 b3

```



special cased work - throwing effort at the problem

legilislational hardness

# 57. Code focus

Enable/disable log lines after running and show/hide log lines that came from there.

# 58. A database is hard to change

# 59. OpenConsult

# 60. Product mixer

# 61. High level low level concern mixing, whenever syntax

How do you mix high level and low level concerns?

High level specification of what should happen, high level logic:

```
checkout-button | review-basket | checkout | sign-in-or-guest-checkout | delivery-address | delivery-options | payment-detils | place-order | payment | send-order-confirmation 
```



Low level specification of what should happen, low level logic,

weave them together

* when "sending an api request", "write it to the write ahead log"

# 62. Calculation complexity score

A computation specification language that includes a complexity score.

* round trip times
* thread synchronizations
* amount of data
* amount of records

# 63. Concurrent hash join

Multiple users are doing the same query, we can share the large table.

# 64. Markdown GUI format

# 65. Exclusive content

# 66. Logic of the kernel

# 67. Readable code

# 68. Turing complete is the golden standard

But we want to do is constrain turing completeness without constraining it.

Such as a builder pattern, to define what should happen when. We want to configure something. To compile it.

Builder pattern that maps to assembly.

Declarative, imperative, something new.

We seem to want to 



# 69. New versions breaking code

# 70. Marketing and demand matching is an unsolved problem

# 71. Event loops and coroutines

# 72. Is assembly might not be the lowest common denominator

# 73. Scheduled Collective Attention

Attention is qualified.

# 74. Code supported by one person is not dependable



# 75. Cache invalidation and GUIs

# 76. Per programming project information system

# 77. Dispatch/Jumping around intelligently more valuable than actual mathematical operations on a CPU

For example, all the methods that must be called in the right order to create a GUI.

# 78. API State machines

Each API call is a mini process with a behaviour.

# 79. Omnichannel distributed system

Frontend and backend cordinated from same codebase.

There was a Haskell project that seamlessly transferred state between frontend and backend but I don't think it was a distributed system. I don't remember what it was called.

Writing APIs to glue together data fetching and actions and GUI state is all very siloed. If you could talk about the system as a whole including GUI interactions at the same time as system interactions that could be truly powerful.

Imagine multi *omnichannel* event streams that map to the users notifications, email inboxes, chat interface, post, deliveries, accounting, customer data, synchronisations, integrations, microservices and business CRM and ERP. Everything is linked together by powerful workflows. An interaction with a customer is just an extension of the system. It's a distributed system of human tasks as well as digital tasks and interactions between the customer and the company.

# 80. The Wiring shouldn't matter

What's important is the sequence of behaviours that should follow on from eachother.

# 81. Coordinates 

# 82. State machine GUI

Use the state machine syntax to define the behaviour of the GUI.

# 83. Community Idea: Fake the App

# 84. State machines in assembly, error handling and structure sizes and attacks 

# 85. GUIs at X11 layer

# 86. Refresh logic in everything, Promise Lattice

I read [this account on Hacker News about a GUI that was written in assembly](https://news.ycombinator.com/item?id=36153989) and it made me think of promises in GUI rendering.

# 87. Literal linear synchronized in memory buffers for everything (linear memory and execution)

Computers are linear with sporadic jumps. 

I don't know how it works: exceptions at the assembly layer.

# 88. Syscalls and function calls

# 89. What you see is how it is organised in the computer

# 90. Subscribe to blogger

# 91. Attention camping

Attention is extremely important and valuable in the internet world, it determines who you buy from and who you are influenced by. This idea is a website where you create a description of what you want attention for and then you camp (which means wait) for a match up with someone who wants to pay attention to it, based on a matching algorithm. When there is a group of 10 people who want to pay attention to something, it opens up the item and people can chat and interact on that item.

Centrally plan your attention based on what you want to pay attention to rather than browsing or doomscrolling.

Create an extremely deep profile of what you want to pay attention to, what you think is interesting and everything you find interesting.

We can use large language models to compare similarity of everyone's profiles with other people in vector/embedding space.

Create items that you want to share with others and when a critical mass of people reach the same item, then an item is created and everyone is notified that they want the same thing.

This is an asynchronous community, like email waits for someone to reply.

# 92. Offline IT, Designed to be down

# 93. The C/C++ project building approach doesn't work

You need to use Bazel or Buck or something serious to do anything properly.

# 94. Refresh rate GUI state

Creating GUIs is extremely difficult because of state management. If we express what the new state should be, a virtual DOM diffs it and decides how to make the old state match the new state.

# 95. Wait state deschedules

We want to avoid polling, so we have a wait command which deschedules the lightweight thread until it is finished. This is a bit like IO but results in a powerful direct style. This is similar to sleep but evented.

```
while True:
    events = event_context.poll();
    for event in events:
        case event.type:
            case TYPE_EVENT: // handle event
                event_context.add_wait("NEXT_STATE")
                
                
```

We can use promises or async await for this pattern!

# 96. Online multiplexing

The simplest multiplexing is a loop. But we can do it as an online algorithm and separated in time, across processes.

# 97. Constraints game

Rust lifecycles and borrow checker are rather complicated to learn.

# 98. Extracted pricing

Itemized pricing

# 99. Diagram the spirit of problems in language

# 100. Metaast

A Java solution to doing something in plain English of the problem to be solved looks different to the same in Rust.

Metaast is the creation of an AST of problems with a simplified configuration model that can transpile to Rust or Java.

# 101. Locks in state machine formulation

If these processes go in parallel:

```T
process-1 = action1 | shared_resource action2
process-2 = action3 | shared_resource action
```

They shall automatically be scheduled so that locks are around the things that need to be protected.

# 102. Parallel GUI visualisation

A GUI where you can see parallel state machines executing and interleaving.

# 103. Log hash

A loghash is a configuration that leads to the output of particular kinds of logs.

Can be stored in a text file and changed with command line tools.

# 104. Isomorphic state machines

This state machine formulation can be executed on the server, on different threads, on different servers as microservices, as different routes, as protocols, on the web browser and in Javascript workers, in WASM and the communication is handled for you, automatically.

```
```

# 105. Recursive descent parsing data fetching (ala GraphQL)

# 106. Composition of APIs

We can schedule behaviour by moving blocks of lexer tokens around

Need a GUI that looks like a Outliner that can move tokens and reorder them around. Can customise behaviour.

Parsing IS composition. Combine two libraries together with a lexer.

Tie together states in each application.

If I have the behaviour as token stream of two programs, then I interleave them, so I need elegant way to do concurrent programming and wait states between different behaviours of each part.

Substates of other programs behaviour, or instances of behaviour?

```
```

Logical clocks, causality marked by thread ID

# 107. Concurrency hoisting

I want to be able to write the following code, where I can include a blocking function anywhere, but it shall never block the event loop of the current thread.

```
hoist while (true) {
	batch = poll events
	for (item in batch) {
		switch (item.type) {
			case EVENT_A:
				blocking_function(); 	# <---- THIS LINE DOESN'T BLOCK THE EVENT LOOP
				call_function_after(); 	# <---- BUT THIS LINE HAPPENS AFTER
				break;
		}
	}
}
```

# 108. Parallel game engine

# 109. Golden concurrency

It should be possible to write to the same database from 3 processes all running as fast as they can without needing to separate the database into three databases and updating them separately.

# 110. Funding IT

# 110. Easy online

A way of configuring a server so it that can come online quickly and join the network.

Platform logic and my programming language and server software runtime should do this. Reliable autoconnect logic.

# 111. Overlaid chunking/buffers

Chunking can be overlaid some existing code for performance, without needing to redesign the underlying implementation.

If I have a complicated algorithm, how do I postprocess the code to add chunking? Do I insert loops everywhere?

# 112. Elastic hierarchies

A function that grows complicated graphs according to a progression, like a mathematical set.

This can be implemented to implement [ideas4 132. Revenue Scaling Plan](https://github.com/samsquire/ideas4#132-revenue-scaling-plan).

# 113. Implementation Freedom

Macros of AST transformation really are a way for implementation freedom, but what about orthogonality?

I talked about is assembly the lowest common denominator.

# 114. Unfair selects in Go

In Go there is a selector operator.

If I have events of different rates, I might want to define a SLA for processing events of each source, in effect I schedule the multiplexing of each channel. This is sampling.



# 115. Multithreaded Runtime architecture Asynchronous and Nonblocking runtime

How do you write a program that never blocks and where everything is asynchronous?

One approach is to separate control and work.

![NonblockingRuntime.drawio.png](NonblockingRuntime.drawio.png)

This design incorporates 3 layers of threads for non-blocking high performance. Nonblocking Ringbuffers are used everywhere.

* **App threads**: No IO or CPU is done in these threads. These coordinate IO and CPU use in the background to the application. They are not associated with a particular request but application state. Change detection happens here.
* **Control threads** This is where liburing or epoll is used. This is a simple routing dispatcher and no IO actually goes on.
* **CPU/IO Thread pool** Work actually happens here and communicates to the application with ring buffers or submitting IO requests.

This design would actually work in a programming language implementation interpreter. The worker thread pool can be sent the context of the function to be executed.

Need to work out how to combine the state machine formulation into this pattern.

# 116. Compatible types

# 117. Collection classes - what should the behaviour be when there's multiple?

Multiply/pluraize behaviour upwards in the stack.

# 118. Template pattern programming

I have a model of system that I want a programming language to compile into. How do I do this?

# 119. The architecture of a web server

The ergonomics of configuring a web server are interesting. Flask, express and Spring Boot take different approaches to configuring web server listeners. Spring Boot uses annotations, flask uses decorators and express uses function calls and callbacks.

I feel configuring a web server to route traffic to code is an information system problem. 

# 120. GUI Assurances

This should never overlap this.

# 121. Compiled dispatch rule engine in a web server

What should happen when.

# 122. Need a C API AST

I want to be capable of generating C code with an API.

# 123. Do nested expressions have value?

```
something(other(another()));
```

# 124. The data structure of code

# 125. Advanced flexible resolution

Resolution is such an underspecified thing. What does every package management solution do and build process look for things? 

* Puppet's Hieradata is an advanced resolution mechanism but is used for a specific purpose.
* C++ templates are a resolution algorithm

# 126. SIMD buffered request processing

If you have a number of requests by different users in flight, could you batch them up and process them with one thread using SIMD instructions?

# 127. Legalistic lens

Pay a company to handle the legal requirements of your solution.

# 128. Thoughts on boilerplate and plumbing

Every developers least favourite task is writing boilerplate and plumbing code.

# 129. Buyer pays IT resources

# 130. Main spider

Point a program at a codebase and see the code spider from the main method.

# 131. State machine formulation as log output

We can use the state formulation I defined in ideas4 [#558. State Machine Formulation](https://github.com/samsquire/ideas4#558-state-machine-formulation) as an output format for log lines.

# 132. Disk Split

# 133. Scalability pattern

# 134. The in-memory website

# 135. Module systems thoughts and Micromodules

Module size is important.

# 136. State machine Playground

# 137. Thoughts on marrying coroutines and threads, an underlying pervasive execution model

I enjoyed this post entitled ["Asyncio Thoughts by Charles Leifer"](https://charlesleifer.com/blog/asyncio/). Asyncio permeates through the entire codebase due to async functions. There must be a way of defining concurrency that is easy to understand and follow.

One or more things can go on at the same time, we want to pause when there is IO such as a disk risk or network call.

What do we want from lightweight processes or coroutines?

* explicit start/stop
* async/await
* yield
* wait for
* fork
* join
* structured concurrency
* continue on thread
* pause
* cancel
* schedule
* mutually exclusive scheduling
* binpack work

Coroutines either have an event loop or an event scheduling function, it's just hidden from the user. Coroutines at the assembly level have extremely more freedom than coroutines implemented in a high level language but the scheduler is much easier to write in a high level language.

It's interesting that the event scheduling function is an example of an online algorithm in the style of 142. Online (Nonblocking/Blocking) use-adaptive algorithms APIs.

Schedule functions change control flow completely, they effect the stack and what is returned to afterwards.

```
while (true) {
	for (Coroutine in coroutines) {
		run coroutine until yield
	}
}
```

"become" control flow (stack abandon, like a superpowerful goto) or shift reset in a high level language

```

```

# 138. Community Idea: Incremental code highlight

I want to see cut back summaries of how code achieves some purpose in a large codebase.

What does the code do to implement X behaviour?

# 139. Standard program designs

I often think of programs as loops.



# 140. Relationship of Turing tape placement and time with multiple actors moving about

# 141. Compute Autoscalability - Autobalancing actors

These are actors that are assigned ownership of a particular kind of object and service requests to that type of objects for a certain element of behaviour. If the requests to a particular key get hot, they are extracted to a thread. Then if that gets hot, they are extracted automatically to a server.

# 142. Online and Incremental (Nonblocking/Blocking) use-adaptive algorithms APIs

If you can design your code so that each part is online or single-shot, then you can use your code in any API integration. This is a style of coding that is nonblocking or blocking, selectively and incremental.

# 143. Rate batching - Would you pay latency for throughput?

If you're bottlenecked on synchronizations per second, such as in your IO response schedules work for a thread.

The event loop can submit ringbuffer events, but then we're synchronization bound.



# 144. Expected API surfaces

In a given piece of code, there's a set of API calls the host of the code expects you to call. What's appropriate when?

# 145. Opt-in Dependencies

Depend on properties

# 146. Sending execution state around, distributed promises

In a complicated distributed system it can be useful to send a execution state around and resume it on different machines.

* If we're using coroutines, we can store a point where we should jump when resuming from a yield.
* If we have promises, can we send promises around and have them resolve in any place?



For example, the following is approximate assembly for a jump table, which can be used to jump to a state once resumed on another machine.

```
.data
statetable     dq      state1, state2, state3            ; states
.code
jump:
lea     statetable,r9
main0:  jmp     qword ptr [r9+rax*8]
main1::
inc     rax
cmp     rax,3
jb      main0
state1:
state2:
state3:


```

# 147. Web request handling state machine

Can define URL handlers with state machine formulation:

/checkout = take-payment

# 148. Thoughts on Shift/reset continuation passing and ASTs

By the AST representing interpretor/execution state, we have extreme power over execution and control flow.

# 149. What is it good at/What does it do/What problems does it solve

When evaluating any technology or programming language, I think this is the most important thing to consider. 

# 150. High level APIs compiling to free form assembly

Need a high level beautiful API and some mechanism for it to be compiled to efficient assembly.

There needs to be a low level abstraction that can implement all the desired features of the 137. Thoughts on marrying coroutines and threads, an underlying pervasive execution model

# 151. Named stack

What's on the stack at any given point?

# 152. Keyframe, Data logistics code generation, Sliding image puzzle assembly code generation: Moving things around revisited, value calculus and boxes

We can use A* algorithm to generate assembly or high level function call code.

You give it memory and registers and it generates instructions that fulfil that state.

My example program takes the following input:

```
start_state = { 
  "memory": [
    0, 0, 0, 0
  ],
  "rax": 0,
  "rbx": 1,
  "rcx": 2,
  "rdx": 3,
  "rsp": -1
}

end_state = {
  "memory": [
    3, 1, 2, -1
  ],
  "rax": 3,
  "rbx": 2,
  "rcx": 1,
  "rdx": 0,
  "rsp": -1
}
```
And interpolates the instructions needed to get to the end state. This is the following instructions:
```
[start, mov %rcx, %rsp, mov %rax, (%rdx), mov %rbx, (%rbx), mov %rbx, %rcx, mov %rsp, %rbx, mov %rbx, (%rbx), mov %rdx, %rsp, mov %rax, %rdx, mov %rsp, %rax, mov %rax, (%rsp)]
```


Why is this idea so extremely powerful?

* **Value based programming** Most modern programming research is on types that variables take upon. I described value calculus in [ideas4 571. Value calculus variable tracing](https://github.com/samsquire/ideas4#571-value-calculus-variable-value-tracing)
* **Can prepare callsites programmatically** We don't need to arrange data fetching if the code to move data into place can be generated. 

This idea is inspired by the Myers algorithm which represents the inclusion of a character from a string as positions on a graph in two dimensions. We can represent values as objects on a graph that can be slid around to take different positions in registers or memory locations. This is how we can implement [#800. Data logistics plotting](https://github.com/samsquire/ideas4#800-data-logistics-plotting-or-the-stack-of-methods-is-a-data-structure-in-memory-and-can-be-manipulated-as-memory) This can be used to cause what we want to happen.



Each slide is a move or xchg instruction.

Trace of a value to a target location.

I want this method to be called with these arguments.

Stackless programming

Special understanding of rsp register.

can generate a yield instruction

We can define target states where things are where we want them to be. This takes advantage of human reasoning which is easier about causality. Things are where we can use them already.

How do we represent the causality of a stack?

coroutines are just moving things in and out of the stack to control control flow.

Moving things around to get the behaviour you want. Can we automate the binpacking of movements to generate algorithms?

We know if we move something here, it shall cause this to happen. Causality

We can use sliding image puzzle solving algorithms to schedule instructions 

we need to synthesise the exact steps to cause what we want to cause

it's all numbers at the end of the day, and assembly is just subtracting and adding numbers and moving them around

target state

puzzles, computer solving image puzzles

ensuring queues are empty when quitting

# 153. Fun crud

Crud should be fun.

# 154. Nested contexts:

My code often results in a large method that takes in many arguments.

is there a programming style that leads to elegant designs where there is relationships between different kinds of objects?

```
my
```

# 155. Tangledness - return in a loop

Exceptions in finally blocks 

# 156. Specify What must happen, be told about ordering issues

# 157. How do you know it's in synchronization?

# 158. Correlation of behaviour from logs

# 159. Stacks are trees

We want to add logic that needs data from elsewhere deep in the stack, how do you do it?

# 160. Program synthesis and search thoughts

My program synthesiser tries to infer the data flow through states, including hidden states such as function calls.

There is a map of available programs that have been written and their structure.

Suggestion

neighbours are iterators

We can see all existing programs as a progression of ordered method calls.

need to avoid creating states that are impossible to recover from

maximise future possibilities

lifetime of a state

generate multiple nodes in one batch

high dimension space

what's the high dimension space of a program?

the arrangement of most programs is the same

valid histories

parameter/calling convention passing, arranging things to be present in right places is pretty difficult

theme iterators

neighbours of a theme

formula for a graph, that most programs take on

ordering component

exclude what you just did

neighbour sequences, each thread tries different generators

threads move problem search space around

# 161. Active and selective logs

Turn logs on or off in a program at runtime, in console output.

# 162. Misses messages check

This has to be the most common bug in distributed and multithreaded systems. Wait state

# 163. Surfacing a fact

Might count something deep internals of code, but inefficient to do it on the hot loop

# 164. Multidimensional modelling

What would Blender look like for higher dimensions.

# 165. Forms are HTML files

Don't even need to generate HTML with values interpolated, just proxy the HTML file through a special function that inserts saved values.

# 166. Example invocations

Example invocations are the most useful documentation.

# 167. Useful library gallery

My A* algorithm for generating code from placements.

# 168. REPL+CRUD - Turing machines are not where we specify things, queries are, REPL to query

Turing machines REALLY are the wrong place for specifying things because they are so rigid, specific and hard to optimise.

Queries are different to Turing logic.

Imagine a web based GUI that allowed objects to be created, edited, reordered and sorted and organised. Every part of the system is a collection that can be edited and queried, inserted and appended and reordered. REPL+CRUD combines a data collection editor with a REPL and REPL commands against those objects can be executed.

There is an implementation that does what it is meant to do. Can the implementation be applied to a different data model and data sources? 

```
for item in items:
	tax = calculate_tax(item)
```

We can implement **stretch logic** which is similar to a branching library. If we want to stretch some REPL based code to another model of something different. For example, we want to stretch it over a GUI.

```
<input type="text" value="{{ tax }}">
```



Optimisation work. We use the relations of things. Pushdown automation.

Turing machines and declarativeness

# 169. Hinge logic

Postgres is considering/proposing moving from its process orientated design to a thread orientated design.

Everything hinges on this logic. Postgres is an enormous codebase and there's no metadata about what the code is doing.

# 170. Programming languages are the wrong place for ontologies

C++ and Scala and Java all try use the programming language to implement an ontology of data structures.

# 171. Coding Topic and callsite databases

Refactoring would be easy if every piece of code was assigned to a topic and that topic was actually a serialization of an idea.

# 172. Markdown GUIs

Adapt a markdown renderer to render GUIs

# 173. Information synchronization

users entering payment details, synchronizing with bank, anti-fraud systems

# 174. The platform should provide the polish

It takes extreme amounts of effort to create a desktop, web application that is beautiful and useable.

# 175. Event loops thoughts

I was reading about Jetbrains Noria and it talks about its event loop.

# 176. How to compiling processes down for efficient execution

* orthogonality to an event loop and assembly
* an event loop is an interpreter, a loop to a instructions is a compiler
* Query engines deal with relational data, or iterators as in the volcano model, but what if we have a model of what should be done, how do we execute it efficiently.
* An event loop is how it gets executed, but what does it look like if it were compiled to assembly, or events?
* Moving around iterators is how you improve performance.
* Effects of an iterator, same effect, compatibility
* C++ parallel iterators and algorithm iterators
* Compiling down to assembly
* O notation
* generalisation of looping
* cardinality
* loop rotation
* 
* loops are definitional, and cheap because they are relations, not logic

How do you shift iterators around, or hoist them for efficiency? It's loops all the way down!

```
for item in a:
	for item in b:
		for item in c:
			do_something()
```

this is equivalent to - just in a different order.

```
for item in c:
	for item in a:
		for item in b:
			do_something()
```



# 177. Infer function application

Change the effects, change the logic, change the log, change the behaviour

# 178. Program synthesis backwards search

We can search backwards to the origin and forwards from the origin to the destination.

# 179. The Product is a number of requests per second

| Requests per second | Price |      |
| ------------------- | ----- | ---- |
| 100                 | $1    |      |
| 200                 |       |      |
| 1000                |       |      |
| 10000               |       |      |
| 25000               |       |      |
| 50000               |       |      |
| 100,000             |       |      |
| 1,000,000           |       |      |

| Concurrent users | Price |
| ---------------- | ----- |
| 1                | £1    |
| 10               |       |
| 25               |       |
| 50               |       |
| 100              |       |
| 1000             |       |
| 10000            |       |
| 20000            |       |
| 100000           |       |
| 150000           |       |
| 500000           |       |
| 1000000          |       |

| IO per second | Price |
| ------------- | ----- |
|               |       |



# 180. Exhaustive state machines and error and state handling



# 181. 2000 line project

# 182. Simulate the journey of a request

For 100,000 requests per second



# 183. Database query engines as scheduling

# 184. Do you want to really want configure with a programming language?

Vimrc is a command language, not a programming language, Xmonad configuration file is a Haskell file. Do you really want to program to configure something? Sometimes you do, sometimes you just want to make an asssertion.

```
only(1, X)
```

I feel generating configuration is really helpful from a programming language, generating data. But connecting data together is something that GUIs are better at.

# 185. Scaling examples and scaling programming

If a lot of people come up with examples, can we infer the result?

# 186. Behavioural percolation

If I take some gold with soil and filter it in a grilled pan, it shall percolate due to gravity through the holes.

This idea is an idea how to generate complex structural changes to code. For example, if our existing code is socket per thread, how do we change it to be multiple sockets per thread?

We insert a loop and call the behaviour in a loop.

```
int socket = accept()
ClientThread clientThread = new ClientThread(socket);
clientThread.start();
```

And I want to transform it to:

```
ClienThread:
	while True:
		for connection in connections:
			int messageType = socket.readInt()
```

Moving behaviour to a different place, what's the path to the desired behaviour, we can use graph finding to find the traversal to the desired behaviour.

Structural boilerplate generation

behaviour percolation numbers, structures built up



# 187. Nondeterminism testing

# 188. Declarational imperative code

Code that isn't executed as-is but creates relations between things, where it shall be filtered down into evaluable code. Similar to functional programming. Mainly applied to loops.

still need to work out how to use prolog to solve logical problems, ontologies, CRUD for system, different kinds of things

concurrent prolog, logic used to solve problems 

# 189. Code hide

Hide irrelevant details from the happy path.

# 190. Mapping high level behaviours to imperative code API function usage

I was reading Postgres sourcecode `postmaster.c` and it talks about how it `forks` to handle requests.

Fork wouldn't be such a bad API if it was not inefficient!

# 191. Program knowledge

# 192. What lines of code have been executed and scroll through them all

# 193. Desired behaviour optimisation API and environmental knowledge

Can the following API be transformed into threads?

```
accept();
fork();
```



# 194. Event loop compiler and replay -able determinism

 a bit like rr and Microsoft Coyote and Vale programming language 

# 195. Refactoring and code generation 

What is it the thing you are you refactoring? Surely it's output, an output of something? It's an output of what the behaviour should be.

If a program that is NOT refactored and there is a program that IS refactored but the behaviour stays the same, what is the code that you are refactoring? Surely the refactoring could be automated?



Process orientated shared memory complexity



# 196. Complex codebase

What is behaviour

anic, prolog processes

#  197. Imaginary API

# 198. Boundary pass

Data flows through a boundary (a hierarchy of structure), we can do something with it. Can this be used to solve N+1 queries?

N+1 queries 

Write code to understand locks

# 199. Beginning and end

An API is easier if we delineate beginning and endings. This is what python context manager does.

# 200. Plot work

# 201. Behaviours and configuration of them

I think this is an enormous problem of computing. A program exhibits behaviours, but configuration of the program is really difficult to define or change without lots of specific hook code.

# 202. Organisational problems

Package management, code layout and structure are all inherent problems of programming.

# 203. Most Rust and C++ programming is working around imposed ordering limitations that nobody writes down or talks about



# 204. 3D ROOM

I think people assume that a 3 dimensional GUI requires movement around, but we can immediately move the view instead. Depth provides useful information.

# 205. State machines and process management, interlocking recoverable states on retry

Any IO creates state that is external to the system that is being written and this state can prevent the program's internal state machine from moving forwards. There's a direct mapping of state machine status and process. We should be capable of promising future states.

# 206. High level definitional

Imperative code as definitional - not literally executed as-is.

# 207. Incremental rerunning - Infer it shall never change

The cheapest refresh logic is to simply re-run everything, but this is really inefficient. When do you need to rerun something? When it has changed. How do you detect it has changed?

# 208. Animation timeline rendering would be useful for scheduling problems

# 209. Method calls and behaviour

Multiple method calls work together to provide behaviour.

# 210. What's the difference between code that works and code that doesn't work?

# 211. Execution in Assembly is just moving through numbers

Algebraic effects



# 212. RETE, crystallisation of order, dispatch and code layout

RETE is awesome. RETE can be used to generate code.

The complicated part of programming is the definition of rules.

Jump hierarchies are slow, when I think of assembly, it is just jumping around!

# 213. We need to decouple definition from "how"

# 214. Scenario editor

# 215. Unlimited scalable design



# 216. Changing a number changes the course of future actions in assembly, movement through code

# 217. Scheduling runtime foundations shouldn't be executed as-is

I see examples of async runtimes where delays are implemented as Thread.sleep. I think the runtime should abstract away the execution of delays from the execution of code like Temporal. Blocking should never happen!

# 218. Dataflow between threads

# 219. Mini codeflows diagrams

Parse sourcecode, create cut-down diagrams of code calls flowcharts.

# 220. LINQ rewriting

# 221. React! Handle all cases

# 221. Moving blocks programming

# 222. Dynamic Table programming, Just a grid, data structure visualization and serialization format

We can change the columns or rows of a grid at runtime! It doesn't have to be static. A tree or graph maps to a table and the table can be interactive.

| Root | Children | Children |
| ---- | -------- | -------- |
| 1    | 1        |          |
|      | 2        |          |
|      | 3        |          |

 We can create object graphs from as serialization format of a table.

# 223. Thoughts on scrolling

# 224. Colours of things pattern matching

# 225. Flow chart error handling

Trampoline to retry.

# 226. Wrong dense

C++ and Rust are the wrong density.

# 227. If that was there, where would it go if I did this? Multirelvis

rotate meanings

# 228. Contexts, behaviour and OOP and imperative code

I want:

* to write imperative code to coordinate behaviour of objects?
* customise interactions between objects
* what if I want an object method to return something?
* programmed interaction sequences
* can record message playback and play at a different time
* coroutines OOP



# 229.  Message passing GUIs are slots backed by pipelines

# 230. Standard cycle and the state grid

Every action changes the state of everything, a 2D grid of changes through time.

Each line of code is a state transition of the entire state grid.

List all the state changes every object should have.

Line up state grids.

# 231. Every object is duplex

# 232. Delayed execution, Using flags when we want to write imperative code, turn imperative code into flags or types/sum types automatically

# 233. Useful portals

I loved Excite.com and Lycos and Yahoo! when they were portals and had portlets. They were valuable.

# 234. Can detect the absence of behaviour by incrementing when an object is reviewed

# 235. Societal rule engine is what people should be using

# 236. Local variables are a struct

# 237. Re-entrant future behaviour code

It is often useful to stagger control flow over the future.

I often find I want to do a sequence of actions with a series of future states, I usually use a boolean to do this logic. (A relevant idea is ideas5 232. ) Instead, I want to define behaviours that should happen in the next call to this function or next calls to other objects.

You can think of this as interlocking future state of calling this method. States that line up, re-entrant code. Multiple invocations between this control flow and the following control flow. Reentrant continue. Wait for future states

```
on_click:
	if state == UNMARKED:
		mark_item()
		on next on_click:
			after render:
				// something done after render
		
    
```



This is a code transformation that makes code easier to follow.

Don't need to move code to start of handler

# 238. Log folders

I want all the logs of this log line together, so show me the logs out of order.

# 239. Event runtime

A high level abstraction for the [samsquire/ideas4 558. State machine formulation](https://github.com/samsquire/ideas4#558-state-machine-formulation) and [samsquire/ideas4, 526. Multiplexing setting format and routing operation](https://github.com/samsquire/ideas4#526-multiplexing-setting-format-and-routing-operation) is to use events.

We can use ringbuffers and lightweight threading.

# 240. The Permanent Website

Fund for the next 25 years.

# 241. Pull-site

An alternative to federation. You pull content from other users.

# 242. Pipeline server

Rather than run a separate database, log server (such as Kafka) and GrapQL, we define our infrastructure as a task pipeline.

# 243. Movement programming

Most programming languages work by providing instructions that operate on state or function parameters to return new values or new states.

Movement programming is different, in movement programming we see what we have available and then move it somewhere, like a Rubik's cube.

dynamic table programming

```
highlight table cells when mouse over them
table cell selected for move
switch view to clicked item
update columns and row to data of data structure
click new destination to place data
```

# 244. Contexts are where callsite parameters come from

Methods don't take parameters

```
context:
	variable = 1
	do_something
	subcontext:
		variable = 6
		do_something
```

# 245. Understandability Kingdoms

# 246. Functions are kind of strange

They take in data as arguments and control flow jumps somewhere to do something with it.

# 247. Slots state change visualisation

Like a slot machine but each cylinder is a sequence of states.

# 248. Flat code

# 249. A shell that is also a pipeline server and task system

# 250. Types as states, states are the more interesting types

States can describe behaviour sequences.

State grids can transform entire collections of objects into different states.

# 251. Robust code: Limited and separate straight line control flow selections

Divergences to happy path, can be retried to get to happy path.

# 252. Happy path state machines: parsing and how it relates to control flow of state machines (train track rendering)

Parsing algorithms used for AST generation can be used to create control flow execution state machines.

Take this mathematical expression:

```
2 + (3 * (8 - 9))
```

Its parsing AST tree looks like this:

```
  Add
2    Mul
    3   Subtract
       8    9
```

Its state machine looks like this though:

```
Subtract | Mul | Add
```

If we put an if statement in the expression, the state machine diverges, but we want to keep the number of states on a happy path.

```
  Add
2    If
   < 0 Mul          Mul
      3 Subtract   4   Add
           8   9      8   9
```

We want to join after the If to the rest of the state machine as soon as possible. The two branches of the if statement:

```
Subtract | Mul | If | Subtract | Mul
Subtract | Mul | If | Add | Mul

```

Now if we replace the`If` with a function instead that could return a number of different states or did IO like a Monad.

```
Subtract | Mul | Function
```

Control flow and state diverges from this `Function`

```
Subtract | Mul | Function | State1
Subtract | Mul | Function | State2
Subtract | Mul | Function | State3
Subtract | Mul | Function | Error1
Subtract | Mul | Function | Error2
Subtract | Mul | Function | Error3
```

How do we get the control flow on the happy path again? And how do we reliably test and retry errors?

So this state machine is like a parser where the next state can be any of the optional states. Will be evaluated in a certain order due to the pratt parser.

Take this definition of an SQL SELECT query from the PostgreSQL documentation. Each thing inside square braces is optional, but could be present.

```

SELECT [ ALL | DISTINCT [ ON ( expression [, ...] ) ] ]
    [ * | expression [ [ AS ] output_name ] [, ...] ]
    [ FROM from_item [, ...] ]
    [ WHERE condition ]
    [ GROUP BY [ ALL | DISTINCT ] grouping_element [, ...] ]
    [ HAVING condition ]
    [ WINDOW window_name AS ( window_definition ) [, ...] ]
    [ { UNION | INTERSECT | EXCEPT } [ ALL | DISTINCT ] select ]
    [ ORDER BY expression [ ASC | DESC | USING operator ] [ NULLS { FIRST | LAST } ] [, ...] ]
    [ LIMIT { count | ALL } ]
    [ OFFSET start [ ROW | ROWS ] ]
    [ FETCH { FIRST | NEXT } [ count ] { ROW | ROWS } { ONLY | WITH TIES } ]
    [ FOR { UPDATE | NO KEY UPDATE | SHARE | KEY SHARE } [ OF table_name [, ...] ] [ NOWAIT | SKIP LOCKED ] [...]
```

Each optional thing must change control flow when executed.

We can define control flow with parsing technologies for elegant and understandable execution of control flow.



# 253. The algorithm is just a loop or even an event loop or AST evaluation

Even databases are just loops ultimately.

# 254. Community Idea: Vote on Value

# 255. Dream Dependency Need table

This is inspired by Scrapscript and Val town. These are my dependencies for imaginary software.

| Dependency name            | Description |
| -------------------------- | ----------- |
| create-email               |             |
| create-file                |             |
| create-tls-connection      |             |
| create-tcp-connection      |             |
| create-https-connection    |             |
| create-http-connection     |             |
| create-postgres-connection |             |
| create-sqlite-connection   |             |
|                            |             |

# 256. 2 phase commit and thoughts on just updating everything in parallel

# 257. Data flow between collections

# 258. What doesn't matter to your business logic

Why IT projects are so slow.

# 259. Wire Grid Configurator: Describe something and Interleaved behaviour

Activations along wires in a grid, like Orleans. Talk about everything in terms of everything else.

# 260. Parallelism in ASTs

Represent coroutines and threads as sibling nodes on a graph.

```
p = producer
c = consumer
p -> c

(let [p producer c consumer]
	(parallel
		p -> c
	)

parallel for 
```



# 261. Parallel data/behaviour flow



# 262. Movement and parallelism

If we move things around, we can move things around in parallel.

# 263. Lock turn-taking distribution



# algorithm crystallization

Loops are preparsed into AST and optimised into equivalents.

 

# data flow machine

flowcharts are fun

Arrange dataflow through code that is in columns and wire it up.

# 264. Processes (control flow) are data

We can model processes or control flow as a data stream.

# 265. Types are about control flow and dispatch and its link to advanced resolution, serialization

When there is a dispatch decision, we need to do an advanced resolution and simplify the resolution callsite. Serialization of types at runtime.

# 266. Java's verbosity is caused by the lack of an advanced resolution algorithm

FactoryFactoryFactory is a recurring thing that occurs with Java, due to the lack of overridability.

# 267. Standardised generalisation

We generally want to generalise with the same approach, perhaps a parameter passed in.

# 268. Writing a loop over an existing program's behaviour, a representation of behaviour for extensible and overridable behaviour

Writing a loop over the existing program's behaviour.

Coupling/uncoupling



Deciding control flow in the future.

# 269. How to understand any codebase at a glance, case based programming

Render the codebase control flow graph to pipe separated state machines (State machine formulation)

# 270. Pipeline syntax and a syntax for hooking into pipelines events

```


pipeline = one | two | three | four | five
pipeline.start()

# pipeline.start:

```

# 271. Task protocols

Two or more programs talking to each other is a protocol. This is a control flow technique too but is linked to parsing. Methods can pass variables between themselves and call code in the other side.

In this example, the lexer function emits "emit_character" events. Tokeniser emits "new_token" events and parser emits "emit_ast" events.

```
task lexer():
	for each character in program:
    	lexer.emit_character(character)

task tokeniser(emit_character):
	while character in emit_character:
    	if character == "\n" or character == " ":
    		continue
        if character == "{":
        	tokeniser.new_token("opencurly")
        if character == "}":
        	tokeniser.new_token("closecurly")

task parser(new_token):
	
	while token there is new_token:
   		if token == "opencurly":
   			tokens = []
   			while token there is new_token:
   				
   				if token == "closecurly":
   					parser.emit_ast(tokens)
                else:
                	tokens.append(token)

lexer = lexer()
tokeniser = tokeniser(lexer.emit_character)
parser = parser(tokeniser.new_token)
```













I need to write a parser for C and look at analysing Postgres sourcecode or something.
