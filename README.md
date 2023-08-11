# block18-Writting-Test-Specs

## Prompts
For each prompt below: 

Read the prompt.</br>
Identify the expectations.</br>
Write specifications in pseudocode/plain English for all the tests that would be useful for that prompt.</br>
Try to take any "edge cases," or unexpected circumstances, into account, and write test specs for them.</br>
Try not to write extraneous tests!</br>

## Unit Tests
### mulitplication
A function called "multiplication" that returns the product of the two input numbers.

### my pseudocode for mulitplication
-expect mulitplication(x,y) to be a number</br>
-expect multiplication(5,10) to be equal to 50</br>
-expect multiplication("b",2) to be an error</br>
-expect multiplication() to be an error</br>
-max of 2 paramaters</br>

### concatOdds
A function called "concatOdds" takes two arrays of integers as arguments. It should return a single array that only contains the odd numbers, in ascending order, from both of the arrays.
Example: concatOdds([3, 2, 1], [9, 1, 1, 1, 4, 15, -1])
...should result in [-1, 1, 3, 9, 15]</br>
Think about the following; you may need to make assumptions or decisions about the prompt and how the code should behave:</br>
What should happen with unexpected inputs?</br>
What kinds of unexpected inputs should we worry about?</br>
What should happen when there are multiples of the same odd number in the arrays? (Hint: We gave you the answer to this one in the example above.)</br>

### my pseudocode for concatOdds()
-expect concatOdds to be a number</br>
-expect concatOdds([3,2,1],[9,1,1,1,4,15,-1]) to be [-1,1,3,9,15]</br>
-expect concatOdds to only return one number if there are multiples of the same value</br>
-expect concatOdds() to be undefined or throw an error</br>
-expect concatOdds([3,"2","1"],["9",1,1,1,"4",15,"-1"]) to be converted to throw an error</br>
-expect ConCatOdds([3,2,1],[9,1,1,1,4,15,-1]) to throw a reference error</br>
-expect concatOdds to be an array of numbers that are listed in the two paramater arrays</br>
-expect concatOdds to be an array in ascending order</br>

## Functional Test
A shopping cart checkout feature that allows a user to check out as a guest (without an account), or as a logged-in user. They should be allowed to do either, but should be asked if they want to create an account or log in if they check out as a guest.</br>
Think about the following; you may need to make assumptions or decisions about the prompt and how the feature should behave:</br>
What should happen if the cart is empty?</br>
What needs to be shown to the user at each step of check out?</br>
What behaviors of this feature does the prompt miss or gloss over?</br>
Hint: Observe the shopping cart and checkout features of some popular websites to get some ideas!</br>

### my pseudocode for shopping cart
-if shopping cart is  empty user should be able to log in on the shopping cart page to see their saved items</br>
-if the shopping cart is empty the user should be able create account on the shopping cart page</br>
-if user is not signed in they should be promted to sign in or continue as a guest</br>
-if user is on the shopping cart page they should see an order summary and a button to checkout</br>
-if user is creating an account they should be allowed to sign in using google or facebook if that website allows that type of account managment instead of siging up through the direct website</br>
-if the user is signed in they should be able to see the saved items in their account or shopping cart</br>
-if the user is using guest mode they should be able to see the items in their cart for at least an hour without signing in</br>
-if the user is in guest mode they should be allowed to create an account at anytime in the process before checkout or during checkout </br>
-the user should be able to see the options for form of payment ie: credit,paypal,apple card in either guest or account mode</br>
-if the user trys to sign in and enters an incorrect password or user name an error should alert them and if they want to change their passwords they should follow the prompts</br>
-if while signing up for an account they enter an incorrect email or password an alert should notify the user</br>
