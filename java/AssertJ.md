```java

   assertThatExceptionOfType(RuntimeException.class)
        .isThrownBy(() ->   billingStructureService.getBillingStructuresByAccount(account))
		.withMessage("");
```



```java
assertThat(author.getBook()).isNotNull().satisfies(it -> {
    assertThat(it.getId()).isEqualTo(10);
});
```


```java

assertThat(user)
                .isNotNull()
                .satisfies(u -> {
                    assertThat(u.getId()).isEqualTo(1L);
                    assertThat(u.getName()).isEqualTo("Wim");
                });
```


```java 
@Test
void givenTestMethodWithTempDirectory_whenWriteToFile_thenContentIsCorrect(@TempDir Path tempDir) 
  throws IOException {
    Path numbers = tempDir.resolve("numbers.txt");

    List<String> lines = Arrays.asList("1", "2", "3");
    Files.write(numbers, lines);

    assertAll(
      () -> assertTrue("File should exist", Files.exists(numbers)),
      () -> assertLinesMatch(lines, Files.readAllLines(numbers)));
}
```