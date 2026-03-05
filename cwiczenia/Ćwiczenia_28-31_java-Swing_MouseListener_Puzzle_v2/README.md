Ćwiczenia 28-31 -- puzzle - MouseListener
Na koniec zajęć prześlij pliki źródłowe i z danymi, wynikami do zasobu w
teams.
Potrzebne obrazki ściągnij z teams.
1.  Napisz puzzle z wykorzystaniem MouseListenera
2.  Efekt końcowy:
> ![](media/image1.png)
3.  Dokumentacja:
> <https://docs.oracle.com/javase/8/docs/api/java/awt/event/MouseListener.html>
>
> <https://docs.oracle.com/javase/8/docs/api/java/awt/image/BufferedImage.html>
4.  Utworzenie głównej klasy z konstruktorem.
> ![](media/image2.png)
5.  ![](media/image3.png)
    Dodanie panelu w układzie grid:
6.  W konstruktorze wywołaj metodę, która podzieli obrazek, np.:
> ![](media/image4.png)
>
> Sprawdzenie rozmiarów dla obrazka:
>
> ![](media/image5.png)
7.  Skorzystaj z klasy BufferedImage lub DrawImage, metody getSubimage
    do podzielenia obrazka na 9 części:
> ![](media/image6.png)
>
> ![](media/image7.png)
8.  Utworzenie klasy wewnętrznej, rozszerza JLabel lub JButton:
> ![](media/image8.png)
>
> Z konstruktorem:
>
> ![](media/image9.png)
9.
10. Utworzenie listenera w tej klasie:
> ![](media/image10.png)
11.
12. ![](media/image11.png)
    Dodaj metodę zamieniającą puzzle
    wewnątrz mousePressed(MouseEvent e), np.:
13. Na starcie losujemy pozycje elementów:
> ![](media/image12.png)
14. Przeprowadź testy.
15. Stwórz drugi projekt, w którym chcemy przeciągać puzzle.
16. ![](media/image13.png)
    Zaimplementuj listenery:
17. KONIEC.
