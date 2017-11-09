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


    ---
    ## should be quoted
    
        object GitPitch{
          val IsAwesome=true
        }
    ## end of quote    

* no @title
* indented code block within a indented code block

+++

#### Quoting markdown whith indented code blocks

```markdown
 ---
## should be quoted
     
     object GitPitch{
       val IsAwesome=true
     }
## end of quote
```

* no @title
* indented code block within a fenced code block
* non breaking space prefix on first line

+++

#### Quoting markdown whith indented code blocks

```markdown
---
## should be quoted
    
    object GitPitch{
      val IsAwesome=true
    }
## end of quote    
```

* no @title
* indented code block within a fenced code block

+++

```scala
 prevent breakage propagatation 
```
---

## it has code delimiter slides

+++?code=md_indented.md
* only displays the first 2 backticks
* doesn`t display the closing backticks

+++?code=md_indented.md?lang=markdown
* works fine
+++

log error :
```
2017-11-09 08:54:26,502 Back-End-Pool [warn] c.g.s.WebService - download: failed pp=/github/jeantil/gitpitch-125/126 [ white, null ], from source=https://raw.githubusercontent.com/jeantil/gitpitch-125/126/md_backticked.md?lang=markdown?gp=25, ex={}
java.lang.RuntimeException: java.net.MalformedURLException: QueryString parameter should not have more than 2 = per part
	at play.libs.ws.ahc.AhcWSRequest.setQueryString(AhcWSRequest.java:106)
	at play.libs.ws.ahc.AhcWSRequest.<init>(AhcWSRequest.java:78)
	at play.libs.ws.ahc.AhcWSClient.url(AhcWSClient.java:38)
	at com.gitpitch.services.WebService.download(WebService.java:109)
	at com.gitpitch.services.WebService.fetchBytes(WebService.java:60)
	at com.gitpitch.services.DiskService.download(DiskService.java:155)
	at com.gitpitch.git.GRSService.download(GRSService.java:81)
	at com.gitpitch.services.CodeService.build(CodeService.java:82)
	at com.gitpitch.models.MarkdownModel.process(MarkdownModel.java:183)
	at com.gitpitch.models.MarkdownModel.lambda$new$0(MarkdownModel.java:111)
Caused by: java.net.MalformedURLException: QueryString parameter should not have more than 2 = per part
	at play.libs.ws.ahc.AhcWSRequest.setQueryString(AhcWSRequest.java:106)
	at play.libs.ws.ahc.AhcWSRequest.<init>(AhcWSRequest.java:78)
	at play.libs.ws.ahc.AhcWSClient.url(AhcWSClient.java:38)
	at com.gitpitch.services.WebService.download(WebService.java:109)
	at com.gitpitch.services.WebService.fetchBytes(WebService.java:60)
	at com.gitpitch.services.DiskService.download(DiskService.java:155)
	at com.gitpitch.git.GRSService.download(GRSService.java:81)
	at com.gitpitch.services.CodeService.build(CodeService.java:82)
	at com.gitpitch.models.MarkdownModel.process(MarkdownModel.java:183)
	at com.gitpitch.models.MarkdownModel.lambda$new$0(MarkdownModel.java:111)
```

+++?code=md_backticked.md

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
* non-breaking space prefix on all lines

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
* non-breaking space prefix on first lines

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
