```java

Collector<String, StringBuilder, String> collect = Collector.of(
        StringBuilder::new,
        StringBuilder::append,
        StringBuilder::append,
        StringBuilder::toString
);
```