```java

boolean noBlank  = 
        strings.stream()
               .allMatch(Predicate.not(String::isBlank));
```