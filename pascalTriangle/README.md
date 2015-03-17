# pascalTriangle

 #Data Structure:

    ArrayList, List

 #Analyze: 

    1st: 1

    2nd: 1 1

    3rd: 1 2 1

    4th: 1 3 3 1

    5th: 1 4 6 4 1

    create one list per row
    length of the x row is x (length of the 5th row is 5)
    the 1st and the last one are 1's
    others are nth+(n-1)th in previous row

 #Time Complexity:

    ex. O(5+4+3+2+1+5)
    O(n+...+1+n)=O((n+1)*n/2+n)=O(n^2/2+n/2+n)=O(n^2)

#Algorithm: 

    Current[n]=Previous[n]+Previous[n-1];
