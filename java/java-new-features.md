# Java new features from JDK 8 to 21

* https://advancedweb.hu/a-categorized-list-of-all-java-and-jvm-features-since-jdk-8-to-21/


## Key New Features

### Virtual Threads
* https://developers.redhat.com/articles/2023/09/21/whats-new-developers-jdk-21#
* Why Use Virtual Threads?
  * Use virtual threads in high-throughput concurrent applications, especially those that consist of a great number of concurrent tasks that spend much of their time waiting. Server applications are examples of high-throughput applications because they typically handle many client requests that perform blocking I/O operations such as fetching resources.

  * Virtual threads are not faster threads; they do not run code any faster than platform threads. They exist to provide scale (higher throughput), not speed (lower latency).

### Record Classes

The following Rectangle declaration can be concisely declared with Record class

``` 
public final class Rectangle {
    private final double length;
    private final double width;

    public Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
    }

    double length() { return this.length; }
    double width()  { return this.width; }

    // Implementation of equals() and hashCode(), which specify
    // that two record objects are equal if they
    // are of the same type and contain equal field values.
    public boolean equals...
    public int hashCode...

    // An implementation of toString() that returns a string
    // representation of all the record class's fields,
    // including their names.
    public String toString() {...}
}
```

Record class:
```
record Rectangle(double length, double width) { }
```

### Pattern Matching
```    void testPrint(Object o) {
        String formatted = switch (o) {
            case Integer i when i > 10 -> String.format("a large Integer %d\n", i);
            case Integer i             -> String.format("a small Integer %d\n", i);
            case Long l                -> String.format("a Long %d\n", l);
            default                    -> o.toString();
        };

        System.out.print(formatted);
    }

    void testTypePatternMatching() {
        testPrint(Integer.valueOf(1));
        testPrint(Integer.valueOf(100));
        testPrint(Long.valueOf(10));
    }
```


### Sequenced Collections

### Local Variable Type Inference