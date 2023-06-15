def binary_serach (list,key):
    low=0
    high=len(list)-1
    mid=0
    while low<=high:
        mid=(low+high)//2
        if key==list[mid]:
            return mid
        elif key<list[mid]:
            high=mid-1
        else:
            low=mid+1
    return-1
list=[20,40,51,65,85,86,89,90,95]
print(list)
key=int(input("enter the value: "))
result=binary_serach(list,key)
if key==-1:
    print("key not found")
else:
    print("key found", result) 
    
