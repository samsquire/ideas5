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

# 44. Reverse log to AST tree

Log to reverse tree to work out logic order.

# 45. Coordinated runtimes

After looking into liburing, it occurred to me that behaviours of systems should be generalised for the best possible performance.

# 46. It's impossible to segfault if we know the range of what is valid

Because you import what you use and what you expect to be where and what you expect each data structure to contain. It's not possible to dereference a value to an invalid piece of memory.

Parsing associated with blocking.

# 47. Can we infer the movement through instructions?

# 48. Monetisation system

# 49. Complete program, separated into pieces, re-stitched together into new program

Imagine you have a complete program that does a task and we want to do a variation of what the existing program does. We can do a simple transformation to get the program into a form that we can extend:

* inline all internal methods until only platform calls exist
* label parameters that pass through the program through to these platform/system calls.
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

With stateful programs, it can be difficult to reason about them when there are interactions between different actors or nodes. This idea is that we represent all states as circles, which always progress forward. We define circles for each actor and circles for overall progress. We link circles together which form valid pathways of execution.

* Any progression backwards is an invalid state, which means there is a bug in the program.
* An unexpected state change is a bug.
* Numbers that increment are new states.
* Trapped state detection: No path of state associations back to the global circle, so it's impossible for the circle to move forward.
* You must write a determine state function to determine the facts about the system at the current time. Concurrent events are represented
* Can create incremental state machines which are snapshots of valid cases, which are stitched together.

For example, we want to schedule two actors, A and B: ABABABABAB,

No matter what interactions with other objects, all circles shall turn forwards.

Must define your state machine as a circle, for each actor. This syntax defines a circle for the global progression of states and individual objects.

The "dot" symbol is a "join" from one state to another state.

```
global = actor(A).scheduled actor(!A).not_scheduled | actor(B).scheduled actor(!B).not_scheduled | regenerate

actor(A-B) = scheduled submitted++ | submitted == total | completed reset submitted = 0 | not_scheduled
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

