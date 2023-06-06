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
* 



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

# 104. Isomorphic state machines

This state machine can be executed on the server, on different threads, on different servers as microservices, as different routes, as protocols, on the web browser and in Javascript workers, in WASM and the communication is handled for you, automatically.

```
```

# 105. Recursive descent parsing data fetching (ala GraphQL)

# 106. Composition of APIs

Parsing IS composition. Combine two libraries together with a lexer.

If I have the behaviour as token stream of two programs, then I interleave them, so I need elegant way to do concurrent programming and wait states between different behaviours of each part.

Substates of other programs behaviour, or instances of behaviour?

```
```

Logical clocks, causality marked by thread ID

# 107. Concurrency hoisting

I want to be able to write the following code, without blocking the event loop:

```
hoist while (true) {
	batch = poll events
	for (item in batch) {
		switch (item.type) {
			case EVENT_A:
				blocking_function(); 			# <---- THIS LINE DOESN'T BLOCK
				call_function_after(); 			# <---- BUT THIS LINE HAPPENS AFTER
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

# 112. Elastic hierarchies

A function that grows graphs according to a progression, like a mathematical set.

# 113. Implementation Freedom

Macros of AST transformation really are a way for implementation freedom, but what about orthogonality?

I talked about is assembly the lowest common denominator.

# 114. Unfair selects in Go

In Go there is a selector operator.

If I have events of different rates, I might want to define a SLA for processing events of each source, in effect I schedule the multiplexing of each channel.

# 115. Multithreaded Runtime architecture Asynchronous and Nonblocking runtime

How do you write a program that never blocks and where everything is asynchronous?

One approach is to separate control and work.

![NonblockingRuntime.drawio.png](NonblockingRuntime.drawio.png)

This design incorporates 3 layers of threads for non-blocking high performance. Nonblocking Ringbuffers are used everywhere.

* **App threads**: No IO or CPU is done in these threads. These coordinate IO and CPU use in the background to the application. They are not associated with a particular request but application state. Change detection happens here.
* **Control threads** This is where liburing or epoll is used. This is a simple dispatcher and no IO actually goes on.
* **CPU/IO Thread pool** Work actually happens here and communicates to the application with ring buffers.

This design would actually work in a programming language implementation interpreter. The worker thread pool can be sent the context of the function to be executed.
