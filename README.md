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

