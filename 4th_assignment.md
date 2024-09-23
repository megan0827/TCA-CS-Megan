# TCA-CS-Megan
목표
- 함수 작성하는 방법 배우기

코드 구현 설명
● 덧셈 함수 구현
- def sum(a, b):
    return (a + b)

a = int(input('Enter 1st number: '))
b = int(input('Enter 2nd number: '))

print(f'Sum of {a} and {b} is {sum(a, b)}')

결과: ![unnamed](https://github.com/user-attachments/assets/0d5a3c57-5f82-414c-b0c9-45acc9f5caac)

+ 연산자를 사용하여 덧셈 연산을 처리했습니다.

● 이름 출력 함수 구현
def greet (name):
    return (f"Hello, {name}!")
print(greet("Alice")) # Hello, Alice!

결과: ![unnamed-1](https://github.com/user-attachments/assets/aa437e78-7845-4205-adbc-1733f8fb2d27)

{name}을 이용하여 해당 이름을 포함한 인사말을 출력했습니다.

● 최대값 함수 구현
def find_max(a,b,c):
    return max(a, b, c)
result = find_max(10, 20, 30)
print(f"최댓값: {result}")

결과: ![unnamed-2](https://github.com/user-attachments/assets/b5efd683-3150-4643-9c6c-c24b365d1fc0)

max() 함수를 이용하여 3개의 숫자 중 가장 큰 숫자를 출력했습니다. 

● 단어 길이 계산 함수 구현 
def word_length(word):
    return len(word)  
    
length = word_length("Hello, World!")
print(f"문자열의 길이: {length}")

결과: ![unnamed-3](https://github.com/user-attachments/assets/589a2b23-9d85-4a88-b4e5-284b83ba5a3d)

입력된 문자열 (word)의 길이를 계산해서 출력했습니다. 

● 리스트 평균 함수 구현
def average(numbers):
    
    total = sum(numbers)  
    count = len(numbers)  
    avg = total / count 
    return avg
numbers = [10, 20, 30, 40, 50]
result = average(numbers)
print(f"리스트의 평균값: {result}")

결과:![unnamed-4](https://github.com/user-attachments/assets/0a0d8b62-da22-42d6-bb81-9a5328666bf8)

sum(numbers)를 사용하여 숫자들의 합을 구했고, len(numbers)를 사용하여 숫자들의 갯수를 구했습니다. 

● 팩토리얼 함수 구현
def factorial(n):
    if n == 0 or n == 1:  
        return 1
    else:
        return n * factorial(n - 1)  
result = factorial(5)
print(f"5! = {result}")

결과: ![unnamed-5](https://github.com/user-attachments/assets/5a3ce25e-7922-4a8f-bd42-17e4f8683994)

n이 0이거나 1이면 팩토리얼 값이 1이고 2 이상이면 n * factorial(n - 1)을 계산했습니다. 

● 피보나치 수열 함수 구현
def fibonacci(n):
    if n == 0:
        return 0  
    elif n == 1:
        return 1  
    else:
        return fibonacci(n - 1) + fibonacci(n - 2)  
result = fibonacci(7)
print(f"피보나치 수열의 7번째 값: {result}")

결과:![unnamed-6](https://github.com/user-attachments/assets/12787512-9231-4391-a33e-ee90cfdf7238)

n=0이면 0 반환, n=1이면 1 반환, n이 2 이상이면 fibonacci(n - 1) + fibonacci(n - 2)를 계산하여 n번째 피보나치 수를 반환했습니다.

어려웠던 점이나 해결 방법
- 리스트 평균 함수, 팩토리얼 함수, 피보나치 수열 함수는 작성하는 데 어려움이 있어서 ChatGPT를 사용했습니다. 

ChatGPT 사용 내역
- 리스트 평균 함수, 팩토리얼 함수, 피보나치 수열 함수를 작성할 때 사용했습니다. 
