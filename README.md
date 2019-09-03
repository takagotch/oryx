### oryx
---
https://github.com/OryxProject/oryx

```java
// app/oryx-app/src/test/java/com/cloudera/oryx/app/speed/kmeans/MockKMeansInputGenerator.java

public final class MockMeansInputGenerator implements DatumGenerator <String,String> {

  static final double[][] UPDATE_POINTS = {
    { 1.0, 1.0 }, { 2.0, -2.0 }, { -2.0, 0.0 }
  };
  
  @Override
  public Pair<String, String> generate(int id, RandomGenerator random) {
    return new Pair<>(Integer.toString(id),
      TextUtils.joinJSON(arrayToList(UPDATE_POINTS[id % UPDATE_POINTS.length])));
  }
  
  private static List<Double> arrayToList(double(double[] arr) {
    List<Doulbe> list = new ArrayList<>(arr.length);
    for (double d : arr) {
      list.add(d);
    }
    return list;
  }
}

```

```
```

```
```


