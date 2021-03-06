# Writing Efficient Codes

## Common things to include:

	Storing data that has already been calculated to avoid calculating it again.
	Using the right data structures.
	Reorganizing the code to ensure that the computer can remain busy while waiting for information from slow sources like disk or over the network.

## Profiler
A profiler is a tool that measures the resources that our code is using, giving us a better understanding of what's going on. In particular, they help us see how the memory is allocated and how the time spent.
Because of how profilers work ,they are specific to each programming language.So we would use gprof to analyse C program but use the c-Profile module to analyse a Python program. 

## Using the Right DS

	Since the dictionary stores key value pair, we can find a value in one operation, however for list we will have to iterate through the list.
	Using a dictionary  to repeatedly look up data will take a lot less time compared to list.
	Creating copies of structures can be  really expensive, therefore we should really check if that is needed.

## Avoid doing operations inside a loop
	If you need data from a file, parse it before loop and store in appropriate ds and then use that DS inside loop. This will save a lot of resource as you will not be parsing again and again.
	If you are reading data, read it outside the loop.
	Break out of the loop once you have found out what you are looking for.

## Keeping Local Results
	Use local variables wherever possible.

## References:
	- https://wiki.python.org/moin/PythonSpeed/PerformanceTips#Local_Variables
	- https://stackify.com/20-simple-python-performance-tuning-tips/
