1.
a=int(input("enter a 1 number:"))
b=int(input("enter a 2 number:"))
if (a>=b):
    print("{} is greater".format(a))
else:
    print("{} is greater".format(b))

--------------------------------------2---------------------------------------------
2.
a=int(input("enter a number 1:"))
b=int(input("Enter a number 2:"))
c=int(input("Enter a number 3:"))
if(a>b and a>c):
    if(b>c):
        print(b,"is the second greatest number")
    else:
        print(c,"is the second greatest number")
elif(b>c and b>a):
    if(c>a):
        print(c,"is the second greatest number")
    else:
        print(a,"is the second greatest number")
else:
    if(a>b):
        print(a,"is the second greatest number")
    else:
        print(b,"is the second greatest number")
.........................................3................................................
3.
a=int(input("Enter a number:"))
if(a%2==0):
    if(a%6==0):
        print(a*6)
    else:
        print(a)
else:
    print(a-6)
    -------------------------------4--------------------------------------
4.
a=input("Enter Your Name:")
b=int(input("Enter your Age:"))
c=input("Enter your Gender:")
if(c=="MALE"):
    if(b>18 and b<70):
        print("dear",a,"is eligible for vote")
    else:
        print("Dear",a,"is not eligible for vote")
elif(c=="FEMALE"):
    if(b>25 and b<70):
        print("Dear",a,"is eligible for vote")
    else:
        print("Dear",a,"is not eligible for vote")
.......................................5................................................
5.
a=int(input("Enter a number :"))
for i in range (2,a):
   if(a%i==0):
      print(i)
......................................6..............................................
6.
a=int(input("Enter a number:"))
c=0
for i in range (2,a):
    if(a%i==0):
      c=c+1
if(c==0):
    print("prime")
else:
    print("composite")
....................................7............................................
7,
for i in range(31):
    print("*",end="")
print()
for i in range(15):
    print("!                             !")
for i in range(31):
    print("!",end="")
...................................8.........................................
8,
n=int(input("Enter a number:"))
fact=1 
for i in range(1,n+1):
    fact=fact*i 
print("the factorial of ",n,"is",fact)
....................................9...........................................
9, TABLES
a=int(input("Enter a number "))
if(a%2==0):
    for i in range(1,21):
        print("{} * {} = {}".format(a,i,i*a))
else:
    for i in range(1,11):
        print("{} * {} = {}".format(a,i,i*a))
....................................10............................................
10,
n=int(input("Enter a number:"))
sum=0
while(n>0):
    rem=n%10
    n=n//10
    sum=rem+sum
print(sum)
......................................11...........................................
11,ADD INFINITE NUMBERS
sum=0
while(1):
    n=int(input("Enter a amount"))
    if(n==0):
        break
    sum=sum+n 
print(sum)
......................................12..............................................
12,
para=input("Enter the sentence :")
c=0
for i in para:
    if(i==" "):
        c=c+1
print("Enter the number of sentence",c+1)
.........................................13.................................................
13,
para=input("Enter the sentence :")
c=0
for i in range(len(para)):
    if(para[i]==" " and para[i+1]!=" "):
        c=c+1
print("The number of words are ",c+1)
........................................14....................................................
14,
password=input("Enter your password :")
l,u,sp,d=0,0,0,0
if(len(password)>7):
    for i in password:
        if(i.isupper()):
            u=u+1
            l=l+1 
        elif(i.islower()):
        elif(i.isdigit()):
            d=d+1 
        else:
            sp=sp+1 
    if(l>0 and u>0 and sp>0 and d>0):
        print("The password is strong")
    else:
        print("The password is weak")
else:
    print("add minimum characters")
    ...............................................................................................................
15,
a=(input("Enter a word :"))
a=a.upper()
b=a[::-1]
if(a==b):
    print("It is palindrome")
else:
    print("It is not palindrome")
.......................................................................................................................
16,
a=[]
b=[]
for i in range(10):
      c=int(input("Enter a number :"))
      a.append(c)
      b.append(c**2)
print(a)
print(b)
............................................................................................................................
17,
a=[10,20,30,40]
b=['-','+','-']
print(a)
print(b)
for i in range(len(b)):
    m1=a.pop()
    n1=a.pop()
    c=b.pop()
    if(c=='+'):
        a.append(m1+n1)
    else:
        a.append(m1-n1)
    print(a)
    print(b)
......................................................................................................................
18,
stud=["ranga","rohith","arun","mith"]
mark=[74,80,70,85]
for i in range(4):
    for j in range(i+1,4):
        if(mark[i]>mark[j]):
            mark[i],mark[j]=mark[j],mark[i]
            stud[i],stud[j]=stud[j],stud[i]
            print(stud)
            print(mark)
............................................................................................................................
19,
emp=["ra","ka","ma","pa","va","ya","la","na","ta","sa"]
gen=['M','M','M','M','M','M','F','F','F','F']
sal=[10,20,30,40,50,60,70,80,90,100]
memo=[1,2,3,1,2,1,2,1,2,3]

a=int(input("No of employee to be removed"))

reject=[]
doubt_memo=[]
doubt_name=[]
doubt_sal=[]

for i in range(10):
    if(len(reject)==a):
        break
    if(memo[i]==3):
        reject.append(emp[i])
    elif(memo[i]==2 and gen[i]=='M'):
        doubt_memo.append(memo[i])
        doubt_name.append(emp[i])
        doubt_sal.append(sal[i])
        
for i in range(len(doubt_sal)):
    for j in range(i+1,len(doubt_sal)):
        if(doubt_sal[i]>doubt_sal[j]):
            doubt_sal[i],doubt[j]=doubt_sal[j],doubt_sal[i]
            doubt_name[i],doubt_name[j]=doubt_name[j],doubt_name[i]
            
doubt1_name=doubt_name[::-1]
for i in range(len(doubt_name)):
    if(len(reject)==a):
        break
    reject.append(doubt1_name[i])
print(reject)
...............................................................................................................................
20,
from datetime import datetime 
import pytz
a=pytz.timezone("Asia/kolkata")
b=datetime.now(a)
print(b)
.......................................................................................................................
21,
import time 
import random

a=input("enter player 1")
b=input("enter player 2")

n1=[]
n2=[]
p1=[]
p2=[]

for i in range(1,15,5):
    d=random.randint(i,i+5)
    n1.append(d)
    
for i in range(1,15,5):
    d=random.randint(i,i+5)
    n2.append(d)

s1,s2=0,0
for i in range(3):
    g=int(input("enter the number"))
    p1.append(g)
    if(n1 in p1):
      s1=s1+1
      
for i in range(3):
    g1=int(input("enter the number"))
    p2.append(g1)
    if(n2 in p2):
      s1=s1+1

time.sleep(5)
print(a)
print()
.........................................................................................................................
22,
def add(b,c):
    print(b+c)
def tables(b):
    for i in range(1,11):
       print("{}*{}={}".format(i,b,i*b))
def vol(x,y,z):
    print(x+y+z)
def avg(x,y,z,v):
    print(x+y+z+v/4)

while(1):
    print(".......1.Addition........")
    print(".......2.Tables.......")
    print(".......3.volume........")
    print(".......4.average........")
    print(".......5.exit.......")
    a=int(input("Enter your choice"))
    if(a==1):
        b=int(input("Enter a number"))
        c=int(input("Enter a number"))
        add(b,c)
    elif(a==2):
        b=int(input("Enter a number"))
        tables(b)
    elif(a==3):
        vol(3,4,5)
    elif(a==4):
        avg(3,4,5,6)
    elif(a==5):
        break
   
    
    
    
    
        
        
