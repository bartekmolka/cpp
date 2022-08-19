# Programowanie w C++

*Krótka dokumentacja języka C++*

---

### Dyrektywa #include

Umożliwia dołączanie bibliotek do języka np. string, cmath, time.h, cstdlib itd.

Przykład użycia: 

```cpp
#include <time.h>
```

### Przestrzenie nazw

Można zredukować kod z:

```cpp
std::cout << "Hello World!"
```

do:

```cpp
cout << "Hello World!"
```

to wszystko dzięki umieszczeniu polecenia:

```cpp
using namespace std;
```

### Funkcja główna

W niej odpala się program, wszystko co się w niej znajduje uruchomi się. Na jej końcu znajduje się polecenie:

```cpp
return 0;
```

Jeżeli zwraca ona 0, to program wykonał się poprawnie.

### Typy zmiennych

Na początku zaznaczę, że jest ich dużo ale wymienię tylko te z którymi się możesz spotkać.

- typy całkowite - najważniejszy z nich to int

- typy rzeczywiste - float, double

- typy znakowe - char, przechowuje po prostu jeden znak (ale ma pewną magiczną moc)

- typ logiczny - bool, przechowuje wartość true (lub 1), false (lub 0)

- za pomocą bibliotek można dołączyć jeszcze typy takie jak string czy vector (tablice dynamiczne)

### Polecenia cout i cin biblioteki iostream

Polecenie cout umożliwia 'wyświetlenie informacji.

```cpp
cout << "Hej";
```

Polecenie cin umożliwia wrzucenie danych.

```cpp
int x = 0; //deklaracja zmiennej o nazwie 'x' i wartosci 0
cout << "Hej! Podaj wartość zmiennej: ";
cin >> x;
cout << "Oto wartość twojej zmiennej: " << x; 
// wyświetli się wpisana wartość
```

Aby zapamiętać co dana instrukcja robi warto zauważyc kierunki strzałek.

### Komentarze w C++

Komentarz jednolinijkowy:

```cpp
cout << "Test działania komentarza"; // To jest komentarz
```

Komentarz wielolinijkowy:

```cpp
cout << "Test działania komentarza"; /* To jest komentarz
 wielolinijkowy */
```

### Operacje matematyczne

Podstawowe z nich to:

- dodawanie +

- odejmowanie -

- mnożenie *

- dzielenie /

- modulo % (reszta z dzielenia liczby przez 2)

#### Zapisy skrócone

Zamiast:

```cpp
x = x + 1
```

Można zapisać

```cpp
x += 1
```

Oraz analogicznie z pozostałymi operatorami

#### Inkrementacja i dekrementacja

Występują ich łącznie 4 rodzaje.

Preinkrementacja to zwiększenie wartości zmiennej o jeden przed wykonaniem polecenia, a postinkrementacja to zwiększenie wartości o jeden po wykonaniu polecenia. 

```cpp
int x = 0;
cout << ++x; // wyświetli się 1
int a = 0;
cout << a++;// wyświetli się 0
```

Predekrementacja to zmniejszenie wartości zmiennej o jeden przed wykonaniem polecenia, a postdekrementacja to zmniejszenie wartości o jeden po wykonaniu polecenia.

```cpp
int x = 1;
cout << --x; // wyświetli się 0
int a = 1;
cout << a--;// wyświetli się 1
```

### Operatory porównania

Służa do, jak sama nazwa wskazuje, porównywania wartości zmiennych w celu np wykonania konkretnego fragmentu kodu. 

| Operator | Krótki opis                         |
| -------- | ----------------------------------- |
| >        | ... jest większe od ...             |
| >=       | ... jest większe lub równe niż ...  |
| <        | ... jest mniejsze od ...            |
| <=       | ... jest mniejsze lub równe niż ... |
| ==       | ... jest równe ...                  |
| !=       | ... jest różne od ...               |

```cpp
int x = 1;
int a = 1;
bool result = a < x; 
cout << result;/* wyświetli się 0 (false), gdyż zmienna a jest tej samej 
wartości co zmienna x */
```

### Instrukcja warunkowa If

Pozwala ona wykonać pewien fragment kodu na podstawie danego warunku

```cpp
int wiek;
cin >> wiek;
if( wiek >= 18 )
{
    cout << "Jesteś pełnoletni" << endl;
}
return 0;
```
