---
layout: post
title: PHOTO GALLERY
---

<blockquote>
<img src="../../../../images/kapuscinski.gif" alt="[Ryszard Kapuściński]" />
<p>
Kiedy się spieszysz, nic nie widzisz, nic nie przeżywasz, 
niczego nie doświadczasz, nie myślisz! Szybkie tempo wysusza najgłębsze warstwy twojej duszy, 
stępia twoją wrażliwość, wyjaławia cię i odczłowiecza.
</p>
<p class="author"> — Ryszard Kapuściński</p>
</blockquote>

# {{ page.title }}


## **SARDYNIA** 
![ godło Sardynii ](../../../../images/godlo.gif)

	
[Sardynia](http://pl.wikipedia.org/wiki/Sardynia)
jest bardzo malowniczą, pełną uroku wyspą na Morzu Śródziemnym. 
Przeważającą część wyspy zajmują góry i płaskowyże.
Wzdłuż wybrzeża znajduje się wiele dużych, płytkich, słonowodnych lagun i rozlewisk. 


Architekturę miasta tworzą nie wysokie kamieniczki. 
A kamienne, wąskie uliczki pełne sklepików prowadzą do małych placy, tworząc to miejsce bardzo malowniczym.

Za pomocą obiektywu postarałam się uchwycić ten niepowtarzalny, pełen uroku klimat.



## **Historia tworzenia galerii**

Pierwszym krokiem do utworzenia galerii był wybór zdjęć z podróży. 
Następnie mogłam przystąpić do pracy i utworzyć album zdjęć.
Poniżej opisałam historię jak on powstawał.


**Kroki:**

* ***Pierwszy*** - tworzenie listy zdjęć do galerii
{% highlight html %}
	<ul id="albumlist">
		<li><img src="1.jpg" alt="#1" width="240"
			height="160" />Stan równowagi</li>
		<li><img src="2.jpg" alt="#2" width="240"
			height="160" />Ważka</li>
		...	
	</ul>
{% endhighlight %}

* ***Drugi*** - zdefiniowanie stylu css dla:  body,  #albumlist,  #albumlist li,  #albumlist img

[Galeria wersja 1.1](http://sigma.inf.ug.edu.pl/~erauchfleisch/galeria/galeria_wer1.1.html)

* ***Trzeci*** - modyfikacja sposobu wyświetlania galerii, z formy listy na wygląd kompaktowy. W kodzie zmodyfikowano następujące zapisy:
{% highlight css %} #albumlist li { float: left; } {% endhighlight %}
oraz wyłączenie punktowania za pomocą modyfikacji w:
{% highlight css %} #albumlist { list-style-type: none; }{% endhighlight %}
[Galeria wersja 1.2](http://sigma.inf.ug.edu.pl/~erauchfleisch/galeria/galeria_wer1.2.html)


* ***Czwarty*** - 


* ***Ostatni szlif*** - zabiegi upiekszające ;)

[Galeria wersja 1.3](http://sigma.inf.ug.edu.pl/~erauchfleisch/galeria/galeria_wer_1.3.html)

