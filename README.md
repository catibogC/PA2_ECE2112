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

---

##B. CURVES DIVISIBLE BY 4

**Objectives:** The goal of this problem was to obtain elements from a cubed 10x10 array that are divisible by 4.






































































