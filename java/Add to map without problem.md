Add to map without problem

```java

.collect(HashMap::new, (m, v) -> m.put(v.getDeviceEUI(), v.getDevicePicto()), HashMap::putAll);
```