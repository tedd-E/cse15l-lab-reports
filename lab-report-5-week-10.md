# CSE15L Lab Report 5
Written by Kai Lee

This report will examine differing tests from two different implementations of markdown-parse, the [provided version](https://github.com/ucsd-cse15l-w22/markdown-parse) and [my version](https://github.com/tedd-E/markdown-parse), and identify their bugs.

First, we find two files to serve as our test cases. We can do so by running each version of markdown-parse, and storing and comparing the results by writing the output to text files and calling the ```diff``` command.

Here, the output of the provided implementation is stored in ```providedresults.txt```, and the output of my implementation is stored in ```myresults.txt```.
![img](lab5img/1.PNG)

Running the ```diff``` command gives the resulting output. Since there are a lot of differences, I'm going to randomly select the first two differences, on line 212 and line 230 to analyze closer.
![img](lab5img/2.PNG)

## Test 194
The first file I'll analyze across the two implementations is ```194.md```. 

My implementation output:
![img](lab5img/3.PNG)

Provided implementation output:
![img](lab5img/4.PNG)

We take a look at the original contents of ```194.md``` to see the following:
![img](lab5img/6.PNG)

Running the original contents on the [Commonmark Demo site](https://spec.commonmark.org/dingus/) shows the following output:
![img](lab5img/7.PNG)

It can be seen that the output of the official demo site doesn't match the output of either implementation we ran. 

## Test 201