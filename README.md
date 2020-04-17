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
Div1 on Codeforces or Codechef and completing Leetcode in < 1 hour is more than enough, but a good benchmark to strive for.

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
### List of Questions to do
 - TBD

### Practice with Googler
Ask a friend to give you a mock interview, behavioral and technical.
