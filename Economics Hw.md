```python
import math
def P_Given_G(i,N,G):
  Term=(1+i)**N
  P=G/i*(((Term-1)/(i*Term))-(N/Term))
  return P
Present_Value_Grad=P_Given_G(.12,6,110)

def P_Given_A(i,N,A):
  Term=(1+i)**N
  P=A*(Term-1)/(i*Term)
  return(P)
Present_Value_A=P_Given_A(.12,6,100)
Total_Present=Present_Value_A+Present_Value_Grad
print(Total_Present)

def P_Given_F(i,N,F):
  Term=(1+i)**N
  P=F*(1/Term)
  return(P)

P_1=P_Given_F(.12,2,100)
P_2=P_Given_F(.12,3,210)
P_3=P_Given_F(.12,4,320)
P_4=P_Given_F(.12,5,430)
P_5=P_Given_F(.12,6,540)
P_6=P_Given_F(.12,7,650)
P_Tot=P_1+P_2+P_3+P_4+P_5+P_6
print(P_Tot)

K_Value=P_Given_F(.12,4,1)+P_Given_F(.12,5,1)
print(K_Value)

K=P_Tot/K_Value
print(K)
