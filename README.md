### jsonassert
---
http://jsonassert.skyscreamer.org/

```java
// src/test/java/org/skycreamer/jsonassert/DependencyTest.java

public class DependencyTest {
  @Test
  public void nop() {
    //
  }
  
  public void testJSonGetLong() throws Exception {
    Long target = -xxxxL;
    String targetString = target.toString();
    
    JSONObject value = new JSONObject().put("id", target);
    Assert.assertEquals(target, (Long) value.getLong("id"));
    
    value = new JSONObject().put("id", targetString);
    Assert.assertEquals(target, (Long) Long.parseLong(value.getString("id")));
    Assert.assertEquals(target, (Long) value.getLong("id"));
  }
}
```

```
```

```
```


