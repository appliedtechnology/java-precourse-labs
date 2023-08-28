# Testing Testing!

## Info

No matter how great you are at coding, you cannot truly guarantee it will do what it should until you run it. Be honest, how many times have you manually tested your code to check that it's doing what it should? Manual testing has its charm, it's fun to see that what you are building works the way it should, but It's slow and takes up valuable time (yours!).

There is a better way! By writing `tests` that validate that for a certain input, we get the correct output, we can have the code test itself! Running lighnitng quick and can be run over and over and over and over...

It's not uncommon for tests to run hundreds of times a day, giving you quick immediate feedback for when something breaks. No more "Wait, when did that stop working"! 

One way to do testing is through unit testing. Unit tests verify the behavior of individual units of code in isolation (like functions or methods). Java has a popular framework for unit testing named JUnit.
For this lab, you'll integrate JUnit with your Maven project to test your calculator's functionality.

## What you will be working on

For this lab, you'll integrate JUnit with your previous calculator Maven project to test your calculator's functionality.

## Resources

- [Arrange, Act, Assert](https://java-design-patterns.com/patterns/arrange-act-assert/)
- [Unit Testing, best practices](https://www.baeldung.com/java-unit-testing-best-practices)
- [TDD, Red, Green, Refactor](https://www.codecademy.com/article/tdd-red-green-refactor)

## Lab instructions

### Should we set up the correct JUnit version?

The versions of dependencies that came with the previous project are old, but it will do for now.

### Writing out test
 
You did actually make a test in the last lab! Browse `src/test/java/<your>/<group>/AppTest.java`, to see it. Good stuff here, we make sure that the value of `true` is `true`. Let's make it into something more useful!

1. Rename the class and file to something more fitting such as e.g. `CalculatorTest`. It's important that the class name either starts or ends with `test` or `tests`, since [else Maven will not find it](https://www.vogella.com/tutorials/JUnit/article.html#junit_namingconventions_maven).

1. **Act** upon one of your methods inside the Calculator class, and **Assert** that the result is what is to be expected.

1. Run the test with the command `mvn test`.

**Congratulations!** You have just written and executed your possibly first test!

### Test Driven Development:

Now that we have a test up and running. Let's try out doing some **Test Driven Development**. TDD is a way of writing code by so-called "wishful coding", following the `Red, Green, Refactor` pattern.

The steps to follow for TDD are as follows:

1. Write the test for what you want to implement, and make sure it fails.  - **Red**

1. Write the most simple solution possible in order to make it pass. - **Green**

1. Refactor the code and possibly the test in order to make it better. - **Refactor**

1. Write more tests!

The advantage of following this approach is that you need to think more about how your code should act and end up with more testable code! Let's try it out. You will be running the command `mvn test` quite a lot!

1. Write a new test for a method called `makeNegative`. Have it assert that for any positive input, return the negative equivalent. Eg. for the input `42`, you should assert that the result is `-42`. Make sure it fails when you run!

1. Make the test pass by implementing the method in the most simple way possible (hint, you are allowed to just return `-42`, that makes the test pass).

1. Write another test, make sure it fails, and then make it pass.

1. Write a test to ensure that for negative numbers, the method returns that negative number. Eg. for `-42`, `-42`. Make sure it fails and then make it pass.

## Conclusion

Nice work! Testing is a vital part of software development and throughout the course, we will dig deeper into the concepts of Unit Testing, Integration Testing, and End-2-End Testing.

## Extra: Should we set up the correct JUnit version?

The versions of dependencies that came with the previous project are old, but it will do for now. If you would like a challenge, see if you can migrate it to Java version 20 and the latest versions of each dependency. Here is the [latest version of JUnit to get you started](https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api/5.10.0).

## Conclusion

Great going! We have dipped our toes in the Maven ocean, and crested and compiled a Java project without any help of other additional software. If you look at the bottom of your file browser in VS-Code, you can see that there are a lot more commands that can be used.

![Maven commands](maven.png)

We will explore these more and more as we proceed. The next lab in specifically will take a look at testing! Look forward to it!
