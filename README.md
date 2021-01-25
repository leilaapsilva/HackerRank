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
