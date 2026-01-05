Ćwiczenia 6 -- klasy, dziedziczenie, polimorfizm, enkapsulacja
Na koniec zajęć prześlij pliki źródłowe z danymi, wynikami do zasobu w
teams.
1.  Utwórz nowy projekt.
2.  Nie importuj żadnych bibliotek, zostaną zaimportowane automatycznie.
3.  Stwórz package o nazwie komputery, prawy klawisz myszy na src
> ![](media/image1.png)
4.  Tworzymy klasę komputer o polach/atrybutach: producent, model i rok
    produkcji.
> ![](media/image2.png)
5.  ![](media/image3.png)
    Utwórz konstruktor dla tych pól.
> ![](media/image4.png)
6.  Utwórz obiekt klasy Komputer
> ![](media/image5.png)
![](media/image6.png)
7.  ![](media/image7.png)
    Utwórz gettery i setery dla wszystkich
    pól.
8.  Testujemy gettery i setery dla wszystkich pól, ale najpierw utwórz
    konstruktor bezargumentowy:
![](media/image8.png)
9.  Stwórz obiekt i nadaj/odczytaj wartości:
![](media/image9.png)
![](media/image10.png)
10. Widok po teście ( o ile dodasz wersję java 25):
> ![](media/image11.png)
11. Utwórz klasę potomną o nazwie Laptop, na package komputery prawy
    klawisz myszy i New:
> ![](media/image12.png)
>
> ![](media/image13.png)
12. Dodaj trzy nowe pola:
> ![](media/image14.png)
13. Dodaj konstruktor z klasy nadrzędnej z uwzględnieniem nowych pól:
> ![](media/image15.png)
>
> W drugim kroku:
>
> ![](media/image16.png)
>
> ![](media/image17.png)
14. Dodaj metodę toString w klasie Komputer oraz w Laptop:
> ![](media/image18.png)
W klasie Laptop ( dopisz super.toString()):
![](media/image20.png)
15. Utwórz obiekt klasy Laptop i nadaj/odczytaj wartości:
> ![](media/image21.png)
16. Utwórz metodę włącz w klasie nadrzędnej Komputer:
> ![](media/image22.png)
17. Nadpisz metodę włącz() w klasie Laptop:
> ![](media/image23.png)
>
> Dla klasy Laptop:
>
> ![](media/image24.png)
18. Przetestuj polimorfizm.
> ![](media/image25.png)
>
> ![](media/image26.png)
19. ![](media/image27.png)
    Utwórz klasę potomną o nazwie
    Smartfon.
20. Dodaj wszystko tak jak dla klasy Laptop.
> ![](media/image28.png)
21. ![](media/image29.png)
    Wykonaj testy.
22. Dodaj nowy package i utwórz klasę nadrzędną oraz dwie potomne według
    własnego pomysłu, testuj analogicznie jak wcześniej.
23. Dodatkowe zadania:
    a)  Dodaj klasę Desktop oraz potomną dla niej GamingDesktop,
    b)  Zaimplementuj metody equals() i hashCode()
> ![](media/image30.png)
c)  Dodaj test
> ![](media/image31.png)
>
> ![](media/image32.png)
24. KONIEC.
