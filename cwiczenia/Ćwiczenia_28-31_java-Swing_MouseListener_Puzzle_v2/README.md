# Ćwiczenia 28-31 -- puzzle - MouseListener

💡Na koniec zajęć prześlij pliki źródłowe i z danymi, wynikami do zasobu w
teams.
Potrzebne obrazki ściągnij z teams.

1. Napisz puzzle z wykorzystaniem MouseListenera

1. Efekt końcowy:

   ![image1](media/image1.png)

1. Dokumentacja:

   <https://docs.oracle.com/javase/8/docs/api/java/awt/event/MouseListener.html>

   <https://docs.oracle.com/javase/8/docs/api/java/awt/image/BufferedImage.html>

1. Utworzenie głównej klasy z konstruktorem.

   ![image2](media/image2.png)

1. Dodanie panelu w układzie grid:

   ![image3](media/image3.png)

1. W konstruktorze wywołaj metodę, która podzieli obrazek, np.:

   ![image4](media/image4.png)

   Sprawdzenie rozmiarów dla obrazka:

   ![image5](media/image5.png)

1. Skorzystaj z klasy BufferedImage lub DrawImage, metody getSubimage
    do podzielenia obrazka na 9 części:

   ![image6](media/image6.png)

   ![image7](media/image7.png)

1. Utworzenie klasy wewnętrznej, rozszerza JLabel lub JButton:

   ![image8](media/image8.png)

   Z konstruktorem:

   ![image9](media/image9.png)

1. Utworzenie listenera w tej klasie:

   ![image10](media/image10.png)

1. Dodaj metodę zamieniającą puzzle
   wewnątrz mousePressed(MouseEvent e), np.:

   ![image11](media/image11.png)

1. Na starcie losujemy pozycje elementów:

   ![image12](media/image12.png)

1. Przeprowadź testy.

1. Stwórz drugi projekt, w którym chcemy przeciągać puzzle.

1. Zaimplementuj listenery:

   ![image13](media/image13.png)

1. KONIEC.🔚
