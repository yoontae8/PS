
### 풀이 
round 하게 다 1bit씩 차이가 나야하는 상황. 
첫 elem을 0으로 고정해두고 생각하면됨 
n=1, n=2, n=3 을 절댓값 차이가 최대한 적도록 아래에서부터 더해주다보니 second half에서 2^(n-1)을 당연히 반드시 올려줘야했고 
그 뒤로는 다시 최소한의 diff로 내려오도록 해보았고 last elem이 0과 1bit 차이 나야하는데 그건 0+2^(n-1)만 가능 
-> first half 에서 0~2^(n-1)-1 이고, second half는 first half의 reversed에 2^(n-1) 더해주면됨 


### 코드 
```python 
class Solution(object):
    def grayCode(self, n):
        """
        :type n: int
        :rtype: List[int]
        """
    
        now_output = [0] # start from zero 
        
        for i in range(n):
            first_half = now_output
            last_half = [x + (1<<i) for x in reversed(first_half) ] # 이거 두줄에 쓰고싶다
            now_output = first_half+last_half 
        return now_output
```        

### 제출 

Time Submitted
Status
Runtime
Memory
Language
12/08/2021 23:25	Accepted	90 ms	19.5 MB	python
12/08/2021 23:22	Accepted	116 ms	19.2 MB	python
12/08/2021 23:22	Accepted	110 ms	19.2 MB	python
12/08/2021 23:21	Accepted	103 ms	19.4 MB	python
 
 
### 코멘트 
코드 정리하니까 time percentages 많이 변한다.. 
