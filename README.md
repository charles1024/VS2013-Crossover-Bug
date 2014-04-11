VS2013-Crossover-Bug
====================

A bug in visual studio where one instance of VS will run the code in another instance.

I have two copies of the same solution, which I will refer to as Hello1 and Hello2.  

Hello1 has a line in Default.aspx that will set the text of a label (lblHelloWorld) to “Hello World”.

Hello2 has this line, but it is commented out.

Steps to reproduce (important to follow exactly):
1)	Open the solution in Hello1
2)	Start debugging Hello1
3)	Observe that in the upper left there is a label with the text “Hello World”
4)	Stop debugging Hello1
5)	Open the solution in Hello 2
6)	Start debugging Hello1 again
7)	Observe that “Hello World” no longer shows up in the upper left.

Can this be fixed by changing a setting somewhere or is it actually a bug?  Are there any workarounds?
