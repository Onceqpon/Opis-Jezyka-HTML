<a id="readme-top"></a>

<br />
<div algin="center">
  <h3 align="center">Opis-języka-HTML</h3>
</div>

<details>
  <summary>Spis Treści</summary>
  <ol>
    <li><a href="#wprowadzenie-do-html">Wprowadzenie do HTML - znaczniki</a></li>
    <li><a href="#roadmap">Szablon strony html5</a></li>
    <li><a href="#contributing">Przykład konwersji tekstu z edytora na html</a></li>
    <li><a href="#license">Elementy blokowe i liniowe w html</a></li>
    <li><a href="#contact">Nagłówki w html</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<a id="wprowadzenie-do-html"></a>
## Wprowadzenie do HTML - znaczniki
Edytor Kodu: Visual Code
Przydatne Rozszerzenie: Live Server

HTML - HyperText Markup Language 
<br>
HTML nie jest językiem programowania np. ```<p>```, jest językiem znaczników który opisuje co ma być wyświetlane w przeglądarce

Skrót tworzący podstawowy szablon strony: !

![obraz](https://github.com/user-attachments/assets/5da7475d-4045-439c-8920-310f0094ff4c)


#Części składowe znaczników

![obraz](https://github.com/user-attachments/assets/f68ca555-f9db-4fb9-85ff-bd36997ee194)

Każdy tag posiada swoją nazwę oraz ostre nawiasy, a co jest pomiędzy tagiem otwierającym, a zamykającym staje się treścią konkretnego elementu, tutaj paragrafu. Dodatkowo tag zamykający musi mieć slash przed nazwą przez co określa, że w tym miejscu koczy się dany element.

Znaczniki(tagi) dają informację przeglądarce na temat:
- Znaczenie tekstu:
  * ```<h1>Tytyuł artykułu</h1>``` tag h1 wskazuje że treść w nim zawarta jest nagłówkiem np artykułu
  * ```<p>paragraf</p>``` tag p to paragrafy tekstu

- Formatowanie tekstu:
  * ```<u>podkreślony tekst</u>``` tag u podkreśla tekst
  * ```<i>pochylony tekst</i>``` tag i tworzy pochylony tekst

- Dodatkowe informacje do wyświetlenia lub akcję do wykonania:
  * ```<img src="obrazek.jpg">``` tag img pokazuje obrazek
  * ```<a href="www.google.pl">ling do strony google</a>```
 
![obraz](https://github.com/user-attachments/assets/6508f242-f457-41d3-8501-a6f48687fabe)


Zagnieżdżanie znaczników:
- Prawidłowe( znacznik u rozpoczął się i zakończył wewnątrz p):
  *```<p>Lorem ipsum dolor sit,<u>consectetur</u> adipiscing.</p>```
  
- Błędne(ponieważ tag u będący wewnątrz paragrafu powinien się w nim zakończyć):
  *```<p>Lorem ipsum dolor sit,<u>consectetur adipiscing.</p></u>```

Pojedyńcze znaczniki tzw. "closing tags": (są to tagi bez znacznika zamykającego, nie jest wymagany dla nich użycie slasha "/") przykład:
* ```<hr>``` - horyzontalna linia na całą szerokość
* ```<br>``` - nowa linia
* ```<img src="obrazek.jpg">``` - wyświetla zdjęcie na stronie
* ```<input type="text">``` - kontrolka folmularza
* Dodatkowo również: ```<link> i <meta>```
    



<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>

<a id="wprowadzenie-do-html"></a>
## Wprowadzenie do HTML - znaczniki

<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>
