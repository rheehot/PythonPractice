# PythonPractice
PythonPractice/ Practice ,  basic
<br><br>Python을 처음 시작하면서, 문법예제 연습을 위해 만들었습니다.
<br><br>
~~~python
print('Hello World!')
print('안녕하세요')
~~~
<br><br>
~~~python
number1 = 1
pi = 3.14
flag = True
char = 'X'
chars = 'I Love Python'

print(number1,pi,flag,char,chars)
print('-------------')

s = number1+2
s2 = pi + number1

print(s,s2)
~~~
<br><br>
~~~python
x=1
y=2

if x>y:
    print('x가 y보다 큽니다.')
elif x<y:
    print('x가 y보다 작습니다.')
else:
    print('x와 y가 같습니다.') 
~~~
<br><br>
~~~python
scope = [1,2,3,4,5]
for x in scope:
    print(x, end=" ")

print(' ')

stri = 'abcdef'
for y in stri:
    print(y, end=" ")

print(' ')

dicti = {'a':97,'b':98,'c':99}
for z in dicti:
    print(z, end=" ")

print(' ')

dicti = {'a':97,'b':98,'c':99}
for q in dicti:
    print(dicti[q], end=" ")

print(' ')

for c in range(2,10,3):
    print(c,end=" ")
~~~

<br><br>
~~~python
scope = [1,2,3,4,5]
for x in scope:
    print(x)
else:
    print('Perfect')

print('=========')

scope = [1,2,3,4,5]
for y in scope:
    print(y)
    break
else:
    print('Perfect')
~~~
<br><br>
~~~python
x=0
while x<10:
    x+=1
    if x<3:
        continue
    print(x)
    if x>7:
        break 
~~~
<br><br>
~~~python
strdata ='Time is money!!'
listdata =[1,2,[1,2,3]]
print(strdata[5])
print(strdata[-2])
print(listdata[0])
print(listdata[-1])
print(listdata[2][-1])
~~~
<br><br>
~~~python
strdata='Time is money'
print(strdata[1:5])
print(strdata[:7])
print(strdata[9:])
print(strdata[:-3])
print(strdata[-3:])
print(strdata[:])
print(strdata[::2])
~~~

<br><br>
~~~python
strdata1='I love'; strdata2='Python'; strdata3='you'
listdata1=[1,2,3]; listdata2=[4,5,6]
print(strdata1+strdata2)
print(strdata1+strdata3*3)
print(listdata1+listdata2)
addata = '나와'+strdata3+'좋아한다'+strdata2*2+'!!'
print(addata)
~~~

<br><br>
~~~python
listdata=[1,2,3,4]
ret1=5 in listdata
ret2=2 in listdata
print(ret1);print(ret2)
strdata='abcde'
ret3='c' in strdata
ret4='j' in strdata
print(ret3);print(ret4)
~~~
<br><br>
~~~python
txt1='자바';txt2='파이썬'
num1=5; num2=10
print('나는 %s보다 %s에 더 익숙합니다.'%(txt1,txt2))
print('%s는 %s보다 %d배 더 쉽습니다.'%(txt1,txt2,num1))
print('%d + %d = %d' %(num1,num2, num1+num2))
print('작년 세계경제 성장률은 전년에 비해 %d%% 더 증가했다.'%num1)
~~~
<br><br>
~~~python
def add_number(n1,n2):
    ret = n1+ n2
    return ret

def add_txt(tx1,tx2):
    print(tx1+tx2)
    
ans = add_number(10, 15)
print(ans)

tx1 ='대한민국~'
tx2 ='만세!!'
add_txt(tx1, tx2)
~~~
<br><br>

~~~python
param = 10
strdata='전역변수'

def func1():
    strdata='지역변수'
    print(strdata)
    
def func2(param):
    param = 1
    
def func3():
    global param
    param = 50
    
func1()
print(strdata)
print(param)
func2(param)
print(param)
func3()
print(param)

    
~~~
<br><br>
~~~python
import py13

ret1 = py13.add_txt('대한민국', '1등')
ret2 = py13.reverse(1, 2, 3)

print(ret1)
print(ret2)
~~~
<br><br>
~~~python
def add_txt(t1,t2):
    return t1 + ':'+ t2

def reverse(x,y,z):
    return z,y,x


~~~
<br><br>
~~~python
import time

print('5초간 프로그램을 정지합니다.')

time.sleep(5)
print('5초가 지났습니다.')
~~~
<br><br>
~~~python
class MyClass:
    var='안녕하세요'
    def sayHello(self):
        print(self.var)
        
obj =MyClass()
print(obj.var)
obj.sayHello()
~~~
<br><br>
~~~python
try:
    print('안녕하세요.')
    print(param)
except Exception as e:
    print (e)
else:
    print('예외가 발생하지 않았습니다.')
finally:
    print('무조건 실행해야하는 코드')
  
~~~
<br><br>
~~~python
k =input('<값>을 입력하세요.')
print('당신이 입력한값은<'+k+'>입니다.')
~~~
<br><br>
~~~python
numdata =57
strdata='python'
listdata=[1,2,3]
def func():
    print('Hello')
    
print(type(numdata))
print(type(strdata))
print(type(listdata))
print(type(func))
  
~~~
<br><br>
~~~python
a = 11113
b =23
ret=a%b 
print('<%d>를 <%d>로 나누면 <%d>가 나머지로 남습니다.'%(a,b,ret))
  
~~~
<br><br>
~~~python
a =1113
b=23
ret1,ret2 = divmod(a,b)

print('<%d/%d>는 몫이 <%d> 나머지가 <%d>입니다.'%(a,b,ret1,ret2))
  
~~~
<br><br>
~~~python
ret1=round(1118)
ret2=round(16.554)
ret3=round(1118,-1)
ret4=round(16.554,2)

print(ret1)
print(ret2)
print(ret3)
print(ret4)
  
~~~
<br><br>
~~~python
def getPrime(x):
    if x%2 ==0:
        return 
    
    for i in range(3,int(x/2),2):
        if x % i == 0:
            break
    
    else:
        return x
    
listdata = [117,119,1113,11113,11119]
ret = filter(getPrime,listdata)
print(list(ret))
~~~
<br><br>

~~~python
listdata = [9.96, 1.27, 5.07,6.45, 8.38, 9.29]
maxval = max(listdata)
minval = min(listdata)
print(maxval);print(minval)

print('----------------------')

txt = 'Alotofthingsoccuerachday'
maxval = max(txt)
minval = min(txt)
print(maxval);print(minval)

print('----------------------')

maxval =  max(2+3, 2*3, 2**3, 3**2)
minval = min('abz','a12')
print(maxval);print(minval)
~~~
<br><br>

~~~python
txt1 = 'A tale that was not right'
txt2 = '이 또한 지나가리라'
print(txt1[5])
print(txt2[-2])

print('-----------------------')

print(txt1[3:7])
print(txt1[:6])
print(txt2[-4:])

~~~
<br><br>

~~~python
txt = 'This Is Python'

for i in range(len(txt)):
    print(txt[:i+1])
~~~
<br><br>

~~~python
txt = 'Hello World'
ret1=txt[::-1]
print(ret1)

ret2=txt[::-2]
print(ret2)

ret3 = txt[2::-2]
print(ret3)

~~~
<br><br>

~~~python
listdata = list(range(5))
ret1 = reversed(listdata)
print('원본리스트',end='');print(listdata);
listdata.reverse()
print(listdata)
print('역순리스트',end='');print(list(ret1))

ret2 = listdata[::-1]
print('슬라이싱 이용',end='');print(ret2)

~~~
<br><br>

~~~python
numstr = input('숫자를 입력하세요: ')
try: 
    num = int(numstr)
    print('당신이 입력한 숫자는 정수 <%d>입니다.'%num)
except:
    try:
        num = float(numstr)
        print('당신이 입력한 숫자는 실수<%f>입니다.'%num)
    except:
        print('++++숫자를 입력하세요~+++++')

~~~
<br><br>





