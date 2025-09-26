# numpy

import numpy as np 
a=[2,4,9,2]
b=np.array([2,4,9,2])
print(type(a))
print(type (b))
print(len(a)) # used to get number of element from list
print(b.size) # used to get number of element from numpy array 
print(a*2) # list itself got repeated 2 times
print(b*2) # broadcasting of numpy array since every number inside is getting multiplied by 2

b=np.array([2,4,9,2,5,8,89,43,789,232,4678,2232,134,4,3122])
print(b.shape) # element and dimension
print(b.size)
print(len(b))
print(b.ndim) # for dimension
# extract 43
print(b[7])
# extract 89,43,789
print(b[6:9])

c=np.array([[7,3,9,3,8],[17,2,8,5,23],[4,8,93,4,56]])
print(c)
print(c.shape)
print(c.size)
print(c.ndim)
# fetch  8,5
#       93,4
print(c[1:,2:4])

for i in range(1,21,2): # this will print number from 1 to 20 and step size is 2
 print(i)

np.arange(1,21)# this will print number from 1 to 20

myarr=np.arange(1,25).reshape(3,4,2) # this will reshape myarr in 3 block,each block has 4 row and each row has 2 numbers 
myarr

import sys # build-in python module 
a=24
b=24.12
print(sys.getsizeof(a))
print(sys.getsizeof(b))

myarr=np.arange(1,17).reshape(2,2,4)
myarr
myarr.reshape(8,-1) # this will give 8 row and for column anything will be fine 

a=[1,2,3,4,5]
b=a
b[1]=20 # changed something in b 
print(b) # change got reflected 
print(a) # change also got reflected in a though
# we didn't make any change in a 

a=[1,2,3,4,5]
b=a.copy()
b[1]=20 # changed something in b
print(b) # change got reflected 
print(a)

a=np.array([[5,64,23,45,78,3,246,89,53,24])
print(a.max())
print(a.min())
print(a.argmax()) # this will give the index number of highest number
print(a.argmin()) # this will give the index number of lowest number 

b=np.array([[4,6,27,34],[4,124,567,85],[3,21,23,57],[54,21,35,67],[12,10,29,56]])
print(b)
print(b.max())
print(b.min())
print(b.argmax())
print(b.argmin())

tanmayee=np.array([1,2,1010,4,108,18,71,610])
tanmayee
tanmayee<100 # this will give output in true/false
tanmayee[tanmayee<100] # and this will give numbers which are less than 100

a=np.array([[[34,45,22],[23,56,21]],[[4,6,13],[1,2,1]],[[43,23,45],[1,21,23]]])
print(a)
# extract 21 
print(a[0][1][2])
# extract 1,2,1
print(a[1][1])
# extract 6 13
#         2  1
print(a[1][:,1:])

mymat=np.ones((6,6)) # this will print ones in 6 rows and 6 columns 
mymat

for i in range(len(mymat)):
 mymat[i]=i
mymat
