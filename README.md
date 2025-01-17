# Types Variables Logic and Operations Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab  - 
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link of your Fork on Canvas and submit

## 1. Which of the following variables/constants are declared correctly?  Select all that apply.

```swift
a. let nameOfPrincipal: Character = "Mrs. Watkins"

b. var temperatureOutside: Int = 90.7

c. var isSummer: String = false

d. let whiteHouseAddress: Int + String = 1600 + "Pennsylvania Ave"

e. var peopleAtParty: Double = "95"




//// Answer: all of the above are declared incorrectly!
```


***
## 2. Which of the following expressions evaluate to true?

```swift
a. !(4 + 3 < 2 * 4)

b. !(1 + 1 != 2) && !(3 >= 3)

c. (3 < 2 || (0 < 1 && 3 >= 3)) && true

d. !!(!!true && !!false)

e. true && (true && (true && (true || false)))


//// Answer: C , E .
```

***
## 3. Mad-Libs! Add a value to the declared variables below in playgrounds. Insert the variables (already in correct order) inside the stringmadLib and print. 

```swift


var geographicLocation: String
var adjective1: String
var pluralNoun1: String
var adjective2: String
var pluralNoun2: String
var number1: Int
var number2: Int
var articleOfClothing: String

var madLib = "Here is tomorrow's weather report for \()
and vicinity. Early tomorrow, a \()-front will
collide with a mass of hot \() moving from the
north. This means we can expect \() winds and
occasional \() by late afternoon. Wind velocity will
be \() miles an hour, and the high temperature should
be around \() degrees. So, if you're going out, you had
better plan on wearing your \()".


//// Answer in Code: var madLib = "Here is tomorrow's weather report for \(geographicLocation) and vicinity. Early tomorrow, a \(adjective1)-front will collide with a mass of hot \(pluralNoun1) moving from the north. This means we can expect \(adjective2) winds and occasional \(pluralNoun2) by late afternoon. Wind velocity will be \(number1) miles an hour, and the high temperature should be around \(number2) degrees. So, if you're going out, you had better plan on wearing your \(articleOfClothing)"
print("Welcome to Tiffany's Weather Channel. \(madLib)")

////Answer in print:Welcome to Tiffany's Weather Channel. Here is tomorrow's weather report for Brooklyn NY and vicinity. Early tomorrow, a cool-front will collide with a mass of hot sun showers moving from the north. This means we can expect strong winds and occasional showers by late afternoon. Wind velocity will be 15 miles an hour, and the high temperature should be around 70 degrees. So, if you're going out, you had better plan on wearing your hoodie

YAY I DID IT!!!! lol 
```

***
## 4. You are given two variables a and b, compute their sum and store it in another variable named sum then print the result.

```swift

Example 1
Input:
var a = 1
var b = 2

Expected values:
sum = 3

Output: 
3

        //// Answer in Code:
                            var a = 1
                            var b = 2
                            var sum = a + b
                            print("the answser is \(sum)")

        //// Answer in print: 
        the answser is 3



Example 2
Input:
var a = 13
var b = 22

Expected values: 
sum = 35

Output:
35

        //// Ansswer in code:
                            var a = 13
                            var b = 22
                            var sum = a + b
                            print("the answser is \(sum)")

        //// Answer in print:
                            the answser is 35
```

***
## 5.Determine the number of seconds in a year and store the number in a variable named secondsInAYear.

```swift
Hint:
The number of seconds in a year is 365 times the number of seconds in a day.
The number of seconds in a day is 24 times the number of seconds in a hour.
The number of seconds in a hour is 60 times the number of seconds in a minute, which is 60.

        //// Answer: 

            var secondsInAYear = 60 * 60 * 24 * 365 
 orrr
                let min = 60
                let hour = 60 
                let day = 24
                let year = 365

            var secondsInAYear = min * hour * day * year 

            var secondsInAYear = 31,536,000
```

***
## 6. Your are given the width and height of a screen in pixels. Calculate the total number of pixels on the screen and store the result in a variable named numberOfPixels.

```swift


Example 1
Input: 
var width = 4
var height = 3

Expected values:
numberOfPixels = 12


        ////Answer:

            var width = 4
            var height = 3

            var numberOfPixels = width * height 

////or

            var numberOfPixels = 12 


Example 2
Input:
var width = 1920
var height = 1080

Expected values:
numberOfPixels = 2073600

        ////Answer:

                var width = 1920
                var height = 1080

                var numberOfPixels = width * height

or 

                var numberOfPixels = 2073600




Hint:
Consider a 5x3 screen like this:
*****
*****
*****

The number of pixels on this screen is 5+5+5 = 5*3


```

***
## 7. You are given the sum and the difference of two numbers. Find out the values of the original numbers and store them in variables a and b.

```swift
let sum = 16 // a + b 
let diff = 4 // a - b

Example 1
Input: 
var sum = 16 
var dif = 4

Expected values:
a = 10
b = 6


            ///// Answer: var a = (diff + sum)/2
                          var b = a - diff  

Example 2
Input:
var sum = 2 
var dif = 0

Expected values:
a = 1
b = 1
            ////// Answer: var a = (sum + diff)/2
                           var b = sum - a 

Hint:
sum + diff = a + a + b - b
sum + diff = 2 * a
```

***
## 8. Given two variable a and b, swap their values. That is the new value of a will become the old value of b and vice versa.

```swift
var a = 1
var b = 2

Example 1
Input: 
a = 2
b = 1

Hint:
Just assigning a to the value of b and b to the value of a will not work.

var a = 1
var b = 2

a = b // a will have the value 2. The original value of a is lost
b = a // b will remain the same


            //// Answer: var a = 1
                         var b = 2
                         var bb = 1
             
                in order to switch we make var a = b ; and var b = bb 
```

***
## 9. You are given a number a. Print the last digit of a.

```swift
var a = 123

Example 1
Input: 
var a = 123

                ///// Answer: 
                var a = 123
                var k = 10

                var answer = a % k


Output:
3

Example 2
Input: 
var a = 337

                ///// Answer: 
                var a = 337
                var k = 10

                var answer = a % k


Output:
7

Hint:
Use the remainder % operator.
Remember that a = k * (a / k) + a % k
Can you think of a value for k that gives the last digit?

```

***
## 10. You are given Rocky’s age in dog years. Print Rocky’s age in human years. You know that 1 human year is 7 dog years.

```swift

Example 1
Input: 
var rockysAge = 50

            //// Answer:
                        var rockysAge = 50 
                        var oneHumanYear = 7

                        var rockyHumanYears: Int = rockysAge / oneHumanYear

Output:
7

```

***
## 11. Everyone hates solving word problems by hand so let’s make a program to solve them for us. 
### x years from now Alice will be y times older than her brother Bob. Bob is 12 years old. How many years does Alice have?

```swift

Example 1
Input: 
var x = 3
var y = 2
var bob = 12

        ///// Answer = 
                        var alice = y * (bob + x) - x

Expected values: 
alice = 27


Example 2
Input: 
var x = 1
var y = 3
var bob = 12

Expected values: 
alice = 38

        ///// Answer =
                        var alice = y * (bob + x) - x
Hint:
alice + x = y * (bob + x)
Solve for alice

```

***
## 12. You have x apples. Bob trades 3 oranges for 5 apples. He does not accept trades with cut fruit. How many oranges can you get from Bob and how many apples will you have left? The number of apples you will have left should be stored in a variable named apples. The number of oranges you will have after the trade should be stored in a variable named oranges.

```swift
var x = 17

Example 1
Input: 
var x = 17

Expected values: 
apples = 2
oranges = 9

Example 2
Input: 
var x = 25

Expected values: 
apples = 0
oranges = 15

////Answer : var apples = x % 5
                 oranges = (x/5) * 3

Hint:
Use the division(/) and the remainder(%) operator

```

***
## 13. A class consists of numberOfBoys boys and numberOfGirls girls.
### Print the percentage of boys in the class followed by the percentage of girls in the class. The percentage should be printed rounded down to the nearest integer. For example 33.333333333333 will be printed as 33.

```swift
var numberOfBoys = 20
var numberOfGirls = 60

Example 1
Input: 
var numberOfBoys = 20  
var numberOfGirls = 60

                /////Answer:

                var numberOfBoys = 20
                var numberOfGirls = 60



                var totalClass = numberOfBoys + numberOfGirls
                var percentOfBoys = Int ((numberOfBoys * 10) / (totalClass / 10))
                var percentOfGirls = Int ((numberOfGirls * 10) / (totalClass / 10))
            
        

Output:
25 // percentage of boys
75 // percentage of girls

```

***
## 14.Which of the following expressions evaluate to true?

```swift
a. false || true
b. false && true
c. !false
d. !!!true
e. !(true && true)

                /////Answer: A, C, 

```

***
## 15.Which of the following expressions evaluate to true?

```swift
a. 3 < 12.3
b. 9 == 2
c. "Hello!" == "Hello!"
d. 19.0 >= 19.0
e. 9 > 7 && 7 < 10

                    ///// Answer A, C, D, E
```

