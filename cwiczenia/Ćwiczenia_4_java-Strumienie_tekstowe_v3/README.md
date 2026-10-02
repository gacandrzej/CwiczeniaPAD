# Ćwiczenia 4 -- praca z PrintWriter, Scanner, FileWriter, BufferedWriter

Na koniec zajęć prześlij pliki źródłowe i z danymi, wynikami do zasobu w
teams.

1. Utwórz nowy projekt w katalogu na dysku C:

1. Użyte w ćwiczeniach biblioteki: ( zostaną zaimportowane
    automatycznie)

1. Dodaj nową klasę, w której utworzysz 6 metod:

    do zapisu danych strumieniem FileWriter,

    do odczytu danych strumieniem Scanner,

    do zapisu danych strumieniem BufferedWriter,

    do odczytu danych strumieniem BufferedReader,

    do zapisu danych strumieniem PrintWriter,

    do odczytu danych strumieniem BufferedReader zapisanych PrintWriterem.

1. Przykładowy kod wywołujący 4 pierwsze metody:

   ```java
   public static final String PATH_FILE = "plik_writera.txt";
    public static final String PATH_FILE_2 = "plik_buffered-writera.txt";
   public static final String PATH_FILE_3 = "plik_print-writera.txt";

    void main() {
        IO.println(String.format("Praca ze strumieniami!"));
       // testFileWriter();
       // testOdczytuScanner();
        testOdczytuFileReader();
        testZapisuBufferedWriter();
    }
   ```

1. Dokumentacja:

    <https://docs.oracle.com/javase/8/docs/api/java/io/FileWriter.html>

    <https://docs.oracle.com/javase/8/docs/api/java/util/Scanner.html>

    <https://docs.oracle.com/javase/8/docs/api/java/io/BufferedWriter.html>

    <https://docs.oracle.com/javase/8/docs/api/java/io/BufferedReader.html>

    <https://docs.oracle.com/javase/8/docs/api/java/io/PrintWriter.html>

    <https://docs.oracle.com/javase/8/docs/api/java/io/FileReader.html>

1. Realizacja: Utwórz metodę do zapisu danych strumieniem FileWriter.

   Dokumentacja:

   <https://docs.oracle.com/javase/8/docs/api/java/io/FileWriter.html>

   ```java
   private void testFileWriter() {
        try (FileWriter fw = new FileWriter(PATH_FILE)) {
            fw.write("New York Knicks\n");
            fw.write("Los Angeles Lakers\n");
            fw.write("Toronto Raptors\n");
            fw.write("Minesota Timberwolves");
        } catch (IOException e) {
            throw new RuntimeException(e);
        }
    }
   ```

1. Realizacja: Utwórz metodę do odczytu danych strumieniem Scanner.

   <https://docs.oracle.com/javase/8/docs/api/java/util/Scanner.html>

   ```java
   private void testOdczytuScanner() {
        String linia;
        try (Scanner sc = new Scanner(new File(PATH_FILE))) {
            while (sc.hasNextLine()) {
                linia = sc.nextLine();
                IO.println(linia);
            }
        } catch (FileNotFoundException e) {
            throw new RuntimeException(e);
        }

    }
   ```

1. Realizacja: Utwórz metodę do odczytu danych strumieniem FileReader.

   ```java
   private void testOdczytuFileReader() {
        try (FileReader fr = new FileReader(new File(PATH_FILE))) {
            int znak;
            while ((znak = fr.read()) != -1) {
                System.out.print((char) znak);
            }
        } catch (FileNotFoundException e) {
            throw new RuntimeException(e);
        } catch (IOException e) {
            throw new RuntimeException(e);
        }
    }
   ```

1. Realizacja: Utwórz metodę do zapisu danych strumieniem BufferedWriter.

   ```java
    private void testBufferedWriter() {
        try (BufferedWriter bw = new BufferedWriter(new FileWriter(PATH_FILE_2))) {
            bw.write("Decathlon CMA CGM Team");
            bw.newLine();
            bw.write("Bahrain – Victorious");
            bw.newLine();
            bw.write("UAE Team Emirates – XRG");
            bw.newLine();
            bw.write("Lidl – Trek");
            bw.newLine();
        } catch (IOException e) {
            throw new RuntimeException(e);
        }
    }
   ```

   <https://docs.oracle.com/javase/8/docs/api/java/io/BufferedWriter.html>

1. Realizacja: Utwórz metodę do odczytu danych strumieniem BufferedReader.

   Dokumentacja:

   <https://docs.oracle.com/javase/8/docs/api/java/io/BufferedReader.html>

   <https://docs.oracle.com/javase/8/docs/api/java/io/FileReader.html>

   ```java
   private void testBufferedReader() {
        String line;
        try (BufferedReader br = new BufferedReader(new FileReader(PATH_FILE_2))) {
            while ((line = br.readLine()) != null) {
                System.out.println(line);
            }
        } catch (FileNotFoundException e) {
            throw new RuntimeException(e);
        } catch (IOException e) {
            throw new RuntimeException(e);
        }
    }
   ```

1. Realizacja: Utwórz metodę zapisującą dane: tekst, liczbę całkowitą,
    rzeczywistą oraz datę do pliku z pomocą PrintWritera.

   Dokumentacja:

   <https://docs.oracle.com/javase/8/docs/api/java/io/PrintWriter.html>

   ![image6](media/image6.png)

   ```java
   private void zapisPrintWriter() {
        Date date = new Date();
        IO.println("date="+date);
        System.out.printf("%tT",date);
        System.out.println(System.lineSeparator());
        System.out.printf("%s %tB %<te, %<tY", " Current date: ", date);
        /*
        Let’s look at the available format specifiers available for printf:
        %c character
        %d decimal (integer) number (base 10)
        %e exponential floating-point number
        %f floating-point number
        %i integer (base 10)
        %o octal number (base 8)
        %s String
        %u unsigned decimal (integer) number
        %x number in hexadecimal (base 16)
        %t formats date/time
        %% print a percent sign
        \% print a percent sign
         */
        try (PrintWriter printWriter = new PrintWriter(PATH_FILE_3)) {

            printWriter.println("Regular text!!!");
            printWriter.println(3.23f);
            printWriter.write(67);
            printWriter.printf("\n%d\n",35);
            printWriter.printf("Liczba e=%.2f %n",Math.E);
            /*
            Date formatting has the following special characters
            A/a - Full day/Abbreviated day B/b - Full month/Abbreviated month
            d - formats a two-digit day of the month
            m - formats a two-digit month
            Y - Full year/Last two digits of the Year
            j - Day of the year
            ‘H’, ‘M’, ‘S’ - Hours, Minutes, Seconds ‘L’, ‘N’ – to represent
            the time in milliseconds and nanoseconds accordingly
            ‘p’ – AM/PM ‘z’ – prints out the difference from GMT.
             */
            printWriter.printf("%tT",date);
            printWriter.printf("%s %tB %<te, %<tY", " Current date: ", date);

        } catch (FileNotFoundException e) {
            throw new RuntimeException(e);
        } catch (IOException e) {
            throw new RuntimeException(e);
        }
    }
   ```

1. Realizacja: Odczytaj dane zapisane PrintWriterem za pomocą BufferedReadera.

   ```java
   private static void odczytBufferedReader() {
        int bufferSize =4096;
        try (BufferedReader reader = new BufferedReader(new FileReader(PATH_FILE_3),bufferSize)) {
            String s = "";
            while((s = reader.readLine()) != null) {
                System.out.println(s);
            }
        } catch (FileNotFoundException e) {
            throw new RuntimeException(e);
        } catch (IOException e) {
            throw new RuntimeException(e);
        }
    }
   ```

   Wynik:

   ```text
   Regular text!!!

    3.23
    C
    35
    Liczba e=2,72
    13:47:18 Current date:  października 2, 2026

   ```

1. Wylosować 10 liczb i zapisać do pliku printwriterem oddzielając
    średnikiem każdą liczbę.

    Odczytać scannerem liczby, następnie dodać je do listy.

    Realizacja:

    ```java
    private void losujZapiszLiczbyPrintWriter(int n) {
        Random random = new Random();
        try (PrintWriter pr = new PrintWriter(PATH_FILE_Liczby)) {
            for (int i = 0; i < n; i++) {
                pr.print(random.nextInt(10,100));
                if (i < n - 1) pr.print(";");
            }
        } catch (FileNotFoundException e) {
            throw new RuntimeException(e);
        }

    }
    ```

    Odczyt, na dwa sposoby:

    ```java
    private void odczytLiczbScannerDodanieDoListy() {
        try (Scanner sc = new Scanner(new File(PATH_FILE_Liczby))) {
            List<Integer> lista = new ArrayList<>();
            sc.useDelimiter(";");
            while (sc.hasNextInt()) {
                int liczba = sc.nextInt();
                lista.add(liczba);
                IO.print(liczba+" ");
            }
        } catch (FileNotFoundException e) {
            throw new RuntimeException(e);
        }
    }
    ```

    ![image11](media/image11.png)

1. Wykorzystaj kod do realizacji zadania domowego.

1. KONIEC. 😀
