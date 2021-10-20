n = int(input("Enter No of Score: "))
if 2 <= n <= 10:
    A = list(map(int, input("Enter Scores(Scores should be between - 100 and 100) separated by a space between them: ").split()))
    # Scores should be between - 100 and 100
    if (min(A) >= -100) and (max(A) <= 100):
        A.sort()
        highest = max(A)
        for i in range(0, n):
            if highest > A[i] > -100:
                runners_up = A[i]
        print(runners_up)
    else:
        exit()
else:
    exit()
