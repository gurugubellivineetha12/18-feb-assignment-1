def count_Primes_nums(n):
    count = 0
    
    for num in range(n):
        if num <= 1:
            continue
        for i in range(2, num):
            if (num % i) == 0:
                break
        else:
            count += 1

    return count

print(count_Primes_nums(10))
print(count_Primes_nums(100))
