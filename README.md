# kotlin-multi-target-offline-fallback
POC of business logic written in Kotlin called on JVM as normal usage and falling back to koltinscript when offline

# Why

- Javascript in not easily maintainable
- We may want to transition from existing codebase stuck in JDK 7
- Calculator : We need to combine business rules
- most of the developers know java

# Todo

- this POC
- unit test
- maybe test on both platforms
- write pros/cons
- build to target JVM and Javascript
- fallback mechanism
- sync back mechanism (when server business logic remains the same)

# Pros/Cons

## pros

- business easier to test coming from java
- can use java test tooling
- can convert java business logic automatically in kotlin
- can use lambdas and java 8ish feature on JVM7 target
- business logic can still be used in 
- ops know how to JAR (they don't have to learn and monitor nodejs yet)
- design patterns using functional style : appropriate for the calculator
- can allow to delay choices

## cons

- another language?
- maybe need gradle to compile multiple targets

## Resources

- [KotlinConf 2017 - Sharing [Kotlin code across platforms] is Caring! by Eugenio Marletti](https://www.youtube.com/watch?v=DctKvZOU56I)
