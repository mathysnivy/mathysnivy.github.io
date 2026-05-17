## Codeforces Contest review - Educational Round 175

&nbsp;&nbsp;&nbsp;&nbsp;*ah yes, an Edu round, where anything can happen.*

### Problem A. FizzBuzz Remixed [(2070A)](https://codeforces.com/contest/2070/problem/A)
&nbsp;&nbsp;&nbsp;&nbsp;Nice, simple problem to start the contest with. The problem itself is quite simple, and there is not much to really talk about here.

### Problem B. Robot Program [(2070B)](https://codeforces.com/contest/2070/problem/B)

&nbsp;&nbsp;&nbsp;&nbsp;This was a nice problem. The solution mainly revolves around finding the number of steps required each time to get back to point $0$, and a simple computation finishes it out. For once I didn't make a bad mistake at problem B, and so I was able to solve this rather quickly.

### Problem C. Limited Repainting [(2070C)](https://codeforces.com/contest/2070/problem/C)
&nbsp;&nbsp;&nbsp;&nbsp;It's been a while since the last problem that required us to binary search for the answer. The idea is quite obvious when we realize that we can skip over any squares that doesn't exceed the penalty that we are aiming for, so checking if an answer can be achieved or not is simply done in $O(n)$.

&nbsp;&nbsp;&nbsp;&nbsp;For some reason, the sample test cases didn't catch my mistake of flipping blue and red, and I went through $2$ submissions before realizing. Quite a bad error on my end, but it didn't create much trouble, and the problem is good regardless.

And finally,
### Problem D. Tree Jumps [(2070D)](https://codeforces.com/contest/2070/problem/D)
&nbsp;&nbsp;&nbsp;&nbsp;How is this rated 1600, when C is rated 1500?

&nbsp;&nbsp;&nbsp;&nbsp;The idea of a valid sequence here is quite interesting. The problem screams some kind of DFS and DP on trees, and the calculation is done in decreasing order of the nodes' depth. 

Overall, nice problem to think about. I did spend almost a full hour here, since I tried different methods to calculate the DP (I almost used DFS 3 times, too), but it was nice to get this one done.

My final ranking was 824th among the official Division 2 contestants, and lost $9$ rating points. I was chilling for most of the contest, the negative delta was kinda unfortunate, but overall this was a decent performance for me.

&nbsp;&nbsp;&nbsp;&nbsp;Note: This is mostly my personal experience with the problems, you might not completely agree with some of the things here. Please do not make this an excuse to attack me and/or anyone who was involved in the making of this contest.
