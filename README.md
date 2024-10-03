# Introduction

![image](https://imgs.xkcd.com/comics/nerd_sniping.png) 

(source: https://xkcd.com/356/)


My brain gets a sudden urge of _epistemic curiosity_ sometimes. A question pops up in my head, and I have to drop everything I'm doing at that point, and look up an answer immediately. Some sort of **brain q & a** :-)


**Most** of the time, after reading the answer, I immediately forget afterwards...
**Sometimes**, they're interesting enough I want them to stick, so  I add them here...
**Lastly**, if an answer makes me ask even more questions, i'll follow-up with some _follow-up_ questions.

# Q & A

## Question 1 : What is the difference between a statement a block, and an expression in Java?

An _expression_ is any construct in java that produces a singular value.

```java
1 == 1
```

```java
    int numLetters = 0;
    Day day = Day.WEDNESDAY;
    switch (day) {
        case MONDAY, FRIDAY, SUNDAY -> numLetters = 6;
        case TUESDAY                -> numLetters = 7;
        case THURSDAY, SATURDAY     -> numLetters = 8;
        case WEDNESDAY              -> numLetters = 9;
        default -> throw new IllegalStateException("Invalid day: " + day);
    };
    System.out.println(numLetters);
```

A _statement_ is a complete unit of execution_

```java
var x = "Foo";
```

A _block_ is a group of zero or more _statements_

```java
{
var x = "foo";
var y =  "bar";
}
```

