# python
A person saves his monthly saving according to the given schema. He saves the same amount of money which is equal to the money saved in the immediate previous two months. Assume, initially, he saved 1000 rupees and in the first month he saved another 1000. Your task is to tell how much he had totally saved at the end of 'n' months

#code for This Problem
#Fuction for the Problem

from functools import reduce 
def save(n):
list=[]
if(n==0):
print("1000") 
elif(n==1): 
print("2000")
else:
m0=1000
list.append(me)
m1=1000
list.append(m1) 
for i in range(2,n+1):
m2=m0+m1
list.append(m2)
m0=m1
m1=m2
tot=reduce(lambda x,y:x+y,list) 
print(tot)
#input is taken Here

n=int(input())
save(n)
