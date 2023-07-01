#!/usr/bin/python3

try:
    with open("tests/test00", "r") as file:
        lines = file.readlines()
        list_of_num = []
        for line in lines:
            list_of_num.append(int(line))
except Exception as e:
    print(e)
finally:
    file.close()


def findFactore(num):
    factors = []
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            factors.append(i)
            factors.append(num // i)
            break
    return factors

for num in list_of_num:
    factors = findFactore(num)
    if factors:
        print("{}={}*{}".format(num, factors[0], factors[1]))
