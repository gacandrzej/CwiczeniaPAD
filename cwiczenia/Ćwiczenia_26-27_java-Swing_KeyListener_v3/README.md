# Ćwiczenia 26-27 -- gra pong - KeyListener

💡Na koniec zajęć prześlij pliki źródłowe i z danymi, wynikami do zasobu w
teams.
Potrzebne obrazki ściągnij z teams.

1. Napisz grę w swing i języku java, która polega na

    poruszaniu dwoma paletkami(zastosuj Rectangle i Graphics2D)

    i odbijaniu piłki paletkami.

    Lewa paletka, czerwona porusza się za pomocą klawiszy WSAD, a prawa,
    niebieska strzałek.

    Paletki mają czarną obwódkę.

    Zastosuj klasę Timer.

    Główna klasa rozszerza JFrame.

    Klasa wewnętrzna JPanel z paintComponent.

    Wynik na środku, stan początkowy 0:0.Otwórz nowy projekt.

1. Efekt końcowy:

   ![image1](media/image1.png)

1. Dokumentacja:

   <https://docs.oracle.com/javase/8/docs/api/java/awt/Rectangle.html>

   <https://docs.oracle.com/javase/8/docs/api/java/awt/event/KeyListener.html>

   <https://docs.oracle.com/javase/8/docs/api/javax/swing/Timer.html>

1. Utworzenie głównej klasy:

   ![image2](media/image2.png)

1. Zaimplementuj wszystkie wymagane metody.

   ![image3](media/image3.png)
   ![image4](media/image4.png)

1. Utworzenie konstruktora klasy PongGame

   ![image5](media/image5.png)

1. Utworzenie klasy wewnętrznej dla JPanel

   ![image6](media/image6.png)

1. Utworzenie konstruktora :

   ![image7](media/image7.png)

   i metody paintComponent()

   ![image8](media/image8.png)

1. Dodaj rysowanie piłki:

   ![image9](media/image9.png)

1. W konstruktorze klasy PongGame dodaj Timer:

   ![image10](media/image10.png)

1. W actionPerformed dodać zmianę współrzędnych piłki, np.:

   ![image11](media/image11.png)

   ![image12](media/image12.png)

   krawędzi oraz piłki od paletek

   na końcu dodać :

   ![image13](media/image13.png)

1. Dodać obsługę dla klawiszy np.:

   ![omahe14](media/image14.png)

1. Dodaj rysowanie paletek i wyniku.

   ![image15](media/image15.png)

1. Przeprowadź testy.

1. Dodaj płynność poruszania się paletki:

   ![image16](media/image16.png)

   ![image17](media/image17.png)

   ![image18](media/image18.png)

1. KONIEC.🔚
