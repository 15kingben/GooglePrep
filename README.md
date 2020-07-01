# Learning #
### Algorithms Live! ###
[youtube](https://www.youtube.com/channel/UCBLr7ISa_YDy5qeATupf26w) | [blogspot](http://algorithms-live.blogspot.com/)


**Recommended: Do them All!**
 - Watch episode and solve each problem on your own (most have online judges)
 - Skim coding section to potentially pick up some new coding techniques


**Minimal: Do the following:**
- [Fenwick Trees](https://www.youtube.com/watch?v=kPaJfAUwViY)
- [Trees and Diameters](https://www.youtube.com/watch?v=2PFl93WM_ao)
- [Segment Trees](https://www.youtube.com/watch?v=Tr-xEGoByFQ)
- [Geometric Sweeps](https://www.youtube.com/watch?v=gXn2yUHpvRE)
- [Cows](https://www.youtube.com/watch?v=OPDRYkCWdGs) (Important Binary search technique but a harder format)
- [Solution Bags](https://www.youtube.com/watch?v=oaYsWnohXpA&t=2661s)
- [Exchange Arguments](https://www.youtube.com/watch?v=Oq1seKJvfQU)
- [Binary Lifting LCA](https://www.youtube.com/watch?v=kOfa6t8WnbI)
- [Knapsack DP](https://www.youtube.com/watch?v=U4O3SwDamA4)
- [Bitmask DP](https://www.youtube.com/watch?v=rlTkd4yOQpE)
- [DFS LowLink](https://www.youtube.com/watch?v=iYJqgMKYsdI)
- [Biconnected Decomposition](https://www.youtube.com/watch?v=tRTezLvPZ3k&t=2318s)
- [Strongly Connected Components](https://www.youtube.com/watch?v=z9oOadBgO9I)
- [Topological Sort](https://www.youtube.com/watch?v=9Wbej7Fy5Lw)
- [Orchestra](https://www.youtube.com/watch?v=bLxsset706E) (It's like a hard version of a classic interview problem)
- [Max Flow](https://www.youtube.com/watch?v=K1i-wP82Zdo&t=771s)
- [Venture Cup](https://www.youtube.com/watch?v=97ovVAJBbkA) (Good Mathematical Approach to simplify a problem)

### Learning From Contests ###
Any time you fail a problem in a contest, look at the solutions afterwards. If it uses a concept you've never heard of, learn that and solve the problem. You will almost certainly see it again somewhere.

# Contests
- Leetcode: Saturday 7:30 PST (1 hour 30 minutes)
- Codeforces: 1-2 per week but latest is like 8am PST (2 hours)
- Codechef: 1 Long Challenge (2 weekends long)
- Google Code Jam: Once a year in April, but usually very fun problems.
- Find more contests: [clist.by](clist.by)

I recommend doing the Long challenge every month, and doing Leetcode as you are in the mood. Leetcode is most representative of interview but less effective for learning. The long contest gives you time to be creative and explore lots of solutions. 

**It's important to not look up the answer immediately. The value in spending hours considering failing approaches is that you learn and gain an intuition for what does not work. That way, in an interview, you spend your time exploring only solutions that have potential.**

#### Goals: 
Division 1 on Codeforces or Codechef and completing the weekly Leetcode contest in < 1 hour is overkill but a good benchmark to strive for anyway.

# Learning Objectives
- Learn Algorithmic concepts
  - This is actually the least important, complicated theory questions are pretty rare in interviews. Segment Trees and Flow is like the absolute limit
- Get better at coding/debugging
  - Debugging problems like these is very hard, and extremely costly in a programming contest. You need to learn how to identify errors quickly and gain an intuition for common edge cases.
  - You need to learn a programming style that minimizes code written and potential mistakes. Ex: sum all neighbors:
```
  for (int x = 0; x < N; x++)
    for (int y = 0; y < N; y++)
      int sum = 0;
      for (int dx =  -1; dx <= 1; dx++)
        for (int dy = -1; dy <= 1; dy++)
          sum += inBounds(x+dx, y+dy) ? arr[x+dx][y+dy] : 0;
	
public boolean inBounds(int x, int y) {
  return (x >= 0 && y >= 0 && x < N && y < N);
} 
```
Having written this code many times this is way cleaner to debug than having a bunch of if statements
- Articulating your thought process
  - Easiest way to fuckup an interview is to not say anything. You MUST explicitly say what you are thinking even if you have no idea. Most interviewers will give you useful hints so assume any hint they give you is the right answer.
  - There should be no dead air even when you are coding

# Interview Script
1. Ask clarifying questions (bounds, types, edge cases)
2. Propose a brute force solution (and describe its runtime)
3. (Time permitting) do the brute force on a small example)
4. Propose an optimized solution (and describe its runtime)
5. Do the optimized on a small example (this will also help you find logical errors)
6. Code the optimized solution
7. Throw out some edge cases that your solution will handle

# Behavioral Questions
- Idk I'm not good at these apparently

# Questions for Interviewer
- Tell me about your work
  - Works every time
  
# Practice Interview
Once you feel like you have mastered most concepts, give these questions a try. Try to complete each in 45 minutes or less.

### List of Questions to do

- [merge k sorted lists](https://leetcode.com/problems/merge-k-sorted-lists/) <details>
  <summary>Open after solving</summary>
  
  This is about 30% of all interview questions, so I hope you solved it.  
</details>


- [critical connections in a network](https://leetcode.com/problems/critical-connections-in-a-network/) <details>
  <summary>Open after solving</summary>
  
  DFS Lowlink coming in huge on this one. Here's another search based question: [minimum moves to move a box to their target location](https://leetcode.com/problems/minimum-moves-to-move-a-box-to-their-target-location/)
</details>

- [minimize malware spread](https://leetcode.com/problems/minimize-malware-spread/) <details>
  <summary>Open after solving</summary>
  
  This type of problem can be solved with Union-Find but I usually go for BFS/DFS when available. Here's another similar one: [check if there is a valid path in the grid](https://leetcode.com/problems/check-if-there-is-a-valid-path-in-a-grid/)
</details>

- [course schedule II](https://leetcode.com/problems/course-schedule-ii/) <details>
  <summary>Open after solving</summary>
  
  Topological sort is definitely something you want to know in and out. Here's another graph one: [find eventual safe states](https://leetcode.com/problems/find-eventual-safe-states/)
</details>

- [construct target array with multiple sums](https://leetcode.com/problems/construct-target-array-with-multiple-sums/) <details>
  <summary>Open after solving</summary>
  
  This one is pretty tricky, but it utilizes a very important technique of working backwards. If you didn't get that one, give this one a shot: [burst balloons](https://leetcode.com/problems/burst-balloons/)
</details>

- [uncrossed lines](https://leetcode.com/problems/uncrossed-lines/) <details>
  <summary>Open after solving</summary>
  
  It's pretty common especially for Google to hide standard problems behind some logical transformation that you need to think through. In an interview you would want to be talking through your though process with your inteviewer, and they might give you hints to put you on track. Here's some more DP practice: [count all valid pickup and delivery options](https://leetcode.com/problems/count-all-valid-pickup-and-delivery-options/)
</details>

- [smallest sufficient team](https://leetcode.com/problems/smallest-sufficient-team/) <details>
  <summary>Open after solving</summary>
  
  I hope you watched the Bitmask DP video, it's not as common in interviews, but if you can't find an optimal solution you can maybe break out the bitmask DP before moving on to something more optimized. Here's some more practice with bitmasks: [maximum students taking exam](https://leetcode.com/problems/maximum-students-taking-exam/)
</details>

- [daily temperatures](https://leetcode.com/problems/daily-temperatures/) <details>
  <summary>Open after solving</summary>
  
  Ah the classic Binary tree problem. In java you can use a TreeMap or TreeSet. These are pretty common and you'll look like a chump if O(N) is the best you can do. Here's another one to try: [minimum number of taps to open to water a garden](https://leetcode.com/problems/minimum-number-of-taps-to-open-to-water-a-garden/)
</details>

- [course schedule III](https://leetcode.com/problems/course-schedule-iii/) <details>
  <summary>Open after solving</summary>
  
  Lots of question have this format of sets of ranges, but the solutions can be varied. Here's are some more to try: [maximum profit in job scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling/) or [minimum number of arros to burst balloons](https://leetcode.com/problems/minimum-number-of-arrows-to-burst-balloons/) or [brick wall](https://leetcode.com/problems/brick-wall/)
</details>

- [find in mountain array](https://leetcode.com/problems/find-in-mountain-array/) <details>
  <summary>Open after solving</summary>
  
  A binary search question was the only one I messed up on in my actual interview. I think they are pretty tough to intuit and have a lot of edge cases that are tricky to iron out without being able to run code. Here's some more binary search: [find first and last position of element in sorted array](https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/)
</details>

### Other questions I like:
Some questions with elegant or clever solutions:
- [remove palindromic subsequences](https://leetcode.com/problems/remove-palindromic-subsequences/)
- [reverse substrings between each pair of parentheses](https://leetcode.com/problems/reverse-substrings-between-each-pair-of-parentheses/)
- [convert to base -2](https://leetcode.com/problems/convert-to-base-2/)
- [distinct sequences II](https://leetcode.com/problems/distinct-subsequences-ii/)
- [element appearing in more than 25% of sorted array](https://leetcode.com/problems/element-appearing-more-than-25-in-sorted-array/)
- [trapping rain water](https://leetcode.com/problems/trapping-rain-water/)
- [maximum performance of a team](https://leetcode.com/problems/maximum-performance-of-a-team/)

### Practice with a Googler
Ask a friend to give you a mock interview, behavioral and technical. I'm at `"".join("bking2015", "@", "gmail.com")`
