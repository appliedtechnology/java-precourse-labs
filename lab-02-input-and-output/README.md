# Command line calculation

## Info

Maven is a build tool used by Java developers, there to make us able to do common tasks such as compile code, test, deploy and manage the dependencies. Since it's relseased in 2004, it has been incredibly influential and established a standard for how to setup projects in Java.

Getting comfortable working with Maven is essential, so today we are going to make a small command line application, using VS Code and maven cli. We will NOT be using IntelliJ today!

## What you will be working on

You'll be building a Maven project from scratch to create a CLI calculator that can perform basic arithmetic operations. It will be clunky and virtually no-one does it this way anymore, but doing it the manual way gives us more understanding of what our IDE is doing for us.

Do not worry if you get stuck or do not know how to proceed immedietly, these labs are made to not hold your hand 100% of the time. You can always ask for help, seach for guides online and take a break. Only thing we do not recommend is asking AI, since that will ruin the excersise.

## Setup

Ensure you have the following tools installed:

- [Java Development Kit \(JDK\)](https://www.oracle.com/java/technologies/downloads/#jdk20-windows)
- Apache Maven
- [VS Code Java Extension Pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)

## Resources

- [Maven in 5 minutes](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html)
- [How to install Maven on Windows](https://phoenixnap.com/kb/install-maven-windows)

## Lab instructions

The end goal of this lab is to be able to run the following commands
```bash
java -cp <jar-file> <class-path> 1 2 add
> 3
java -cp <jar-file> <class-path> 9 2 multiply
> 18
java -cp <jar-file> <class-path> 3 2 subtract
> 1
java -cp <jar-file> <class-path> 10 2 divide
> 5
```

#### Creating out Maven project

1. In your terminal or command prompt, navigate to your preferred directory and create a new Maven project via the CLI command `mvn archetype:gener... <you fill in the rest>`

1. Navigate into the new project directory, add the .gitignore file from this repo [.gitignore](.gitignore) and then, make the project into a new `git` repo via the command `git init`

1. Then, open up the project with `code .`

#### Creating a CLI Calculator

*Tip! Remember to commit small and often as you go! Building up good git routines*

1. Create a new Class names `Calculator` in the src/main/java/\<your\>/\<group\> directory.

1. In this new class, implement basic arithmetic operations for addition, subtraction, multiplication, and division. As [static methods](https://www.geeksforgeeks.org/static-method-in-java-with-examples/)

1. Once these metods are in place, it's time to parse user arguments. In the command:
`java -cp <jar-file> <class-path> 10 2 divide`  
The `10`, `2` and `divide` will be available as Strings in the `String[] args` array inside the main class. Use these to select the correct method and print the result.

1. When all things are in place it's time to compile. Use the command `mvn package` to create your java application.

1. And now, finally, we should be able to run the application with the `java -cp` command!

## Conclusion

Great going! You have dipped you toes in working with Maven. If you look at the bottom of your file browser in in VS-Code, you can see that there are a lot more commands that can be used.

![Maven commands](maven.png)

We will get more familiar with these commands day by day.
