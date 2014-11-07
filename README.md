What it's not:
 * Outside-in vs Inside-out TDD
 * DDD
 * Top-down vs bottom-up
 
Issues to reference:
 * Pattern abuse
 * Missing the domain
 * Building programs from the requirement and not from how we see the requirement
 * We tend to immediately pigeonhole problems into familiar patterns - this is bad and causes bad abstractions (pattern-driven rather than domain-driven)
 * Apache HttpClient 4 as an example

---------

How would you build a new system? "I would use Scala. And Spring. Maybe Netty. Definitely throw in some Factories. And DAOs. Everyone needs them. "

But what we're missing here is "what does it do? What is it for?"

Is your codebase full of classes containing pattern names? Do you have CatController, CatService and CatDao? If so, you're most likely focusing on patterns, yielding mechanical abstractions, while completely missing a semantical abstraction that yearns to be carved out. 

----------

Each layer of the system should expose its own language that abstracts over lower-level concerns. This language is the semantical abstraction. 

----------
http://taskinoor.wordpress.com/2011/09/21/the-abuse-of-design-patterns-in-writing-a-hello-world-program/
http://c2.com/cgi/wiki?DesignPatternsConsideredHarmful
http://programmers.stackexchange.com/questions/35755/overused-or-abused-programming-techniques
http://programmers.stackexchange.com/questions/49379/when-should-i-use-and-not-use-design-patterns
