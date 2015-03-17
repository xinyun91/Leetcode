#Analyze:

ex: n=25 #ofTrailingZeros?

  # of 5's: 25=5*5
  
  # of 5's: 20=5*4

  # of 5's: 15=5*3

  # of 5's: 10=5*2

  # of 5's: 5=5*1

  Sum: 6

#Algorithm: 

while(n>0){n/=5; #ofZeros = #ofZeros + n;}
