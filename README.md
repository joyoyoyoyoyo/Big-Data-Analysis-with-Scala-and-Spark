# Big Data Analysis with Scala and Spark
[![Build Status](https://travis-ci.com/joyoyoyoyoyo/Big-Data-Analysis-with-Scala-and-Spark.svg?branch=master)](https://travis-ci.com/joyoyoyoyoyo/Big-Data-Analysis-with-Scala-and-Spark)

## Wikipedia
1. Start a SparkContext (Setup SparkConfigs)
2. Read in Wikipedia Data
3. Compute a ranking of programming languages

How a ranked language might look like:
```
List(("Scala", 999999), ("JavaScript", 1278), ("LOLCODE", 982), ("Java", 42))
```


## StackOverflow 
K-Means clustering algorithm on StackOverflow postings by programming language tag

List of Languages:
```
  /** Languages */
  val langs =
    List(
      "JavaScript", "Java", "PHP", "Python", "C#", "C++", "Ruby", "CSS",
      "Objective-C", "Perl", "Scala", "Haskell", "MATLAB", "Clojure", "Groovy")

```

Computed score examples:
```
((1, 6,   None, None, 140, Some(CSS)),  67)
((1, 42,  None, None, 155, Some(PHP)),  89)
((1, 72,  None, None, 16,  Some(Ruby)), 3)
((1, 126, None, None, 33,  Some(Java)), 30)
((1, 174, None, None, 38,  Some(C#)),   20)
```

Resulting cluster details:
```
Resulting clusters:
  Score  Dominant language (%percent)  Questions
================================================
      1  C#                (0.0  %)       177651
      1  JavaScript        (0.0  %)       179411
      1  Objective-C       (0.0  %)        46511
      1  PHP               (0.0  %)       155061
      1  Groovy            (0.1  %)         1027
      2  Java              (0.0  %)       188364
      2  Perl              (0.0  %)         9375
      2  MATLAB            (0.0  %)         5010
      2  CSS               (0.0  %)        55438
      2  Python            (0.0  %)        85743
      2  Ruby              (0.0  %)        26590
      2  C++               (0.0  %)        88841
      4  Scala             (0.0  %)         6040
      4  MATLAB            (0.0  %)         2081
      4  Clojure           (0.1  %)         1320
      8  Haskell           (0.0  %)         4692
      8  Groovy            (0.2  %)          438
      9  Perl              (0.0  %)         2283
     16  Clojure           (0.2  %)          634
     21  Groovy            (2.2  %)           45
     41  MATLAB            (2.7  %)           37
     44  Haskell           (0.3  %)          386
     52  Scala             (0.3  %)          346
     55  Clojure           (2.4  %)           41
     98  Objective-C       (0.2  %)          401
    108  C++               (0.3  %)          341
    117  Scala             (3.0  %)           33
    124  PHP               (0.1  %)          794
    124  Perl              (1.9  %)           54
    144  Ruby              (0.3  %)          356
    160  C#                (0.1  %)         1260
    180  Java              (0.3  %)          395
    182  Haskell           (14.3 %)            7
    282  CSS               (0.4  %)          226
    300  JavaScript        (0.4  %)          279
    301  Python            (0.3  %)          334
    431  PHP               (2.6  %)           39
    586  C++               (5.3  %)           19
    657  Ruby              (2.8  %)           36
    925  C#                (1.5  %)           66
    983  CSS               (3.6  %)           28
   1097  Objective-C       (3.3  %)           30
   1432  JavaScript        (3.7  %)           27
   1445  Python            (2.9  %)           34
   3092  Java              (12.5 %)            8
```
