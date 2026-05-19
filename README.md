# Prime number calculator

## Installation
Using **uv**: 
```bash
uv add prime-number-calculator
```
Using **pip**: 
```bash
pip install prime-number-calculator
```

## Examples
```python
number=int(input())

# Checks if the number is a prime number
from prime_number import prime_number
print(prime_number(number))

# Returns the smallest prime factor of the number
from prime_number import submultiple
print(submultiple(number))

# Decomposes the number into a product of prime factors
from prime_number import prime_factorization
print(prime_factorization(number))
```

## Introduction
This algorithm is much faster for positive integers less than 10<sup>16</sup> comparing with the classical ones such as: 
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
