# HackerRank
Resolução de problemas do site

[Loops](https://www.hackerrank.com/challenges/python-loops/problem?isFullScreen=true)

~~~python
if __name__ == '__main__':
    n = int(raw_input())
    
    lista = []
    for i in range(0, n):
        print(i**2)
~~~

[Write a function](https://www.hackerrank.com/challenges/write-a-function/problem?isFullScreen=true)

~~~python
def is_leap(year):
    leap = False
    
    # Write your logic here
    if not year%4:
        leap = True
    if not year%100:
        leap = False
    if not year%400:
        leap = True
    
    return leap

year = int(raw_input())
print is_leap(year)
~~~

[Print Function](https://www.hackerrank.com/challenges/python-print/problem?isFullScreen=true&h_r=next-challenge&h_v=zen)

~~~Python
from __future__ import print_function

if __name__ == '__main__':
    n = int(raw_input())
 
for i in range(1,n+1):
    print(i, end='')
~~~

[What's your name?](https://www.hackerrank.com/challenges/whats-your-name/problem?isFullScreen=true)

~~~Python
def print_full_name(a, b):
    print ("Hello " + a + " " + b + "! You just delved into python.")

if __name__ == '__main__':
    first_name = raw_input()
    last_name = raw_input()
    print_full_name(first_name, last_name)
~~~

[Mutations](https://www.hackerrank.com/challenges/python-mutations/problem?isFullScreen=true&h_r=next-challenge&h_v=zen)

~~~Python
def mutate_string(string, position, character):
    
    aux_list = list(string)
    aux_list[position] = character
    string = ''.join(aux_list)
    
    return string

if __name__ == '__main__':
    s = raw_input()
    i, c = raw_input().split()
    s_new = mutate_string(s, int(i), c)
    print s_new
~~~

[String Validators](https://www.hackerrank.com/challenges/string-validators/problem?isFullScreen=true)

~~~Python
if __name__ == '__main__':
    s = raw_input()
    
    a, b, c, d, e = False, False, False, False, False
    
    
    for i in range(len(s)):
        if s[i].isalnum():
            a = True
    
        if s[i].isalpha():
            b = True
        
        if s[i].isdigit():
            c = True
            
        if s[i].islower():
            d = True
        
        if s[i].isupper():
            e = True    
            
    print(a)
    print(b)
    print(c)
    print(d)
    print(e)
~~~

[sWAP cASE](https://www.hackerrank.com/challenges/swap-case/problem?isFullScreen=true)

~~~python
def swap_case(s):
    
    aux = ""
    for i in range(len(s)):
        if(s[i].isupper()):
            aux += s[i].lower()
        elif(s[i].islower()):
            aux += s[i].upper()
        else:
            aux += s[i]
    
    return aux

if __name__ == '__main__':
    s = raw_input()
    result = swap_case(s)
    print result
~~~

[String Split and Join](https://www.hackerrank.com/challenges/python-string-split-and-join/problem?isFullScreen=true&h_r=next-challenge&h_v=zen)

~~~Python
def split_and_join(line):
    a = "-".join(line.split(" ")) 
    return a
    
if __name__ == '__main__':
    line = raw_input()
    result = split_and_join(line)
    print result
~~~

[Mod Divmod](https://www.hackerrank.com/challenges/python-mod-divmod/problem?isFullScreen=true)

~~~Python
a = int(input())
b = int(input())

print(a // b)
print(a % b)
print(divmod(a, b))
~~~

[Power - Mod Power](https://www.hackerrank.com/challenges/python-power-mod-power/problem?isFullScreen=true&h_r=next-challenge&h_v=zen)

~~~Python
a = int(input())
b = int(input())
m = int(input())

print(pow(a, b))
print(pow(a, b, m))
~~~

[Integers Come In All Sizes](https://www.hackerrank.com/challenges/python-integers-come-in-all-sizes/problem?isFullScreen=true&h_r=next-challenge&h_v=zen&h_r=next-challenge&h_v=zen)

~~~Python
a = int(input())
b = int(input())
c = int(input())
d = int(input())

print(a**b + c**d)
~~~

[Capitalize!](https://www.hackerrank.com/challenges/capitalize/problem?isFullScreen=true)

### Não funcionou para todos os casos por enquanto :c

~~~Python
def solve(s):
    lista = s.split()
    
    aux = []
    for item in lista:
        aux.append(item[0].upper())
        for i in range(1, len(item)):
            
            aux.append(item[i])
        
        aux.append(" ")    
    
    s = ''.join(aux)
    return s
~~~
