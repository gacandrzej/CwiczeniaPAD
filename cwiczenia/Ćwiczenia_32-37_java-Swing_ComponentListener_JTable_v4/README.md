# Ćwiczenia 32-37 -- JTable - TableModelListener

💡Na koniec zajęć prześlij pliki źródłowe i z danymi, wynikami do zasobu w
teams.
Potrzebne obrazki ściągnij z teams.

1. Napisz aplikację:

   ![image1](media/image1.png)

1. Dokumentacja:

   <https://docs.oracle.com/javase/8/docs/api/index.html?javax/swing/event/TableModelListener.html>

   <https://docs.oracle.com/javase/8/docs/api/java/awt/event/ComponentListener.html>

   <https://docs.oracle.com/javase/tutorial/uiswing/events/componentlistener.html>

   <https://docs.oracle.com/javase/8/docs/api/javax/swing/JTable.html>

   <https://docs.oracle.com/javase/tutorial/uiswing/components/table.html>

   <https://regex101.com/>

1. Utworzenie głównej klasy z
   konstruktorem. Okno responsywne, początkowo 60% szerokości ekranu i
   95% wysokości. Ustaw minimalne dopuszczalne rozmiary okna na
   800x600.

   ![image2](media/image2.png)

   ![image3](media/image3.png)

1. Dodaj

   ![image4](media/image4.png)

1. Dodaj model i ustaw identyfikatory dla
   kolumn:

   ![image5](media/image5.png)

   Napisz : model = new DefaultTableModel()
   W środkuCtrl+o i zacznij pisać metodę getColumnClass

   ![image6](media/image6.png)

   Dla return wpisz:

   ![image7](media/image7.png)

   ![image8](media/image8.png)

1. Utwórz metodę czytającą dane z pliku
   vegetables.txt i ją wywołaj. Format danych:

   ![image9](media/image9.png)

1. Ustaw dla tabeli wysokość wiersza na 80 oraz domyślne auto
   sortowanie dla kolumn.

   ![image10](media/image10.png)

1. Dodaj listener dla modelu, który reaguje na dodawanie usuwanie i
    edytowanie.

   ![image11](media/image11.png)

1. Dodanie panelu w układzie BorderLayout

1. Ustaw renderery i edytory

    ![image12](media/image12.png)

1. Dodaj obsługę dla przycisku edytuj

   ![image13](media/image13.png)

   ![image14](media/image14.png)

   ![image15](media/image15.png)

   ![image16](media/image16.png)

1. Dodaj obsługę pozostałych przycisków.

   ![image17](media/image17.png)

1. Dla listy obrazów wypisz wszystkie posiadane, ikonki

   ![image18](media/image18.png)

1. Wypisuj informacje o dodaniu, edycji i usunięciu:

   ![image19](media/image19.png)

   ![image20](media/image20.png)

1. KONIEC.🔚
