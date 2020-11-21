Sample Exercise
===============

Context
-------

If you own a dog, you've probably heard this rule: 1 year for doggy equals 7 years for you. 
Turns out, the math isn't that simple. Dogs mature more quickly than we do early on. 
So the first year of your fuzzy friend’s life is equal to about 15 human years.

Using the instructions below, you're going to create a calualtor that lets you accurately predict the age of doggies in human years.

Instructions
------------

* Write a function that returns the age of a dog as an integer in dog years. 
* The parameter can be a decimal number. E.g. 6.5 means six and a half actual years. A dog that is actually 6.5 years old is 51 in dog years.
* If the actual years is 2 or less, the dog’s age is twelve times the years.
* If the actual years is more than 2, the dog is 24 plus six for every year, minus two years.


Example Solution
----------------

~~~~

# Function to return dog years
def DogYears(Years):
    # Zero years is zero age
    if Years == 0:
        Age = 0
    # Less than 3, age is 12 times years
    elif Years <= 2:
        Age = 12 * Years
    else:
        # Otherwise age is years minus 2, multiplied by 6, plus 24
        Age = 24 + (6 * (Years -2))
    return Age

# Main program
print(DogYears(6.5))

~~~~

Learning Objectives Tested
--------------------------

* Learner will be able to effectively use number datatypes.
* Learner will be able to create and apply a function.
