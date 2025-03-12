## Codeforces Contest review - Codeforces Round 1008

&nbsp;&nbsp;&nbsp;&nbsp;For once, my luck changed.

### Problem A. Final Verdict [(2078A)](https://codeforces.com/contest/2078/problem/A)
&nbsp;&nbsp;&nbsp;&nbsp;Another trolly problem to begin with. The problem essentially asks us if $x = avg(a)$ is correct, since each subsequence has equal length, the average will never change.

### Problem B. Vicious Labyrinth [(2078B)](https://codeforces.com/contest/2078/problem/B)

&nbsp;&nbsp;&nbsp;&nbsp;A nice problem to think about in my opinion. The idea is just greedy, we want as many people at room $n$ at the end as possible. We only need to check the parity of $k$ here, one parity will give us a minimum distance of $0,$, the other one gives $1.$

### Problem C. Breach of Faith [(2078C)](https://codeforces.com/contest/2078/problem/C)

&nbsp;&nbsp;&nbsp;&nbsp;The complicated third condition basically translates to "sum of even positions = sum of odd positions". Since we want all number to be pairwise distinct, we might as well make $a_1$ the largest number, which can be done if we group $a_1$ with the smallest $n-1$ numbers in the even positions, and throwing the other number at the odd positions.

&nbsp;&nbsp;&nbsp;&nbsp;I actually overthought this problem at first, and somehow I thought that the case $n = 1, a = [4, 8]$ was impossible. The only solution to this test case (which is $a_1 = 12$) gave me the solution immediately, but I really think that I shouldn't have spent $15$ minutes here.

### Problem E. Finding OR Sum [(2078E)](https://codeforces.com/contest/2078/problem/E)
&nbsp;&nbsp;&nbsp;&nbsp;For some reason, interactive problems just get their rating and position shot up higher than it should be, so I attempted this instead of D. The gamble did work out, but I think that I could have solved this way faster.

&nbsp;&nbsp;&nbsp;&nbsp;The idea for this problem is to figure out for each bit position, if the corresponding bit in $x$ and $y$ are both $0,$, both $1,$ or one of each. We can do that bit-by-bit, starting from the lowest position. If we ask $0$ and $1$ in two different queries and compare the differences, we should immediately learn which combination it is. Cramming all of those into $2$ queries will give us the two queries being $1010...10$ and $0101...01$ in binary (each has $30$ digits), which is $715827882$ and $357913941$ in decimal.

&nbsp;&nbsp;&nbsp;&nbsp;The idea for this problem is quite neat, and the idea is quite natural also. It is a nice interactive problem, but in my opinion, this should have been in the D slot.

&nbsp;&nbsp;&nbsp;&nbsp;I didn't attempt D at all, and I solved E within the last half-hour. It was good enough to earn me $22$ rating points, which I am quite happy about.

&nbsp;&nbsp;&nbsp;&nbsp;Note: This is mostly my personal experience with the problems, you might not completely agree with some of the things here. Please do not make this an excuse to attack me and/or anyone who was involved in the making of this contest.
