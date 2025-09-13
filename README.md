# Radix Vs Quick

Well, the title gives away most of the parts of this project. Here, we want to compare the two sorting algorithms, **Quick Sort** and **Radix Sort**.
<br><br>
1) **Quick Sort:** \
Most of us here might be knowing what is Quick sort. Here is a briefing anyway. In Quick sort, we proceed with choosing a 'pivot' in the array (mostly the middle, or a random element). Then, we move all the rest of its elements in such a way that all the smaller ones are on the left side of pivot, and the larger ones on its right side. Then, we sort the left and right sub-parts (recursive algorithm), and return the final array.\
This algorithm has the O($n$ $\log$ $n$) time complexity, which is the best possible complexity for a sorting technique (can be proven using an inverted trees structure for combinations of array).
<br><br>
2) **Radix Sort:** \
If we already have the best algorithm to sort, why go further, right? Well, it turns out, like in most other cases in life, that if the situation satisfy some special conditions, then we can do even better. Here, the special condition is that if `the size of array is huge, but the number of elements constituting the array is much small`. In simpler terms, if $n$ is the size of array, and $m$ is the number of unique elements in the array, then space complexity of sorting such an array using Radix sort will be O($nm$).\
We should pause here and realize this fact properly. Note that for a fixed $m$, and for a large enough $n$, we will eventually have $m$ $<$ $\log$ $n$. Thus, Radix sort is expected to outperform Quick sort in the long run.
<br><br>
In this project, we will conduct experiments to see for which cases Radix sort turns out to be better than Quick sort, and where the case is reversed.
