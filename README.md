# Langton-s-Ant

<h1>Mrówka Langtona</h1>
<h3>#Problem badawczy</h3>
Mrówka Langtona, to automat komórkowy, który został zaprojektowany przez Chrisa Langtona. Zasady działania "mrówki":<br>
1. Początkowo plansza jest niezamalowana.<br>
2. Mrówka startuje z pola niezamalowanego i skręca w lewo zamalowując pole z którego startuje.<br>
3. Mrówka, która wchodzi na niezamalowane pole zmienia je na zamalowane i skręca w lewo.<br>
4. W przypadku, gdy mrówka wchodzi na pole zamalowane zmienia je na niezamalowane i skręca w prawo.<br>
5. Gdy mrówka dotrze do końca planszy, to kończy swój ruch.<br>

Ruch mrówki jest ciężki do przewidzenia, dlatego program pomoże nam w badaniu procesu ruchu mrówki.


<h3>#Rozwiązanie problemu badawczego</h3>
Użytkownik może użyć domyślnych parametrów lub zmienić poniższe parametry w pliku config.<br>
- Liczba mrówek(ants_count)<br>
- Liczba iteracji(iter)<br>

Parametry mrówki takie jak pozycja(x,y) i kolor są generowane losowo. 

<h3>Krótki opis działania programu</h3>
1. Odczyt parametrów z pliku config.txt<br>
2. Wygenerowanie planszy przy użyciu biblioteki turtle.h<br>
3. Sprawdzenie poprawności podanych parametrów w pliku config.txt<br>
4. Ustawienie parametru dla każdej mrówki<br>
5. Dla każdej iteracji są wykonywane ruchy mrówki zgodne z algorytmem Langtona<br>
6. Zapisanie wyniku do pliku wyjściowego output.bmp<br>


Dzięki programowi możemy obserwować proces poruszania się mrówki. Ponadto przy większej ilości mrówek możemy podziwiać ciekawe, wręcz abstrakcyjne symulacje które normalnie byłyby ciężkie do przewidzenia.

<h3>#Przykład użycia wraz z zrzutami ekranu</h3>

Wygenerowany wynik w pliku wyjściowym output.bmp
<img src ="https://i.ibb.co/crnVbk5/output.png">

Parametry, które zostały użyte przy zrzucie

iter = 70000<br>
ants_count = 100


<h3>#Lista użytych dodatkowych bibliotek</h3>
- turtle.h<br>


<h3>#Opis kompilacji programu</h3>

Kompilacja programu przy użyciu komendy

>gcc proba.c turtle.c
