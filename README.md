# SeniorSem

newlist = []

inputNum = input('Enter 3 or more numbers seperated by space \n')

newlist = inputNum.split()

for i in range(len(newlist)):
    newlist[i] = int(newlist[i])

def insertionsort(num):

    for i in range(1,len(num)):
        j = num[i]

        k = i-1

        while k >= 0 and j < num[k]:
            num[k+1]= num[k]
            k -= 1
            num[k+1]= j


print(newlist)


insertionsort(newlist)
print(newlist)
