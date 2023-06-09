Download Link: https://assignmentchef.com/product/solved-605-202-project4-sort-comparison
<br>
This lab assignment requires you to compare the performance of two distinct sorting algorithms to obtain some appreciation for the parameters to be considered in selecting an appropriate sort.  Write a <strong>Quicksort</strong> and a <strong>Heap</strong> <strong>Sort</strong>. They should both be recursive or both be iterative, so that the overhead of recursion will not be a factor in your comparisons.  In this case iteration is recommended, but you are free to choose recursion. <strong><u>Be sure to justify your choice</u> <u>in your analysis.</u>  </strong>Also, in your analysis, consider how your code would have differed if you had made the other choice.

A <strong>Quicksort</strong> (or Partition Exchange Sort) divides the data into 2 partitions separated by a pivot.  The first partition contains all the items which are smaller than the pivot.  The remaining items are in the other partition. In the analysis, be sure to comment on your choice of an iterative or recursive version of quicksort. You will write four versions of Quicksort:

<ul>

 <li>Select the first item of the partition as the pivot. Treat a partition of size one and two as a stopping case.</li>

 <li>Select the first item of the partition as the pivot. Process down to a stopping case of a partition of size k = 100. Use an insertion sort to finish.</li>

 <li>Select the first item of the partition as the pivot. Process down to a stopping case of a partition of size k = 50. Use an insertion sort to finish.</li>

 <li>Select the median-of-three as the pivot. Treat a partition of size one and two as a stopping case.</li>

</ul>

<strong>Heap Sort</strong> is a practical sort to know and is based on the concept of a heap.  It has two phases: Build the heap and then extract the elements in sorted order from the heap.

Create input files of four sizes: 50, 500, 1000, 2000 and 5000 integers.  For each size file make 3 versions.  On the first use a randomly ordered data set.  On the second use the integers in reverse order.  On the third use the

integers in normal ascending order.  (You may use a random number generator to create the randomly ordered file, but it is important to limit the duplicates to &lt;1%.  Alternatively, you may write a shuffle function to randomize one of your ordered files.)  <strong>This means you have an input set of 15 files plus whatever you deem necessary and reasonable.  </strong>The size 50 files are to be turned in.  The other sizes are only for timing purposes.  Your code needs to print out the sorted values. Files are available at on the course web page if you want to copy them. Your data should be formatted so that each number is on a separate line with no leading blanks. There should be no blank lines in the file. Each sort must be run against all the input files.  With five sorts and 15 input sets, you will have 75 required runs.

Your program should access the system clock to get some time values for the different runs.  The call to the clock should be placed as close as possible to the beginning and the end of each sort.  If other code is included, it may have a large, albeit fixed, cost, which would tend to drown out the differences between the runs, if any. Why take a chance!  <strong><u> If you get</u> <u>too many zero time data values or any negative time values then you must fix the problem.</u></strong> One way to do this is to use larger, files than those specified.  Another solution is to perform the sorting in a loop, N times, and calculate an average value.  <u>You would need to be careful to start over with unsorted data, each time through the loop.</u>

Turn in an analysis comparing the two sorts and their performance.  Be sure to comment on the relative runtimes of the various runs, the effect of the order of the data, the effect of different size files, and the effect of different partition sizes and pivot selection methods for <strong>Quicksort</strong>.  Which factor has the most effect on the efficiency? Be sure to consider both time and space efficiency.  Be sure to justify your data structures.  As time permits consider examining alternate methods of selecting the pivot for <strong>Quicksort</strong>. Also consider files of size 10,000 or additional random files – perhaps with 15-20% duplicates.   <u>Your write-up must include a table of the times obtained.</u>