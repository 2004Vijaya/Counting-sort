# Counting-sort

'''
It is a non comparision sort
no negative numbers
long numbers are not used

value=2 1 1 0 2 5 4 0 2 8 7  7  9  2  0  1  9
index=0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16

Range of values:0 1 2 3 4 5 6 7 8 9
Number of vales:3 3 4 0 1 1 0 2 1 2
possibilities of o/p:3 6 10 10 11 12 12 14 15 17(sum of the repeated values in above)

*****Algorithm*****
1. find max min of array
2.min!<0
3.create a count array to store frequency of numbers
4.modify the count array for each element to be stored the sum of previous counts
5.place the output array back to the original array

#pseudo code

countsort(arr,n):
1. find the max in array
2.crate count(0-max)
3.for i in range(0,n-1):
count[arr[i]]+=1
4.for i in range(t,max_val):
count[i]+=count[i-1]
create outputt arr[n]
5.for i ->n-1 to 0:
output[count[a[i]]-1]=a[i]
count[a[i]]-=1
copy output to array
'''
