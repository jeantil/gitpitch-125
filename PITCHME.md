## gitpich is awesome

---
@title[working title]
## it has working titles

---

@title[working title 2]

## it is GFM compliant

---
@title[it has code higlight]
## it has code higlight

```scala
object GitPitch{
  val IsAwesome=true
}
```

+++

But you can't quote it's own markup in code blocks

```markdown
 ---
 @title[it has code higlight]
 ## it has code higlight
 
 ```scala
 object GitPitch{
   val IsAwesome=true
 }
 ```

```

To make the code display properly I had to :
- put a non breaking space at each start of lines 
- drop the last ` on the closing quoted code block

---

@title[it has broken code higlight]

## it has broken code higlight

```scala
object GitPitch{
  val IsAwesome=true
}
```
+++

```markdown
 ---
 
 @title[it has broken code higlight]
 ## it has broken code higlight
 
 ```scala
 object GitPitch{
   val IsAwesome=true
 }
 ``

```

To make the code display properly I had to :
- put a non breaking space at each start of lines 
- drop the last ` on the closing quoted code block

The difference with working sample is the line break between the slide marker and the @title.

---
@title[it has sublists]
## is has nested lists

* item 1
  * item 2
  * item 3
* item 1
  * item 2
  * item 3
---

@title[it has sublists]
## is has nested lists


* item 1
  * item 2
  * item 3
* item 1
  * item 2
  * item 3
* event when skipping a line before @title

---
@title[can't quote markdown]

```markdown
@title[can't quote markdown]
## it has working titles
```
here is the result of a naive attempt at quoting markdown