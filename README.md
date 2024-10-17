# Homework_8.1


def add_one(some_list):
    num = int(''.join(map(str, some_list)))
    
    num += 1
    
    result = [int(digit) for digit in str(num)]
    
    return result

assert add_one([1, 2, 3, 4]) == [1, 2, 3, 5], 'Test1'
assert add_one([9, 9, 9]) == [1, 0, 0, 0], 'Test2'
assert add_one([0]) == [1], 'Test3'
assert add_one([1, 0]) == [1, 1], 'Test4'

print("Все тесты пройдены!")
