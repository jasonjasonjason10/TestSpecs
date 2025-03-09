# TestSpecs

Function: Multiplication

-Expect multiplication(4, 5) to be a number 
-Expect multiplication(4, 5) to equal to 20 
-Expect multiplication(-4, 5) to equal -20
-Expect multiplication(0, 7) to equal 0
-Expect multiplication(2, 1.5) to equal 3
-Expect multiplication("x, 7) to be an error
-Expect multiplication(null, 4) to be an error
-Expect multiplication(3) to be an error
-Expect multiplication(6, 3, 9) to be an error
-Expect multiplication([], {}) to be an error

Funtcion: contactOdds
-Expect contactOdds([8, 4, 7], [-2, -4, 4, 9]) to return ([-4, -2, 4, 7, 8, 9])
-Expect contactOdds([], []) to return []
-Expect contactOdds([2, 5,8], [8,10, 12]) to return []
-Expect contactOdds ([6, 7, 3], [3, 7, 6]) to return [3, 6, 7] (duplicates moved and sorted)
-Expect contactOdds([9, 10, 12] [12, 18, 20]) to return [9, 10, 12, 18, 20]
-Expect contactOdds([1, "a", 3], [5, "b", 7]) to return [1, 3, 5, 7] (ignoring non-numeric values)
-Expect contactOdds``([1, null, 3], [5, undefined, 7]) to return [1, 3, 5, 7] (ignoring null/undefined value)
-Expect contactOdds(1, [3, 5]) to be an error
-Expect contactOdds([3, 5], "test") to be an error

Feature: Shopping CArt Checkout

-When a user attempts to checkout with an empty cart, they should see a message stating that their cart is empty and should not proceed further

-When a guest user checks out, they should be given the option to log in or continue as a guest

-When a guest user proceeds with checkout, they should be prompted to enter their shipping and payment details

-When a guest user completes checkout, they should be given the option to create an account

-When a logged-in user checks out, their saved shipping and payment details should be pre-filled, but editable

-When a logged-in user completes checkout, they should be shown an order confirmation page

-When a user provides invalid payment details, they should see an error message and be prompted to correct the information.

-When a user provides an invalid shipping address, they should see an error message and be prompted to correct the information

-When a user applies a valid discount code, the total price should update accordingly

-When a user applies an invalid or expired discount code, they should see an error message

-When a user successfully places an order, they should receive an email confirmation