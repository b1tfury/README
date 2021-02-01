# README

This is a one page project, which talks about how to setup a simple README for any tech project be it
* Library
* Service
* Scripts

## Recommended Minimum Structure for a project

* Problem Description
* Dev environment setup
* Build instructions
* Run instructions

## Sample Readme for a plain java project.

# Project Description
As a fan of wealth, I want to model money which can be expressed in Rupees, paise or a combination thereof,  So that I can add and subtract values of money. I also want to print it on screen. Also we should be able to compare two money and sort them.

## Dev Environment Setup for OS X.
* Java v15
```
$ brew install java
```
At present(01/02/2021) it will directly install java 15. Please verify the version if you are using it later.

* Gradle v5.0

[To install gradle please refer](https://gradle.org/install/)

## Test instructions
```
$ ./gradlew clean test
```

## Build instructions
```
$ ./gradlew build
```

## Code Coverage instructions
```
$ ./gradlew clean build jacocoTestReport
```

## Code complexity
```
$ ./gradlew clean build check
```

### How to use
```
money1 = new Money(1, 20);
money2 = new Money(-2, -40);
money1.add(money2); 
```
Returns `new Money(-1, -20)`
<br>
```
money1 = new Money(1, 20);
money2 = new Money(-2, -40);
money1.subtract(money2); 
```
Returns `new Money(-3, -60)`
<br>
```
money = new Money(-1, -20);
money.toString();
```
Returns `"minus 1 rupee, 20 paise"`
<br>
```
Moneys moneys = new Moneys();
moneys.addMoney(new Money(1, 10));
moneys.addMoney(new Money(-1, -10));
moneys.addMoney(new Money(-1, -5));
moneys.sort();
```
Returns [`new Money(-1, -10)`,`new Money(-1, -5)`, `new Money(1, 10)`]
<br>
```
Money money1 = new Money(10,10);
Money money2 = new Money(20,20);
money1.compareTo(money2);
```
Returns `-1`

### Author
Sahil Kharb


