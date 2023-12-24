
```java

ByteArrayOutputStream csv = new ByteArrayOutputStream();

PrintStream printer = new PrintStream(csv);

printer.println("a;b;c");

printer.println("1;2;3");

printer.close();

csv.close();

```