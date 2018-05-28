# 4.8
import math
from scipy import stats
P1 = 0.52
P2 = 0.47
n1 = n2 = 100
# both are binomial distribution
sd =  math.sqrt((P1*(1-P1))/n1 + (P2*(1-P2))/n2)
# z= X-Mu/Sigma = X - (Mu1-Mu2)/sd
# since we want p2 > p1 then p1-p2<0 so we are taking X=0 here
z1 = (0-(.52-.47))/sd
print (z1)
#z score of z1 = .2420 =24%
print ("Probability of greater percentage of Republican voters in the second state than in the first state is 24%")
