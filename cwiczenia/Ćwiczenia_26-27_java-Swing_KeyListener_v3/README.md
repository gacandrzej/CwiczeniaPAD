Ćwiczenia 26-27 -- gra pong - KeyListener
Na koniec zajęć prześlij pliki źródłowe i z danymi, wynikami do zasobu w
teams.
Potrzebne obrazki ściągnij z teams.
1.  Napisz grę w swing i języku java, która polega na
> poruszaniu dwoma paletkami(zastosuj Rectangle i Graphics2D)
>
> i odbijaniu piłki paletkami.
>
> Lewa paletka, czerwona porusza się za pomocą klawiszy WSAD, a prawa,
> niebieska strzałek.
>
> Paletki mają czarną obwódkę.
>
> Zastosuj klasę Timer.
>
> Główna klasa rozszerza JFrame.
>
> Klasa wewnętrzna JPanel z paintComponent.
>
> Wynik na środku, stan początkowy 0:0.Otwórz nowy projekt.
2.  ![](media/image1.png)
    Efekt końcowy:
3.  Dokumentacja:
> <https://docs.oracle.com/javase/8/docs/api/java/awt/Rectangle.html>
>
> <https://docs.oracle.com/javase/8/docs/api/java/awt/event/KeyListener.html>
>
> <https://docs.oracle.com/javase/8/docs/api/javax/swing/Timer.html>
4.  ![](media/image2.png)
    Utworzenie głównej klasy:
5.  Zaimplementuj wszystkie wymagane metody.
![](media/image3.png)
![](media/image4.png)
6.  Utworzenie konstruktora klasy PongGame
> ![](media/image5.png)
7.  Utworzenie klasy wewnętrznej dla JPanel
> ![](media/image6.png)
8.  ![](media/image7.png)
    Utworzenie konstruktora :
> i metody paintComponent()
>
> ![](media/image8.png)
9.  ![](media/image9.png)
    Dodaj rysowanie piłki:
10. W konstruktorze klasy PongGame dodaj Timer:
> ![](media/image10.png)
11. W actionPerformed dodać zmianę współrzędnych piłki, np.:
> ![](media/image11.png)
>
> ![](media/image12.png)
> krawędzi oraz piłki od paletek
>
> na końcu dodać :
>
> ![](media/image13.png)
12. ![](media/image14.png)
    Dodać obsługę dla klawiszy np.:
13. ![](media/image15.png)
    Dodaj rysowanie paletek i wyniku.
14. Przeprowadź testy.
15. Dodaj płynność poruszania się paletki:
> [![](media/image16.png)
>
> ![](media/image17.png)
![](media/image18.png)
16. KONIEC.
