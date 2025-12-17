# Prime number calculator

## Installation
Please copy the file 'prime_number.py' and put it in 'Python\Lib\site-packages'.

## Examples
```python
number=int(input())

from prime_number import prime_number
print(prime_number(number))

from prime_number import submultiple
print(submultiple(number))

from prime_number import prime_factorization
PF=prime_factorization(number)
if eval(str(PF).replace('{','').replace('}','').replace(': ','**').replace(', ','*'))==number:
    print(PF)
else:
    print('error')
```

## Introduction
This algorithm is much faster for positive integers less than 10^16 than the classical ones such as: 
```python
def isPrime(N):
    if N%2==0 and N-2:
        return False
    else:
        for n in range(3,int(N**0.5)+1,2):
            if N%n==0:
                return False
        return True
```
