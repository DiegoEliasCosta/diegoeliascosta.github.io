---
title: "Selecting Efficient Data Structures"
header:
  #image: /assets/images/bio-photo.jpg
  teaser: ""
  #assets/images/bio-photo.jpg
 #classes: "wide"
---

Data structures are the bread and butter of computer programming. 
Almost every Computer Science (or similar) course teaches Data Structures and Algorithms in the first semester of their program, given how fundamental data structures are for developing effective programs.  
And yet, the suboptimal selection of data structures is a major source of real performance inefficiencies. 

### Why is this a problem?
Let us take a very simple example of performance inefficiency caused by collections. 
We all know we should avoid using `array lists` in an algorithm dominated by element search, and still, this is a frequent issue in Java programming.
There are several possible explanations for these inefficiencies:

1. High-level abstraction fools the best of us. In Java collections, `ArrayList` provides the convenient method `.contains` that performs the element search in a single method call. It makes perfect sense to search for an element is lists sometimes (e.g., the list is small and search is performed infrequently). Performance, however, is a problem of scale. Once the program is in production and the list starts growing, that high-level method will charge the price for its convenience. 
     
2. Projects evolve. "I selected a list for this use-case, but at that time, that was no requirement of searching for elements". As projects start to evolve and new requirements pour in, developers have to refactor the code to better accommodate the evolution of the software. The problem is, sometimes, this refactoring never happens.    

3. Real application workload is hard to grasp. Developers have their expectations on what the workload the program their develop will 

### Our research

We have investigated how developers use Java Collections in their programs.