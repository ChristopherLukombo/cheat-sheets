```java


Foo<Bar> mockFoo = (Foo<Bar>) mock(Foo.class);
when(mockFoo.getValue()).thenReturn(new Bar());
```