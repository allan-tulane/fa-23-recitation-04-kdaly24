# CMPS 2200 Reciation 5
## Answers

**Name:**___Killian Daly__________


Place all written answers from `recitation-05.md` here for easier grading.







- **1b.**
Random List
|        |      n  |  random-pivot |         fixed-pivot |              timsort |
|--------|---------|---------------|---------------------|----------------------|
|    100 |   0.183 |         0.242 |               0.274 |                0.002 |
|    200 |   0.392 |         0.506 |               0.942 |                0.003 |
|    500 |   1.011 |         1.361 |               1.442 |                0.006 |
|   1000 |   2.230 |         2.749 |               2.257 |                0.010 |
|   2000 |   4.753 |         6.399 |              14.808 |                0.020 |
|   5000 |  12.931 |        15.405 |              43.442 |                0.052 |
|  10000 |  26.537 |        33.501 |             258.070 |                0.097 |
|  20000 |  59.608 |        70.957 |             599.225 |                0.191 |
|  50000 | 168.004 |       192.039 |            6615.044 |                0.509 |
| 100000 | 351.777 |       406.680 |           28161.521 |                1.017 |

Sorted List
|        |      n  |  random-pivot |         fixed-pivot |              timsort |
|--------|---------|---------------|---------------------|----------------------|
|    100 |   0.188 |         0.235 |               0.275 |                0.003 |
|    200 |   0.397 |         0.517 |               0.949 |                0.003 |
|    500 |   1.056 |         1.418 |               5.487 |                0.007 |
|   1000 |   2.172 |         3.058 |              21.515 |                0.011 |
|   2000 |   4.753 |         6.069 |              86.862 |                0.020 |
|   5000 |  13.176 |        17.062 |             547.420 |                0.053 |
|  10000 |  28.202 |        33.794 |            2290.433 |                0.100 |
|  20000 |  59.646 |        71.857 |            9830.731 |                0.192 |
|  50000 | 162.532 |       198.390 |           67924.822 |                0.492 |
| 100000 | 357.450 |       421.079 |          283908.669 |                1.180 |

The Quicksort implementations seem to have a time complexity of around $O(nlogn)$, which falls within the expected bound $O(nlogn)$ for Quick sort algorithms. 
For selection sort, the average time complexity seems to be $O(n^2)$, which again matches the selection sort upper bound $O(n^2)$.
When changing the list input to sorted lists, fixed pivots efficiency heavily decreases, and the time taken increases. This makes sense as in a sorted list, fixed pivot will run through every possible pivot value as the fixed pivot starts on the furthest side of the list, and will have to run through the pivot N times.

- **1c.**
Timesort, as seen in the two graphs, is much faster than our current implementations, both for sorted and unsorted lists.