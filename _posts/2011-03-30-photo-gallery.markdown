---
layout: post
title: Photo Gallery
---

<aside>
  <img src="../../../../images/kapuscinski.gif" alt="[Ryszard Kapuściński]" />
  <p>
  Kiedy się spieszysz, nic nie widzisz, nic nie przeżywasz, 
  niczego nie doświadczasz, nie myślisz! Szybkie tempo wysusza najgłębsze warstwy twojej duszy, 
  stępia twoją wrażliwość, wyjaławia cię i odczłowiecza.
  </p>
  <p class="author">— Ryszard Kapuściński</p>
</aside>

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

* ***Pierwszy*** &ndash; tworzenie listy zdjęć do galerii
{% highlight html %}
	<ul id="albumlist">
		<li><img src="1.jpg" alt="#1" width="240"
			height="160" />Stan równowagi</li>
		<li><img src="2.jpg" alt="#2" width="240"
			height="160" />Ważka</li>
		...	
	</ul>
{% endhighlight %}

* ***Drugi*** &ndash; zdefiniowanie stylu css dla:  body oraz stylu wyświetlania listy o id albumlist (#albumlist, #albumlist li,  #albumlist img)

[Galeria wersja 1.1](http://sigma.inf.ug.edu.pl/~erauchfleisch/galeria/galeria_wer1.1.html)

* ***Trzeci*** &ndash; modyfikacja sposobu wyświetlania galerii, z formy listy na wygląd kompaktowy. W kodzie zmodyfikowano następujące zapisy:
{% highlight css %} #albumlist li { float: left; } {% endhighlight %}
oraz wyłączenie punktowania za pomocą modyfikacji w:
{% highlight css %} #albumlist { list-style-type: none; }{% endhighlight %}
[Galeria wersja 1.2](http://sigma.inf.ug.edu.pl/~erauchfleisch/galeria/galeria_wer1.2.html)


* ***Czwarty*** &ndash; ostateczny kształt galerii &ndash; dodanie odnośników **a** oraz pesudo klasy **:hover**, która jest wykorzystywna, 
gdy kursor najedzie na odnośnik. 
Domyślnie wysokość odnośnika **a** oraz zdjęcia jest ustawiona na 30pt, a po najechaniu kursorem na odnośnik zwiększa się na 200pt. Zaś wysokość całej galerii jest określona na 400pt.
Chcąc dodać kolejne zdjęcie, wysokość tą należy modyfikować o 30pt dla każdego dodanego zdjęcia.
{% highlight css %}
#albumlist li a { display: block; height: 30pt; width: 310pt; float: left; text-decoration: none; 
  			border-bottom: 3pt solid #FFFACD; cursor: pointer; }
#albumlist li a img { width: 310pt; height: 30pt; border: 0; }
#albumlist li a:hover { background: #711515; height: 200pt; }
#albumlist li a:hover img { height: 200pt; } 
{% endhighlight %}
Użyto również id **wrapper**, w celu ustabilizowania położenia galerii na stronie.
{% highlight css %}
#wrapper { margin: 0 auto; width: 310pt; }
{% endhighlight %}

* ***Ostatni szlif*** - zabiegi upiekszające ;)

[Galeria wersja 1.3](http://sigma.inf.ug.edu.pl/~erauchfleisch/galeria/galeria_wer_1.3.html)

