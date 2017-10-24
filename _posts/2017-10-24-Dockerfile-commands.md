---
layout: post
title: "Dockerfile Commands"
author: "Andre Santos Barros da Silva"
---

Dockerfile, aquele jogo da baleia azul para TI.

Vamos lá.

{% highlight markdown %}
FROM debian:wheezy
MAINTAINER andre da silva <andre.silva@axiros.com>

RUN apt-get update

RUN apt-get install -y python-pip
RUN apt-get clean

{% endhighlight %}

Agora hora de fazer este belo comando rodar:

$sudo docker build -t container/django1.0

Veja em pronto:

$sudo docker images

pronto, seu container está pronto, hora de usar:

$sudo docker run -it container/django1.0 /bin/bash

no container rode, para visializar os processos: $ps -ef

ctrl+p+q, para sair do container e use um: $curl <IP container> para acessar algo que ele retorna
