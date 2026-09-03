# Ćwiczenia 6 -- klasy, dziedziczenie, polimorfizm, enkapsulacja

Na koniec zajęć prześlij pliki źródłowe z danymi, wynikami do zasobu w
teams.

1. Utwórz nowy projekt.
1. Nie importuj żadnych bibliotek, zostaną zaimportowane automatycznie.
1. Stwórz package o nazwie komputery, prawy klawisz myszy na src

   ![image1](media/image1.png)

1. Tworzymy klasę komputer o polach/atrybutach: producent, model i rok
    produkcji.

   ![image2](media/image2.png)

   ![image3](media/image3.png)

1. Utwórz konstruktor dla tych pól.

   ![image4](media/image4.png)

1. Utwórz obiekt klasy Komputer

   ![image5](media/image5.png)
   ![image6](media/image6.png)

1. ![image7](media/image7.png)
    Utwórz gettery i setery dla wszystkich
    pól.
2. Testujemy gettery i setery dla wszystkich pól, ale najpierw utwórz
    konstruktor bezargumentowy:
![image8](media/image8.png)
3. Stwórz obiekt i nadaj/odczytaj wartości:
![image9](media/image9.png)
![image10](media/image10.png)
4. Widok po teście ( o ile dodasz wersję java 25):

> ![image11](media/image11.png)

1. Utwórz klasę potomną o nazwie Laptop, na package komputery prawy
    klawisz myszy i New:

> ![image12](media/image12.png)
>
> ![image13](media/image13.png)

1. Dodaj trzy nowe pola:

> ![image14](media/image14.png)

1. Dodaj konstruktor z klasy nadrzędnej z uwzględnieniem nowych pól:

> ![image15](media/image15.png)
>
> W drugim kroku:
>
> ![image16](media/image16.png)
>
> ![image17](media/image17.png)

1. Dodaj metodę toString w klasie Komputer oraz w Laptop:

> ![image18](media/image18.png)
W klasie Laptop ( dopisz super.toString()):
![image20](media/image20.png)

1. Utwórz obiekt klasy Laptop i nadaj/odczytaj wartości:

> ![image21](media/image21.png)

1. Utwórz metodę włącz w klasie nadrzędnej Komputer:

> ![image22](media/image22.png)

1. Nadpisz metodę włącz() w klasie Laptop:

> ![image23](media/image23.png)
>
> Dla klasy Laptop:
>
> ![image24](media/image24.png)

1. Przetestuj polimorfizm.

> ![image25](media/image25.png)
>
> ![image26](media/image26.png)

1. ![image27](media/image27.png)
    Utwórz klasę potomną o nazwie
    Smartfon.
2. Dodaj wszystko tak jak dla klasy Laptop.

> ![image28](media/image28.png)

1. ![image29](media/image29.png)
    Wykonaj testy.
2. Dodaj nowy package i utwórz klasę nadrzędną oraz dwie potomne według
    własnego pomysłu, testuj analogicznie jak wcześniej.
3. Dodatkowe zadania:
    a)  Dodaj klasę Desktop oraz potomną dla niej GamingDesktop,
    b)  Zaimplementuj metody equals() i hashCode()

> ![image30](media/image30.png)
c)  Dodaj test
> ![image31](media/image31.png)
>
> ![image32](media/image32.png)

1. KONIEC.
