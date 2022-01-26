# Measuring Code Execution Time Using Stopwatch

You might have used the `System.out.println(end - start + "ms elapsed")` through `System.currentTimeMillis()` to measure the execution time of a piece of code.

If you have a small number of code points to measure, it can be quite appropriate to do this.

**But when we have a lot of code points to measure, this makes us difficult.**

![](https://c.tenor.com/dTP4cRnO9bEAAAAC/sweating-nervous.gif)

If you want to see the result with a meaningful name and how much of the total time it takes, you have to add cumbersome code to do it. like: 

```java
long start = System.currentTimeMillis();

long initStart = System.currentTimeMillis();
// initialization
long initEnd = System.currentTimeMillis();

long processingStart = System.currentTimeMillis();
// processing
long processingEnd = System.currentTimeMillis();

long end = System.currentTimeMillis();

System.out.println("initialization: " + (initEnd - initStart) + "ms");
System.out.println("processing: " + (processingEnd - processingStart) + "ms");
System.out.println("total: " + (end - start) + "ms");
```

![](https://c.tenor.com/Rv1xH5kdMu8AAAAC/endgame-now.gif)

### It's Time to Use Stopwatch

[Stopwatch](https://github.com/silentsoft/stopwatch) is a library that helps you measure the execution time of a piece of code with a meaningful name and how much of the total time it takes.

We can simply use it like this:

```java
Stopwatch stopwatch = new Stopwatch();

stopwatch.start("initialization");
// ...
stopwatch.stop();

stopwatch.start("processing");
// ...
stopwatch.stop();

stopwatch.start("rendering");
// ...
stopwatch.stop();

stopwatch.print();
```

The `stopwatch.print()` will give you the result like this:

```
|           name |     % |      ms |      s |
|----------------|-------|---------|--------|
| initialization | 59.5% | 1,234ms | 1.234s |
|     processing | 40.0% |   830ms | 0.830s |
|      rendering |  0.5% |    10ms | 0.010s |
|                |       |         |        |
|          total |  100% | 2,074ms | 2.074s |
```

### One More Thing

![](https://c.tenor.com/kPoUqVlwGg0AAAAC/benedict-cumberbatch-endgame.gif)

The Stopwatch can be paused and resumed to remove the time between code points where you do not want to measure. like this:

```java
stopwatch.start("rendering");
// prepare rendering
stopwatch.pause();
// load font stuff
stopwatch.resume();
// render
stopwatch.stop();
```

## Conclusion

Stopwatch can remove chores from your code. If you have a lot of code points to measure, or you want to see the result with a meaningful name and how much of the total time it takes, you can use it.

Thank you for reading this article. If you like Stopwatch, give it a :star2: on [GitHub](https://github.com/silentsoft/stopwatch).

{% github silentsoft/stopwatch %}