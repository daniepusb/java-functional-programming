# java-functional-programming
Practice functional programming paradigm’s core principles with Java programming language.


# Documentation

For review the documentation you can use:
```bash
https://www.baeldung.com/java-functional-programming
```


# Example:
In this example, a Stream is used to process a list of names. The lambda expression name -> name.startsWith("A") is passed to the filter method, which selects only elements that meet the criterion of starting with "A". The result is collected into a new list (namesStartingWithA). This approach reflects the functional nature by treating operations as transformations rather than direct state changes.

```bash
import java.util.Arrays;
import java.util.List;

public class FunctionalProgrammingExample {

    public static void main(String[] args) {
        List<String> names = Arrays.asList("Alice", "Bob", "Charlie", "David", "Eve");

        // Using lambda expressions and the filter method to get names starting with "A"
        List<String> namesStartingWithA = names.stream()
                .filter(name -> name.startsWith("A"))
                .collect(java.util.stream.Collectors.toList());

        System.out.println("Names starting with 'A': " + namesStartingWithA);
    }
}

```

Functional programming is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids state change and mutable variables. Instead of modifying state, it focuses on applying pure functions that produce results based solely on their inputs, without side effects.

Java introduced functional programming features with the release of Java 8 in March 2014. One of the most significant additions was the introduction of lambda expressions and the java.util.function package, which provides pre-defined functional interfaces.
