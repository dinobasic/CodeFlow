CodeFlow
========

CodeFlow is a JavaScript app intended to show how the various components of a code are linked together.

It is intended for the analysis of JavaScript and Java code only. It is still experimental, in the sense that is isn't yet clear whether the approach it takes (described below) does indeed help the software developer to better perform. That's why its usage shall decide on that matter.

At one point in their career, every software developer is confronted with the situation where he has to understand someone else's code. Assume he has to take over an entire Java program, with a user interface, and he gets to solve a a bug case concerning some kind of exception. The Java stack trace will allow to locate the source of the exception. The developer has to figure out why this certain pieace of code throws the exception. How and why does it come to that ? A good tool for understanding such things are breakpoints. Breakpoints will show the route the program is taking to get to a certain point and the state of its variables/attributes at every step. But it does not show you all the possible routes leading to that point, which is important because if we bring changes to our code, it is important know if other parts might be affected.

The aim of CodeFlow is to visually show how the various components of a code are linked and thus thus to more easily identify all the routes leading to a given point. Currently, it only takes into account method/function and attribute/variable usage (it does not for instance consider conditions and loops). This way, we can know if the piece of code we want to change to fix our bug, might affect other parts.
