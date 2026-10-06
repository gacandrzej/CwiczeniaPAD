# Ćwiczenia 5 -- praca z ObjectOutputStream, DataOutputStream,FileOutputStream itd

Na koniec zajęć prześlij pliki źródłowe i z danymi, wynikami do zasobu w
teams.

1. Utwórz nowy projekt w katalogu na dysku C:

1. Użyte w ćwiczeniach biblioteki: ( zostaną zaimportowane
    automatycznie)

1. Dodaj nową klasę, w której utworzysz 8 metod:

   - do zapisu danych strumieniem PrintWriter,
   - do odczytu danych strumieniem Scanner+parsowanie,
   - do zapisu danych strumieniem ObjectOutputStream,
   - do odczytu danych strumieniem ObjectInputStream,
   - do zapisu danych strumieniem DataOutputStream,
   - do odczytu danych strumieniem DataInputStream,
   - do zapisu danych strumieniem FileOutputStream,
   - do odczytu danych strumieniem FileInputStream,

1. Zadanie 1: PrintWriterem zapisać stringa z danymi
    dla trzech osób:

   ```java
   String testData = "John,25,75000.50,true\nAnna,30,80000.75,false\nPiotr,35,90000.25,true";
   ```

   Następnie sparsować i odczytać dane scanerem.

1. Zadanie 2: Zapisz listę języków programowania do pliku z pomocą
    ObjectOutputStream,

   następnie odczytaj tę listę i wypisz na ekran.

   Zadanie dodatkowe zapisz i odczytaj obiekt klasy.

1. Zadanie 3: Z wykorzystaniem strumieni
    DataOutputStream/ DataInputStream zapisz i odczytaj minimum 5 typów
    danych.

   ![image3](media/image3.png)

1. Zadanie 4: Skopiować wybrany obrazek \*.png lub inny z pomocą
    FileInputStream /FileOutputStream,

1. Realizacja zadania 1:

   ```java
   private static void testScanner() {
        System.out.println("4. Scanner:");

        // Używamy konkretnego delimitera
        String testData = "John,25,75000.50,true\nAnna,30,80000.75,false\nPiotr,35,90000.25,true";

        // Zapis danych
        try (PrintWriter writer = new PrintWriter(tekstowyPath)) {
            writer.print(testData);
        } catch (FileNotFoundException e) {
            e.printStackTrace();
        }

        // Odczyt z custom delimiterem
        try (Scanner scanner = new Scanner(new File(tekstowyPath))) {
            System.out.println("Odczyt z parsowaniem typów:");
            /**
             * \\r - carriage return (powrót karetki)
             * ? - oznacza "0 lub 1 raz" (opcjonalny)
             * \\n - newline (nowa linia)
             */
            scanner.useDelimiter(",|\\r?\\n"); // delimiter: przecinek lub nowa linia

            while (scanner.hasNext()) {
                try {
                    String name = scanner.next();
                    int age = Integer.parseInt(scanner.next());
                    double salary = Double.parseDouble(scanner.next());
                    boolean active = Boolean.parseBoolean(scanner.next());

                    System.out.printf("Name: %s, Age: %d, Salary: %.2f, Active: %b\n",
                            name, age, salary, active);

                } catch (Exception e) {
                    System.out.println("Błąd parsowania: " + e.getMessage());
                    break;
                }
            }

        } catch (FileNotFoundException e) {
            System.out.println("Plik nie znaleziony: " + e.getMessage());
        }
        System.out.println("---");
    }
   ```

1. Realizacja zadania 2:

   ![image6](media/image6.png)

1. Realizacja zadania 3:

   ![image7](media/image7.png)

1. Realizacja zadania 4:

   ![image8](media/image8.png)

   ![image9](media/image9.png)

1. KONIEC.🔚
