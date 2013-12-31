# Setup Play Framework #
```
wget http://downloads.typesafe.com/play/2.2.1/play-2.2.1.zip
unzip play-2.2.1.zip
```

```
export PATH=/Applications/play-2.2.1:$PATH
```

```
play new woo
```

# REPL Basics #
```
play console-quick
```

```
scala> 1+1
res0: Int = 2

scala> res0 + 1
res1: Int = 3

scala> def example(test: Int): Int = {
     | test + 1
     | }
example: (test: Int)Int

scala> def example
     | 
     | 
You typed two blank lines.  Starting a new command.
```

# Collections #

## map ##
```
scala> val firstList = List(1,2,3)
firstList: List[Int] = List(1, 2, 3)
```

Explain val, var, maybe lazy

```
scala> firstList map (a => a + 1)
res1: List[Int] = List(2, 3, 4)
```

Explain first class functions and syntax variations
Explain map

## find ##

```
scala> firstList find (a => a == 1)
res2: Option[Int] = Some(1)
```

Explain find
Explain Option[T]

## flatMap ##

```
scala> firstList flatMap (a => if((a % 2) == 0) Some(a) else None)
res3: List[Int] = List(2)
```

Explain flatMap

```
scala> for(a <- firstList if (a % 2) == 0) yield a
res4: List[Int] = List(2)
```

Explain monads and for comprehensions

# Objects and case classes #

```
scala> object D
defined module D

scala> case class A(t: Int)
defined class A

scala> case object B
defined module B
```

Explain object
Explain case class
Explain case object

## Pattern matching ##






# Play Framework #

## Application Structure ##
app - 
conf - 
project - 
public - 
test - 

## Running ##
```
play compile
play run
play start
```

## Writing your first controller ##

