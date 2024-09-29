Jeżeli chcemy przechować jakąś informację w programie do późniejszego wykorzystania, to najpierw musimy stworzyć zmienną.
Zmienne możemy stworzyć na 2 sposoby (jest jeszcze 3, ale na razie nie chcę o nim mówić).

Sposób 1, który używaliśmy na naszych zajęciach

```js
const nameOfTheVariable = "jakaś wartość jak np.: ten tekst";
```

Sposób 2 uzupełnie na następnych zajęciach

---

Sposób 3 przedstawię pod koniec nauki by Ci nie mieszać. Nie powinno się go używać w nowoczesnym programowaniu jak co

---

W programie mamy różne typy danych. Mamy tekst, który musi być zapisywany pomiędzy jakimkolwiek z tych 3 symboli ' " \`. Poza tekstem mamy też wartości logiczne, jak true lub false. Używamy ich w przypadku sytuacji binarnych, jak chociażby do określenia czy jest włączony włącznik światła. Może być włączony (`true`), albo wyłączony (`false`). Posiadamy również obiekty, które podczas naszej lekcji nazywaliśmy grupą/obiektem. Służą one do zgrupowania danych w schemacie klucz: wartość. Dla przykładu stworzyliśmy obiekt `person`, opisujący Ciebie. Były w nim chociażby takie klucze/pola/właściwości jak name, czy favSongs. Wartościa odpowiednia dla name, była wartość "Julia", która była tekstem, a dla favSongs była to lista ulubionych piosek zapisanych jako tekst. Każda piosenka była reprezentowana jako osobny tekst w tablicy/liście. Jedną z nich była TTFU (reszty nie pamiętam xD).

W tablicy/liście mogą znajdować się obiekty/grupy i vice versa. Możemy nieskończenie zagnieżdżać listy/tablice w obiekty/grupy lub obiekty/grupy w listy/tablice. Tego też wymaga od Ciebie aktualne zadanie domowe, byś to przetestowała sobie i się z tym oswoiła.

Żeby odnieść się do konkretnego elementu z listy musimy użyć składni jak w przykładzie poniżej:

```js
somethingWhichIsAnArray[index];
```

Należy pamiętać, że w programowaniu liczymy od zera. Zerowy element tablicy, naszą pierwszą daną tam zawartą.

Jeżeli chcemy odnieść się do konkretnego klucza/pola/właściwości w obiekcie/grupe należy użyć kropki. Dla przykładu jeżeli chcemy odnieść się do `favSongs` dla konkretnego człowieka, w sytuacji czy `favSongs`, są zdefiniowane w obiekcie `person`, to musimy zapisać to w następujący sposób.

```js
person.favSongs;
```

W programowaniu, możemy schować naszą logikę w funkcji. Funkcje powinny być reużywalne, żeby zachować czystość kodu i stosować się do dobry praktych. Na naszych zajęciach użyliśmy funkcji `console.log`, która wyświetla dane do konsoli. W momencie, gdy chcieliśmy jej użyć musieliśmy ją wywołać używając nawiasów kółkowatych.

```js
console.log(someData);
```

Ta zasada jest uniwersalna dla każdej\* funkcji w języku. Dla przykładu jak stworzyliśmy funkcję do dodawania, lub odejmowania, to wywoływaliśmy ją w ten sam sposób. Pomiędzy kółkowate nawiasy podczas wywoływania funkcji wrzucamy argumenty, czyli dane, które chcemy do niej przekazać. Na podstawie tych funkcja dostosuje swoje działanie.

Aby stworzyć funkcję należy stworzyć zmienną, która po operatorze przypisania `=`, będzie miała następujące znaki `() => {}`. W nawiasach kółkowatych definiujemy argumenty, czyli dane, których będziemy oczekiwać by na nich operować w ramach danej funkcji. Argumenty zapisujemy po przecinku. Nazwa argumentu może być w pełni abstrakcyjna. Będzie ona reprezentować daną, która zostanie przekazana "z góry". Dla funkcji do dodawania, było to następująco `firstNumber`, oraz `secondNumber`, ponieważ to właśnie tego potrzebuje, by dokonać jakichkolwiek operacji matematycznych. Nimożliwe byłoby dodawanie wartości, jak nie mamy nic co chcielibyśmy ze sobą dodać. Pomiędzy ostrymi nawiasami definujemy logikę funkcji, czyli to co ma się dziać podczas jej działania.

W programowaniu posiadamy operatory matematyczne do dodawania, odejmowania, mnożenia, dzielenia, modulo, itd. Cała listą włącznie z tymi, których nie omawaliśmy jest dostępna tutaj: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_operators#assignment_operators

Poza nimi są operatory do sprawdzania danych wartości. Np. czy dana wartość jest identyczna `==`, czy jest mniejsza bądź równa `<=`, większa bądź równa `>=`, itd. Musimy pamiętać, że o ile operator do porównywania ma sens prawie zawsze, czyli `==`, o tyle np. nie możemy sprawdzić czy tekst jest większy bądź równy, bo co to tak właściwie znaczy. Potencjalnie moglibyśmy sprawdzić czy długość tekstu jest większa bądź równa od czegoś. `"jakiś tekst".length >= 100`

Jeżeli jakiś warunek zostanie spełniony, jak chociażby `"jakiś tekst".length >= 100`, to możemy stwierdzić co ma się stać w pozytywnym przypadku, a co w negatywnych. Taką logikę zapisujemy w następujący sposób: `somethingToCheckIfItsTrue ? valueIfItsTrue : valueIfItsFalse`
