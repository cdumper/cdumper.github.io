---
layout: default
title: Groovy Intro
category: Learning
comments: true
---

{% highlight ruby %}
First peek at groovy
{% endhighlight %}

##Groovy

### Syntax
__Strings__:

- single quoted string

>single line plain string

- double quoted string 

>support string interpolation

- triple quoted string

>multiple line plain string

```groovy
def number = 1
def eagerGString = "value == ${number}"
def lazyGString = "value == ${ -> number}"

assert eagerGString == "value == 1"
assert lazyGString == "value == 1"

number = 2

assert eagerGString == "value == 1"
assert lazyGString == "value == 2"
```
