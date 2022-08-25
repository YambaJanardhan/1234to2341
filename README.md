x=int(input())

for i in range(x):
    y=input().split()
    a=int(y[0])
    b=int(y[1])
    c=int(y[2])
    if b>a:
        d=int(b/a)
        e=(b-(d*a))
        s=[]
        for i in range(1,a+1):
            s.append(i)
        first=s[0:e+1]
        second=s[c-1:]
        second.extend(first)
        print(second)
        l=len(second)
        print(second[l-1])
    elif b==a:
        s=[]
        for i in range(1,a+1):
            s.append(i)
        a1=s
        b1=c+1
        r=b1%len(a1)
        first=a1[0:r]
        second=a1[r:]
        second.extend(first)
        print(second)
        l=len(second)
        print(second[l-1])
    elif b<a:
        d=a-b
        s=[]
        for i in range(c,a+1):
            s.append(i)
        q=(s[0:b])
        print(q)
        l=len(q)
        print(q[l-1])
