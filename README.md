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
