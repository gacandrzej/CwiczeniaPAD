Ćwiczenia 32-37 -- JTable - TableModelListener
Na koniec zajęć prześlij pliki źródłowe i z danymi, wynikami do zasobu w
teams.
Potrzebne obrazki ściągnij z teams.
1.  ![](media/image1.png)
    Napisz aplikację:
2.  Dokumentacja:
> <https://docs.oracle.com/javase/8/docs/api/index.html?javax/swing/event/TableModelListener.html>
>
> <https://docs.oracle.com/javase/8/docs/api/java/awt/event/ComponentListener.html>
>
> <https://docs.oracle.com/javase/tutorial/uiswing/events/componentlistener.html>
>
> <https://docs.oracle.com/javase/8/docs/api/javax/swing/JTable.html>
>
> <https://docs.oracle.com/javase/tutorial/uiswing/components/table.html>
>
> <https://regex101.com/>
3.  ![](media/image2.png)
    Utworzenie głównej klasy z
    konstruktorem. Okno responsywne, początkowo 60% szerokości ekranu i
    95% wysokości. Ustaw minimalne dopuszczalne rozmiary okna na
    800x600.
> ![](media/image3.png)
4.  ![](media/image4.png)
    Dodaj
5.  ![](media/image5.png)
    Dodaj model i ustaw identyfikatory dla
    kolumn:
Napisz : model = new DefaultTableModel()
W środkuCtrl+o i zacznij pisać metodę getColumnClass
> ![](media/image6.png)
>
> Dla return wpisz:
> ![](media/image7.png)
![](media/image8.png)
6.  ![](media/image9.png)
    Utwórz metodę czytającą dane z pliku
    vegetables.txt i ją wywołaj. Format danych:
7.  Ustaw dla tabeli wysokość wiersza na 80 oraz domyślne auto
    sortowanie dla kolumn.
> ![](media/image10.png)
8.  Dodaj listener dla modelu, który reaguje na dodawanie usuwanie i
    edytowanie.
> ![](media/image11.png)
9.  Dodanie panelu w układzie BorderLayout
10. ![](media/image12.png)
    Ustaw renderery i edytory
11. ![](media/image13.png)
    Dodaj obsługę dla przycisku edytuj
> ![](media/image14.png)
>
> ![](media/image15.png)
>
> ![](media/image16.png)
12. ![](media/image17.png)
    Dodaj obsługę pozostałych przycisków.
13. Dla listy obrazów wypisz wszystkie posiadane, ikonki
> ![](media/image18.png)
14. Wypisuj informacje o dodaniu, edycji i usunięciu:
> ![](media/image19.png)
>
> ![](media/image20.png)
15. KONIEC.
