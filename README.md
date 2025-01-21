<a id="readme-top"></a>

<br />
<div algin="center">
  <h3 align="center">Opis-języka-HTML</h3>
</div>

<details>
  <summary>Spis Treści</summary>
  <ol>
    <li><a href="#wprowadzenie-do-html">Wprowadzenie do HTML - znaczniki</a></li>
    <li><a href="#template">Szablon strony html5</a></li>
    <li><a href="#example">Przykład konwersji tekstu z edytora na html</a></li>
    <li><a href="#inlineandline">Elementy blokowe i liniowe w html</a></li>
    <li><a href="#hedings">Nagłówki w html</a></li>
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

<a id="template"></a>
## Szablon strony html5

Skrót tworzący podstawowy szablon strony: !

![obraz](https://github.com/user-attachments/assets/5da7475d-4045-439c-8920-310f0094ff4c)

W żródle storny internetowej można wyróżnić kilka podstawowych elementów:
- Deklarację doctype - to deklaracja dla przeglądarki określająca wersję dokumentu html (Nie jest tagiem)
- Sekcję head - nagłówek dokumentu, czytany wyłącznie przez przeglądarkę. Zawiera tytuł strony, adresy do plików Javascript czy arkuszy stylów oraz znaczniki meta
- Sekcję body - główna treść strony tzw. ciało dokumentu prezentowane użytkownikowi

<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>

<a id="example"></a>
## Przykład konwersji tekstu z edytora na html

```<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tytuł artykułu</title>
</head>
<body>
    <!-- Nagłówek główny -->
    <h1>Tytuł artykułu</h1>

    <!-- Paragraf powitalny -->
    <p>Witaj w naszym artykule! Oto lista rzeczy do zrobienia:</p>

    <!-- Lista numerowana -->
    <ol>
        <li>Sprawdź zadania.</li>
        <li>Dodaj zdjęcia.</li>
        <li>Publikuj artykuł.</li>
    </ol>

    <!-- Cytat blokowy -->
    <blockquote>Cytat: "Inspiracja jest kluczem do sukcesu."</blockquote>

    <!-- Link do strony -->
    <p>Na koniec możesz odwiedzić 
        <a href="http://www.example.com" target="_blank">naszą stronę</a> 
        lub obejrzeć ten obrazek:
    </p>

    <!-- Obrazek -->
    <img src="obrazek.jpg" alt="Przykładowy obrazek">

    <!-- Formatowanie tekstu -->
    <p>
        <u>Podkreślony tekst</u>, 
        <i>pochylony tekst</i> i 
        <strong>tekst pogrubiony</strong>.
    </p>
</body>
</html>
```

<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>

<a id="inlineandline"></a>
# Elementy blokowe i liniowe w HTML

## Elementy blokowe
Elementy blokowe zajmują całą szerokość rodzica i rozpoczynają się od nowej linii.  
Przykłady elementów blokowych:
- `<address>` — adres kontaktowy.
- `<article>` — niezależny fragment treści.
- `<aside>` — zawartość poboczna (np. pasek boczny).
- `<blockquote>` — cytat blokowy.
- `<details>` — rozwijany szczegół.
- `<dialog>` — dialog (okno dialogowe).
- `<div>` — ogólny kontener.
- `<dl>` — lista definicji.
- `<fieldset>` — grupa elementów formularza.
- `<figcaption>` — podpis pod elementem `<figure>`.
- `<figure>` — grupa treści multimedialnych (np. obraz z podpisem).
- `<footer>` — stopka sekcji lub strony.
- `<form>` — formularz.
- `<h1>` - `<h6>` — nagłówki o różnym poziomie.
- `<header>` — nagłówek sekcji lub strony.
- `<hr>` — pozioma linia oddzielająca sekcje (self-closing).
- `<li>` — element listy.
- `<main>` — główna zawartość strony.
- `<nav>` — nawigacja.
- `<ol>` — lista uporządkowana.
- `<p>` — paragraf.
- `<pre>` — tekst preformatowany (zachowuje białe znaki).
- `<section>` — sekcja tematyczna.
- `<table>` — tabela.
- `<tbody>` — ciało tabeli.
- `<td>` — komórka tabeli.
- `<tfoot>` — stopka tabeli.
- `<th>` — komórka nagłówkowa tabeli.
- `<thead>` — nagłówek tabeli.
- `<tr>` — wiersz tabeli.
- `<ul>` — lista nieuporządkowana.

## Elementy liniowe
Elementy liniowe zajmują tylko tyle miejsca, ile wymaga ich treść, i mogą być umieszczane obok siebie w jednym wierszu.  
Przykłady elementów liniowych:
- `<a>` — link.
- `<abbr>` — skrót.
- `<b>` — tekst pogrubiony (bez nacisku na znaczenie).
- `<bdi>` — tekst izolowany pod względem kierunku pisma.
- `<bdo>` — zmiana kierunku tekstu.
- `<br>` — nowa linia (self-closing).
- `<cite>` — tytuł pracy lub cytat.
- `<code>` — fragment kodu.
- `<data>` — dane o maszynowym znaczeniu.
- `<dfn>` — definicja terminu.
- `<em>` — tekst pochylony (z naciskiem na znaczenie).
- `<i>` — pochylony tekst (bez nacisku na znaczenie).
- `<img>` — obraz (self-closing).
- `<input>` — pole formularza (self-closing).
- `<kbd>` — tekst reprezentujący wejście z klawiatury.
- `<label>` — etykieta formularza.
- `<mark>` — podświetlony tekst.
- `<q>` — cytat inline.
- `<s>` — tekst przekreślony (oznacza nieaktualne informacje).
- `<samp>` — przykład wyjścia programu.
- `<small>` — pomniejszony tekst.
- `<span>` — ogólny inline kontener.
- `<strong>` — tekst pogrubiony (z naciskiem na znaczenie).
- `<sub>` — indeks dolny.
- `<sup>` — indeks górny.
- `<time>` — data lub czas.
- `<u>` — podkreślony tekst.
- `<var>` — zmienna matematyczna lub w kodzie.
- `<wbr>` — sugerowane miejsce podziału linii (self-closing).

---

## Podział funkcjonalny
- **Elementy blokowe** są używane do tworzenia struktury i układu strony.
- **Elementy liniowe** służą do formatowania tekstu i innych treści wewnątrz elementów blokowych.



<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>

<a id="hedings"></a>
#Nagłówki w html

```
<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Przykład nagłówków HTML</title>
</head>
<body>
    <h1>To jest nagłówek H1 (najwyższego poziomu)</h1>
    <h2>To jest nagłówek H2</h2>
    <h3>To jest nagłówek H3</h3>
    <h4>To jest nagłówek H4</h4>
    <h5>To jest nagłówek H5</h5>
    <h6>To jest nagłówek H6 (najniższego poziomu)</h6>
</body>
</html>
```

<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>


<a id="listofmarkup"></a>

# Lista znaczników HTML5

1. **Strukturalne (Semantyczne)**

    `<html>`, `<head>`, `<body>`, `<header>`, `<footer>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<nav>`, `<div>`, `<search>`

2. **Metadane dokumentu**

    `<base>`, `<meta>`, `<link>`, `<style>`, `<title>`

3. **Sekcjonowanie treści**

    `<address>`, `<h1>` - `<h6>`, `<hgroup>`, `<header>`, `<footer>`, `<article>`, `<section>`, `<nav>`, `<aside>`, `<main>`

4. **Tekstowe**

    `<p>`, `<br>`, `<hr>`, `<blockquote>`, `<q>`, `<pre>`, `<code>`, `<abbr>`, `<cite>`, `<small>`, `<strong>`, `<em>`, `<mark>`, `<b>`, `<i>`, `<u>`, `<s>`, `<kbd>`, `<samp>`, `<var>`, `<sub>`, `<sup>`, `<time>`

5. **Listy**

    `<ul>`, `<ol>`, `<li>`, `<dl>`, `<dt>`, `<dd>`, `<menu>`

6. **Multimedia**

    `<img>`, `<audio>`, `<video>`, `<source>`, `<track>`, `<map>`, `<area>`, `<picture>`

7. **Osadzone treści**

    `<iframe>`, `<embed>`, `<object>`, `<param>`

8. **Elementy formularzy**

    `<form>`, `<input>`, `<textarea>`, `<button>`, `<select>`, `<option>`, `<optgroup>`, `<fieldset>`, `<legend>`, `<datalist>`, `<output>`, `<progress>`, `<meter>`, `<label>`

9. **Tabela**

    `<table>`, `<thead>`, `<tfoot>`, `<tbody>`, `<tr>`, `<th>`, `<td>`, `<caption>`, `<col>`, `<colgroup>`

10. **Interaktywne elementy**

    `<details>`, `<summary>`, `<dialog>`

11. **Komponenty Webowe**

    `<template>`, `<slot>`

12. **SVG i MathML**

    `<svg>`, `<math>`

13. **Skrypty**

    `<script>`, `<noscript>`, `<canvas>`

14. **Przestarzałe elementy (Nie zaleca się używania)**

    `<big>`, `<center>`, `<font>`, `<marquee>`, `<tt>`, `<strike>`, `<acronym>`, `<xmp>`


# Lista znaczników HTML5 z opisem

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
- `<details>` — Rozwijany szczegół.
- `<summary>` — Podsumowanie dla elementu `<details>`.
- `<dialog>` — Dialog (okno dialogowe).

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
- `<sub>` — Indeks dolny.
- `<sup>` — Indeks górny.
- `<bdi>` — Izolacja kierunku tekstu.
- `<bdo>` — Nadpisanie kierunku tekstu.
- `<s>` — Przekreślony tekst (oznacza nieaktualne informacje).
- `<q>` — Cytat inline.
- `<samp>` — Przykład wyjścia programu.
- `<var>` — Zmienna w kodzie lub matematyce.
- `<kbd>` — Wprowadzanie z klawiatury.

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
- `<picture>` — Kontener dla obrazów o różnych rozmiarach.
- `<map>` — Mapowanie obrazów.
- `<area>` — Aktywny obszar w mapie obrazów (self-closing).

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
- `<caption>` — Tytuł tabeli.
- `<colgroup>` — Grupa kolumn.
- `<col>` — Kolumna w tabeli.

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
- `<datalist>` — Lista predefiniowanych wartości dla `<input>`.
- `<output>` — Wynik operacji.
- `<optgroup>` — Grupa opcji w `<select>`.

## Meta i skrypty
- `<meta>` — Informacje o dokumencie (self-closing).
- `<link>` — Połączenie z zewnętrznym zasobem (self-closing).
- `<style>` — Wbudowane style CSS.
- `<script>` — Skrypty JavaScript.
- `<title>` — Tytuł dokumentu.
- `<noscript>` — Treść wyświetlana, gdy skrypty są wyłączone.

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
- `<template>` — Szablon treści.
- `<slot>` — Miejsce na treść w komponencie.
- `<wbr>` — Opcjonalne miejsce podziału linii (self-closing).



<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>



<a id="wprowadzenie-do-html"></a>
## Wprowadzenie do HTML - znaczniki

<p align="right">(<a href="#readme-top">Wróć na góre</a>)</p>

