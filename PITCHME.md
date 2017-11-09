## gitpich is awesome
--- 
@title[it renders simple markdow]
## it renders markdown

foo is bar

baz is oof

* item list
* item list

+++ 
#### The markdown for the above slide
```markdown
@title[it renders simple markdow]
## it renders markdown

foo is bar

baz is oof

* item list
* item list
```
* using backtick fences
+++
#### The markdown for the above slide no @title
```markdown
## it renders markdown

foo is bar

baz is oof

* item list
* item list
```
* using backtick fences

+++

#### The markdown for the above slide

    @title[it renders simple markdow]
    ## it renders markdown

    foo is bar

    baz is oof

    * item list
    * item list

* using indented code block (4 spaces) fences

+++

#### The markdown for the above slide no @title
  
    ## it renders markdown

    foo is bar

    baz is oof

    * item list
    * item list

* using indented code block (4 spaces) fences

---

## it has indented code blocks


    object GitPitch{
      val IsAwesome=true
    }

+++

#### Quoting markdown whith indented code blocks

```markdown
---
## it has code higlight
    
    object GitPitch{
      val IsAwesome=true
    }
```

* no @title
* indented code block within a fenced code block

+++

#### Quoting markdown whith indented code blocks


    ---
    ## it has code higlight
    
        object GitPitch{
          val IsAwesome=true
        }

* no @title
* indented code block within a indented code block

---

## it has backtick fenced code blocks

```scala
object GitPitch{
  val IsAwesome=true
}
```

+++

#### Quoting markdown whith fenced code blocks


    ---
    ## it has code higlight
    
    ```scala
    object GitPitch{
      val IsAwesome=true
    }
    ```

* no @title
* indented code block

#### Quoting markdown whith fenced code blocks

```markdown
 ---
 ## it has code higlight
  
 ```scala
 object GitPitch{
   val IsAwesome=true
 }
 ```
```
* no @title
* nested backtick fenced block
* non-breaking space prefix
+++

#### Quoting markdown whith fenced code blocks

```markdown
---
## it has code higlight
 
```scala
object GitPitch{
  val IsAwesome=true
}
```
```
* no @title
* nested backtick fenced block

+++