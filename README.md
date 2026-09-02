# PA2_ECE2112

Please take note that the following code was used in order to access the NumPy library.

    import numpy as np

## A. REPRODUCIBLE NORMALIZATION PROBLEM

**Objective:** The goal of this problem was to normalize a random 5x5 array and to get the mean and standard deviation of all the elements within that array.

**Discussion:**

To begin, the following statements were written in order to create the random 5x5 array. The initial randomized array is expressed as X.

    np.random.seed(2112)
    X = np.random.randint(10, 101, size=(5, 5))
    print(X)

To normalize the array, the following formula was used:

---

$$
Z = \frac{X - x̄}{σ}
$$

Where:

Z - Normalized Array

X - Randomized Array

x̄ - Mean of All Elements in Randomized Array

σ = Standard Deviation of All Elements in Randomized Array

***

Before using the equation, it is important to note that we should get the mean and standard deviation of all elements in the randomized 5x5 array we made.

In getting the mean of the randomized 5x5 array, the following statement was used:

    np.mean(X) #gets the mean of every element in an array
    print(np.mean(X))

In getting the standard deviation of the randomized 5x5 array, the following statement was used:

    np.std(X) #gets the standard deviation of every element in an array
    print(np.std(X))

After obtaining the mean and standard deviation of all elements in the randomized 5x5 array, we can now compute the normalized array.

To input the equation and to get the normalized array, the following statement was used. The normalized array is expressed as X_normalized.

    X_normalized = (X - np.mean(X)) / np.std(X)
    print(X_normalized)

Although we have the normalized array, it is part of the objective to get its mean and standard deviation.

This can be done by using the statements we used previously, but instead, we relay them to X_Normalized.

    print(np.mean(X_normalized))
    
    print(np.std(X_normalized))

*Do note that after normalizing the array, the standard deviation should always be equal to 1.

With this, I successfully created a normalized array and I was also able to get its mean and standard deviation.

The following statement was used to store the values in X_Normalized.

    np.save("X_normalized.npy", X_normalized)
    np.save

---

## B. CURVES DIVISIBLE BY 4

**Objectives:** The goal of this problem was to obtain elements that are divisible by 4 from a cubed 10x10 ndarray.

**Discussion:**

To set up the array, I listed down all the elements starting from 1 to 100.

    matrix = np.arange(1,101)
    print(matrix)

To cube the elements in the array, the array was exponentiated to 3.

    array = array ** 3
    print(array)

The following statement was used to reshape the array into a 10x10 array. This array would be expressed as C. Do note that it would not look like a true 10x10 array due to the numbers being too large, hence not fitting within the cell.

    C = array.reshape(10,10)
    print(C)

In order to get the elements that are divisible by 4, using Boolean conditions, I made it so that if an element has a remainder of 0 when it is divided by 4, it would be printed in the next array. This array would be expressed as div_by_4.

    div_by_4 = C[C % 4 == 0]
    print(div_by_4)

With this, I successfully obtained the elements that are divisible by 4 from a cubed 10x10 ndarray.

The following statement was used to store the values in div_by_4.

    np.save("div_by_4.npy", div_by_4)
    np.save

## C. ABOVE-MEAN SQUARE PROBLEM

**Objectives:** The goal of this problem was to obtain elements from a squared 6x6 ndarray that are larger than the mean of said ndarray.

**Discussion:**

To set up the array, I listed down all the elements starting from 1 to 36.

    array = np.arange(1,37)
    print(array)

To square the elements, the array was exponentiated to 2.

    array = array ** 2
    print(array)

The following statement was used to reshape the array into a 6x6 array. This array would be expressed as S.

    S = array.reshape(6,6)
    print(S)

The following statement was used to get the mean of the array. The mean would be expressed as S_mean.

    S_mean = S.mean()
    print(S_mean)

To 




























































