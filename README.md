# Array-Pair-Sum-Divisibility-Problem
Problem of Day (11-dec-2022) (GFG)

```
class Solution:
	def canPair(self, nuns, k):
	    if len(nums)%2!=0:
	        return False
	    l=[]
	    for i in range(len(nums)):
	        if nums[i]%k!=0:
	            l.append(nums[i]%k)
	    l.sort()
	    i=0
	    j=len(l)-1
	    if len(l)%2!=0:
	        return False
	    while i<j:
	        if (l[i]+l[j])%k==0:
	            i+=1
	            j-=1
	        else:
	            return False
        return True
