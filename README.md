def fibonacci(n):
    if n <= 0:
        return "Input should be a positive integer."
    elif n == 1:
        return 0
    elif n == 2:
        return 1
    else:
        a, b = 0, 1
        for _ in range(n - 2):
            a, b = b, a + b
        return b

# Test the function
print(fibonacci(1))  # 0
print(fibonacci(2))  # 1
print(fibonacci(3))  # 1
print(fibonacci(4))  # 2
print(fibonacci(5))  # 3
print(fibonacci(6))  # 5
print(fibonacci(7))  # 8
print(fibonacci(8))  # 13
print(fibonacci(9))  # 21
print(fibonacci(10)) # 34
print(fibonacci(-1)) # Input should be a positive integer.
