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
    <li><a href="#listofmarkup">Lista znaczników w HTML5</a></li>
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

<a id="listofmarkup"></a>
# Lista znaczników HTML5

## Strukturalne (Semantyczne)
- `<html>` — Główny element dokumentu HTML.
- `<head>` — Sekcja zawierająca meta-informacje o dokumencie.
- `<body>` — Główna część dokumentu HTML.
- `<header>` — Nagłówek sekcji lub strony.
- `<footer>` — Stopka sekcji lub strony.
- `<section>` — Sekcja tematyczna dokumentu.
- `<article>` — Niezależna część dokumentu (np. artykuł, wpis na blogu).
- `<nav>` — Nawigacja w dokumencie.
- `<aside>` — Zawartość poboczna (np. pasek boczny).
- `<main>` — Główna treść dokumentu.
- `<div>` — Ogólny kontener dla grupowania elementów.

## Tekstowe
- `<h1>` - `<h6>` — Nagłówki o różnym poziomie ważności (od największego `h1` do najmniejszego `h6`).
- `<p>` — Paragraf tekstu.
- `<span>` — Inline element dla grupowania tekstu.
- `<br>` — Nowa linia (self-closing).
- `<hr>` — Linia horyzontalna (self-closing).

## Formatowanie tekstu
- `<b>` — Tekst pogrubiony (bez nacisku na znaczenie).
- `<strong>` — Tekst pogrubiony (z naciskiem na znaczenie).
- `<i>` — Tekst pochylony (bez nacisku na znaczenie).
- `<em>` — Tekst pochylony (z naciskiem na znaczenie).
- `<u>` — Podkreślenie tekstu.
- `<mark>` — Tekst podświetlony.
- `<small>` — Pomniejszony tekst.
- `<del>` — Tekst przekreślony.
- `<ins>` — Tekst dodany.

## Listy
- `<ul>` — Lista nieuporządkowana.
- `<ol>` — Lista uporządkowana.
- `<li>` — Element listy.
- `<dl>` — Lista definicji.
- `<dt>` — Termin w liście definicji.
- `<dd>` — Definicja terminu.

## Media
- `<img>` — Obraz (self-closing).
- `<video>` — Wideo.
- `<audio>` — Audio.
- `<source>` — Źródło dla mediów (self-closing).
- `<track>` — Napisy dla mediów (self-closing).

## Linki i nawigacja
- `<a>` — Link.
- `<nav>` — Nawigacja.

## Tabele
- `<table>` — Tabela.
- `<thead>` — Nagłówek tabeli.
- `<tbody>` — Ciało tabeli.
- `<tfoot>` — Stopka tabeli.
- `<tr>` — Wiersz tabeli.
- `<th>` — Komórka nagłówkowa tabeli.
- `<td>` — Komórka tabeli.

## Formularze
- `<form>` — Formularz.
- `<input>` — Pole formularza (self-closing).
- `<textarea>` — Obszar tekstowy.
- `<button>` — Przycisk.
- `<select>` — Pole wyboru.
- `<option>` — Opcja w polu wyboru.
- `<label>` — Etykieta dla elementu formularza.
- `<fieldset>` — Grupa pól formularza.
- `<legend>` — Tytuł grupy pól formularza.

## Meta i skrypty
- `<meta>` — Informacje o dokumencie (self-closing).
- `<link>` — Połączenie z zewnętrznym zasobem (self-closing).
- `<style>` — Wbudowane style CSS.
- `<script>` — Skrypty JavaScript.
- `<title>` — Tytuł dokumentu.

## Inne
- `<canvas>` — Obszar do rysowania grafiki.
- `<svg>` — Grafika wektorowa.
- `<iframe>` — Wbudowana ramka.
- `<progress>` — Pasek postępu.
- `<meter>` — Wartość w zakresie.
- `<code>` — Fragment kodu.
- `<pre>` — Sformatowany tekst (zachowanie białych znaków).
- `<blockquote>` — Cytat blokowy.
- `<cite>` — Źródło cytatu.
- `<abbr>` — Skrót.
- `<data>` — Dane z maszynowym znaczeniem.
- `<time>` — Reprezentacja czasu lub daty.


<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>



<a id="wprowadzenie-do-html"></a>
## Wprowadzenie do HTML - znaczniki

<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>

