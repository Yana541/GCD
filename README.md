
# Euclidean Algorithm for GCD

## Description

The Euclidean Algorithm is a method for finding the Greatest Common Divisor (GCD) of two non-negative integers, denoted as `gcd(a,b)gcd(a,b)`. In English, GCD stands for "greatest common divisor," and it is commonly represented by the notation gcdgcd.

The GCD of two numbers is the largest number that divides both of them. If one of the numbers is zero and the other is non-zero, their GCD is the non-zero number. When both numbers are zero, the GCD is undefined, and in this case, we consider it to be zero. Therefore, a general rule is that if one of the numbers is zero, the GCD is equal to the second number.

The Euclidean Algorithm, presented below, efficiently computes the GCD of two numbers aa and bb in `O(log⁡min⁡(a,b))O(logmin(a,b))` time complexity.

This algorithm was first described in Euclid's book "Elements" around 300 BCE, although it might have earlier origins.
## Algorithm
The algorithm is remarkably simple and can be described by the following formula:

![изображение](https://github.com/Yana541/GCD/assets/149325426/e4ce82d2-b769-423c-b785-884d40cbf459)

The steps of the algorithm are as follows:

1. Start with two non-negative integers ` a ` and ` b `.
2. If ` b ` is equal to zero, return ` a ` as the GCD.
3. Otherwise, replace `a ` with ` b ` and ` b ` with the remainder of the division `a ` by `b`.
4. Repeat steps 2 and 3 until `b ` becomes zero.
5. Return `a `, which is now the GCD of the original ` a ` and `b`.

## Example

Let's take an example where `a = 48 ` and `b = 18 `.

Step 1: `b ` is not zero, proceed to the next step.

Step 2: `gcd(a, b)` = `gcd(18, 48 \mod 18)` = `gcd(18, 12) `.

Step 3: ` b ` is not zero, proceed to the next step.

Step 4: `gcd(a, b)` = `gcd(12, 18 \mod 12)` = `gcd(12, 6)`.

Step 5: ` b ` is not zero, proceed to the next step.

Step 6: `gcd(a, b)` = `gcd(6, 12 \mod 6)` = `gcd(6, 0)`.

Step 7: `b ` is zero, return `a = 6`.

Therefore, `gcd(48, 18) = 6`.

