---
layout: post
title: "Dockerfile Commands"
author: "Andre Santos Barros da Silva"
---

Selecionar distintos que terminam e começam com vogais:

{% highlight MySQL %}
SELECT DISTINCT CITY FROM STATION WHERE city regexp '[aeiou]$' or city regexp '[^aeiou]'
{% endhighlight %}

Selecionar distintos que nao terminam e começam com vogais:

{% highlight MySQL %}
SELECT DISTINCT CITY FROM STATION WHERE city regexp '[^aeiou]$' or city regexp '^[^aeiou]'
{% endhighlight %}
