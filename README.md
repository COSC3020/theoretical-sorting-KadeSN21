# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

Being that we cant see the source code, deciding if this algorithm runs in $O(n)$ might be harder to decide than if we could look at the source code, however we can test the algorithm with various inputs that will give us hints as to wether the algorithm actually runs in $O(n)$ time or not. 

The first test would be to run the algorithm with various input sizes to see if the time taken to sort the input list is linear to do this, we can pass arrays with $10^k$ elements, where k = 1,2,3,..., and plot the runtime of the algorithm relative to n, if the runtime seems to grow linearly, it would lean twards a $O(n)$ complexity, however it may also resemble $O(log n)$ time, or another patter that would suggest otherwise. Another test would be to give this algorithm different forms of sorted lists(reversed, random, in order, etc) to see if the creator could have possibly assumed lower bound $/Omega$ and mistakenly marketed the algorithm as $O(n)$, when $n$ is the best case instead.

Theoretically speaking, this is not possible due to the nature of sorting algorithms, as comparisons between elements must take place, and for a $O(n)$ time complexity to become reality, the elements would only be compared once, which would violate the $/Omega(n log n)$ lower bound places on comparrison based algorithms by mathematical limitations.

Help: I reviewed the course lecture videos.


“I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.”
