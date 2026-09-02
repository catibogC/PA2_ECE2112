# PA2_ECE2112

Please take note that the following code was used in order to access the Numpy library.

    import numpy as np #changes numpy to np

## A. REPRODUCIBLE NORMALIZATION PROBLEM

**Objective:** The goal of this problem was to normalize a random 5x5 array and to get the mean and standard deviation of all the elements within that array.

**Discussion:**

To begin, the following statements were written in order to create the random 5x5 array.

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

---

Before using the equation, it is important to note that we should get the mean and standard deviation of all elements in the randomized 5x5 array we made.

In getting the mean of the randomized 5x5 array, the following statement was used:

    np.mean(X) #gets the mean of every element in an array
    print(np.mean(X))

In getting the standard deviation of the randomized 5x5 array, the following statement was used:

    np.std(X)
    print(np.std(X))

After getting the values for the mean and standard deviation of all the elements in the randomized 5x5 array, we can now 









































































