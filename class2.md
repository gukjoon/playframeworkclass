# Play Configuration #

# Scala Futures #

```
scala> import scala.concurrent._
import scala.concurrent._

scala> import scala.concurrent.duration._
import scala.concurrent.duration._

scala> import scala.concurrent.ExecutionContext.Implicits.global
import scala.concurrent.ExecutionContext.Implicits.global
```

Explain ExecutionContext

Explain Future data model

```
scala> Future.successful(2) map (a => a + 1)
res0: scala.concurrent.Future[Int] = scala.concurrent.impl.Promise$KeptPromise@27c250e9

scala> Await.result(res0, 2 micros)
res1: Int = 2
```

Explain chaining futures and monadic nature

# Play WS #

# Agents #

Use as idempotent blackboard

# Actors #



