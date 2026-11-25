# Ćwiczenia 12 -- praca z JFrame, JComboBox, ItemListener

Na koniec zajęć prześlij pliki źródłowe i z danymi, wynikami do zasobu w
teams.

1. Utwórz nowy projekt w katalogu na dysku C:

1. Dodaj podstawowe metody

   ![image1](media/image1.png)

1. Ikony pobierz z katalogu Obrazy z teams: plik sport.zip.

1. Postać aplikacji do testów:

   ![image2](media/image2.png)

1. Przygotuj panel dla checkbox i umieść go na północ.

1. Przygotuj panel na obrazki w układzie gridLayout(3,3) i umieść panel w centrum.

1. Zaznaczenie danego checkboxa dodaje obrazek do panelu, odznaczenie powoduje zniknięcie.

1. Zastosuj obramowania dla paneli oraz obrazków.

1. Popraw wygląd aplikacji poprzez:

   - dobór czcionki, klasa Font,
   - wyświetlenie całych napisów na przyciskach,
   - dodaj ikonę aplikacji,
   - dodaj kolory.

1. Zmodyfikuj klasę tak, aby implementowała ItemListener.

   ```java
   /**
   * Klasa SportImageAppIconSport
   * <p>
   * Aplikacja Swing wyświetlająca listę sportów do wyboru za pomocą JCheckBox.
   * Po zaznaczeniu sportu, jego ikona i nazwa pojawiają się w panelu obrazów.
   */
   public class SportImageAppIconSport extends JFrame implements ItemListener {
   ```

1. Dodaj klasę z testem sprawdzającą czy dodałeś/aś ikonę aplikacji.

   ![testy](../../media/2026-11-25-13-37-15.png)

1. Koniec.🔚
