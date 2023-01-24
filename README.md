# hanoi_tower_python_recursion
Hanoi tower problem using Python recursion
def hanoi(a, b, c, k):
    if(len(a) <= 0):
        return b
    else :
        c = a[0 : k+1]
        b.append(a[k]) 
        r = c
        a = r
        return hanoi(a[0 : -1],b, c, k-1)
q = [1,2,3,4]
s = len(q) -1
source = []
destination = []
t = []
t = hanoi(q,source, destination, s)
for i in range(len(t)-1, -1, -1):
    print(t[i])
