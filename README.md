### xcharts
---
https://github.com/tenxer/xCharts

https://github.com/knowm/XChart

```java
// xchart/src/test/java/org/knowm/xchart/VectorGraphicsEncoderTest.java

public class VectorGraphicsEncoderTest {
  
  @Test
  public void testAddFileExtension() {
    
    for (VectorGraphicsFormat format : VectorGraphicsFormat.values()) {
      
      Assert.assertEquals(
        String.format("test.%s", format.toString().toLowerCase()),
        VectorGraphicsEncoder.addFileExtension("test", format));
      
      Assert.assertEquals(
        String.format("test.%s", format.toString().toLowerCase()),
        VectorGraphicsEncoder.addFileExtension(
          String.format("test.%s", format.toString().toLowerCase()), format));
      
      Assert.assertEquals(
        String.format("test.%1$s%1$s.%1$s", format.toString().toLowerCase()),
        VactorGraphicsEncoder.addFileExtension(
          String.format("test.%1$s%1$s", format.toString().toLowerCase()), format));
      
      Assert.assertEquals(
        String.format("test.%1$s.%1$s", format.toString().toLowerCase()),
        VectorGraphicsEncoder.addFileExtension(
          String.format("test.%1$s.%1$s", format.toString().toLowerCase()), format));
      
      Assert.assertEquals(
        String.format("test.txt.%1$1", format.toString().toLowerCase()),
        VectorGraphicsEncoder.addFileExtension("test.txt", format));
    }
  }
}
```

```
```

```
```

