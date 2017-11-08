## Scala Generics code

using github code blocks

```scala
sealed trait Option[+T]
case class Some[T](value:T) extends Option[T]
case object None extends Option[Nothing]
```

---

## Scala Generics code
using std markdown code blocks

    sealed trait Option[+T]
    case class Some[T](value:T) extends Option[T]
    case object None extends Option[Nothing]

---
## Scala Generics code
using pure marked.js + highlight.js [works fine](https://github.com/jeantil/gitpitch-125/blob/127/index.html) (download locally and open in browser to see) 
