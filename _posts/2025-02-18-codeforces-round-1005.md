## Codeforces Contest review - Round 1005 test

&nbsp;&nbsp;&nbsp;&nbsp;This was my first round in about a month \(my last contest was January 22nd\), so I'm pretty rusty. It isn't really an excuse to how bad this contest went for me, I completely could've done better.

### Problem A. Brogramming Contest [(2064A)](https://codeforces.com/contest/2064/problem/A)
&nbsp;&nbsp;&nbsp;&nbsp;This is (at least to me) a standard problem for the div2A, only requiring a quick observation and some greedy work. To avoid doing some casework with the string beginning with either $0$ or $1$, simply add a $0$ to the beginning of the string, and now it remains to count the number of adjacent characters that are different.

&nbsp;&nbsp;&nbsp;&nbsp;Alright, let the chaos begin.

### Problem B. Variety is Discouraged [(2064B)](https://codeforces.com/contest/2064/problem/B)

&nbsp;&nbsp;&nbsp;&nbsp;This wasn't a particularly difficult problem. The main idea is that the entire array will give the maximal score, so the issue is to find what we can remove, while still keeping the same score. Any elements that appear exactly once will do just that, so the problem reduces down to find the largest segments of the number $1$.

&nbsp;&nbsp;&nbsp;&nbsp;Though for some reason, I decided to just *forget* how to code, and used a **continue**, instead of a **break**, to exit the for loop. This mistake somehow wasn't caught in the sample tests (and I should've been more careful), so I received a WA on my first submission. Thankfully I fixed it quite quickly after that, so no rage induced (yet).

### Problem C. Remove the Ends [(2064C)](https://codeforces.com/contest/2064/problem/C)
&nbsp;&nbsp;&nbsp;&nbsp;Quite a weird problem, in my opinion. It is still just greedy, the idea being that "if you take a positive integer, might as well take all of those on the left" (and also the opposite for the negatives). So the problem reduces down to a classic prefix-suffix problem, in which we calculate the prefix sum of all positive integers, and suffix sum of all negative integers.

&nbsp;&nbsp;&nbsp;&nbsp;My first two submissions tried to simulate the process with a **while** loop, and try to account for some cases where the signs are the opposite of what we want it to be. It wasn't really caught in the sample tests (again, somehow?), so I spent some time trying to figure out in which cases the loop would break. Eventually I came up with the correct solution, with the realization that the loop that I implemented was really only solving for $1$ case of the prefix-suffix combination, as opposed to the $n$ cases we were supposed to do.

And finally,
### Problem D. Eating [(2064C)](https://codeforces.com/contest/2064/problem/D)
&nbsp;&nbsp;&nbsp;&nbsp;To be honest, this was quite an interesting idea for a problem, since it's not often to see bitwise operations in the mix with queries. It was *very* challenging though, I personally didn't solve it myself.

&nbsp;&nbsp;&nbsp;&nbsp;The idea to calculate the score is basically to look at the highest bit, since it is guaranteed that if a slime has a lower highest bit, it will be eaten immediately. The hardest part was coming up with a strategy to implement it.

My first few submissions were basically a *wrong* submission - for some reason I thought that the slime's highest bit is lowered after every time it eats another slime. The **while** loop was also $O(q)$, so the code got TLE on pretests $8$, and WA on pretests $3$. I then tried to use a segment tree to do the *skipping* part (where we jump over the slimes whose highest bit were not high enough). The final code that I submitted at the last minute ultimately didn't make it - the complexity was (I think?) $O(n + q \cdot log A \cdot (log n)^2)$, with probably a very high constant factor. It definitely was quite frustrating to fail here, but it was mostly due to myself not being good enough, not the problem itself.

Overall, my final delta was $-79$. It was quite deserved to be honest, my performance were really sub-par for this contest.

&nbsp;&nbsp;&nbsp;&nbsp;Note: This is mostly my personal experience with the problems, you might not completely agree with some of the things here. Please do not make this an excuse to attack me and/or anyone who was involved in the making of this contest.
