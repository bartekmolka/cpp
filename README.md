# Programowanie w C++

*Krótka dokumentacja języka C++*

---

#### Dyrektywa #include

Umożliwia dołączanie bibliotek do języka np. string, cmath, time.h, cstdlib itd.

Przykład użycia: 

```cpp
#include <time.h>
```

#### Przestrzenie nazw

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

#### Funkcja główna

W niej odpala się program, wszystko co się w niej znajduje uruchomi się. Na jej końcu znajduje się polecenie:

```cpp
return 0;
```

Jeżeli zwraca ona 0, to program wykonał się poprawnie.

#### Typy zmiennych

Na początku zaznaczę, że jest ich dużo ale wymienię tylko te z którymi się możesz spotkać.

- typy całkowite - najważniejszy z nich to int

- typy rzeczywiste - float, double

- typy znakowe - char, przechowuje po prostu jeden znak (ale ma pewną magiczną moc)

- typ logiczny - bool, przechowuje wartość true (lub 1), false (lub 0)

- za pomocą bibliotek można dołączyć jeszcze typy takie jak string czy vector (tablice dynamiczne)

#### Polecenia cout i cin biblioteki iostream

Polecenie cout umożliwia 'wyświetlenie informacji.

```cpp
cout << "Hej Andzia";
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
