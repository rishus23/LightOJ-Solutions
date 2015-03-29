#Solutions For Light OJ

Use the hints for solving the problem. See the solutions only in worst case situations. 

###1002 - Country Roads
You need to use a modification of Dijkstra's algorithm for solving thr peorblem. They key catch is in Dijkstra we use 

`a[i][j] + d[i] < d[j]`
`d[j] = a[i][j] + d[i]`

While here we should use

`max(a[i][j], d[i]) < d[j]`
`d[j] = max(a[i][j], d[i])`

###1003 - Drunk
The task is to check whether cycle exists in the directed graph. If cycle exists he can't drink all. You can use a hash function or map to convert the drinks to numbers. Once converted use DFS or a suitable algo for checking the existance of cycles. I used `DFS` for the search of cycles. 

###1004 - Monkey Banana Problem
This is a basic Dynamic Programming problem. The tricky part is to write the loops. While calculating the maximum bananas the second inner loop will run forward till i < n and for the remaining it would run backward. Check the solution for understanding the logic behind this. 

###1006 - Hex-a-bonacci
This question is quite simple and straight forward as compared to the previous questions. All you need to dos is to replace the recursion with a for loop. Also make sure to take the modulo before storing the values in array as the values can be quite large

###1007 - Mathematically Hard
You should take exereme care while solving this problem. The input require very first IO method. Scanf and Printf would be the best choice if you are using C++. You can need to use a modified version of the Sieve method for cracking the problem. The approach I used was to first store the prime numbers using the sieve method and then to use a sieve like method to calculate `phi of n`. Take extra care to use `llu` while printing out the answer as the output is in the range of unsigned long long.

###1008 - Fibsieve`s Fantabulous Birthday 
Try to find the pattern in which the numbers are appearing. If you look carefully you can obtain the pattern and device an formula to find the coordinates. 

###1009 - Back to Underworld
I didn't use any normal graph algorithm for solving this problem. Even tough the problem uses a little concept of connected componenents. Try approaching the problem by considering the rivals as nodes in a graph. Check the code if you are stuck for a long time

###1011 - Marriage Ceremonies 
This is a normal Memoization with Bit masking type problem. Normal recursion without memoization causes a TLE. 

###1012 - Guilty Prince
This is one is a really simple graph problem. Keep marking the visited nodes to avoid visiting them again

###1014 - Ifter Party
This is also a normal Ad-Hoc problem. The simplified task is to find the divisors of p - l which are greater than l.

###1016 - Brush II
This is yet another adhoc problem. What you need to do is to ietrate over all the y points in ascending order in such a way that you increase the counter only when the difference of ym, ym+1, ....yn becomes greater than w. The counter would give you the answer. 

###1019 - Brush IV
This is a trivial application of Shortest Path algorithms. Implementing Floyd Warshal solution for this can accept the solution in a few lines of code

###1020 - A Childhood game
This is a problem under Game theory. You can write the solution for this problem by just observing the pattern of win or loss. If Alice is taking the stone first she will get a win for 0, 2, 3, 5 .... and loss for 1, 4, 7 .... You can easily use this observation for solving the problem. 

###1022 - Circle in Square
The only tricky part in this question is to use double for all the calculations. Always use double instead of float in programming contests. 

###1023 - Discovering Permutations
This is a pretty simple questions. You can use the C++ `next_permutation` for cracking this problem in a few lines of code

###1025
This is a dp problem
