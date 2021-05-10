# Projekt_JS
11. Program w Pythonie wywołujący funkcję z biblioteki dll liczącą iloczyn macierzy
Opis zadania
*Okno z przyciskiem "Uruchom obliczenia”, polem z informacjami o ostatnim
uruchomieniu (czas obliczeń w Pythonie, czas obliczeń w C/C++, czas potrzebny
na konwersję danych), oraz polami pozwalającymi wybrać:
-Liczbę kolumn macierzy,
-Liczbę wierszy macierzy,
-Zakres generowanych wartości w macierzach (od, do),
-Rodzaj generowanych wartości (liczby całkowite/rzeczywiste),
-Liczba powtórzeń mnożenia (do uśrednienia czasu obliczeń).
* Powinna dodatkowo istnieć możliwość ręcznego wprowadzenia niewielkich (do 
trzech wierszy i kolumn) macierzy które mają być przemnożone. Wprowadzanie
tych macierzy można zrealizować przez tablice pól tekstowych do wprowadzania
elementów macierzy.
* Po wciśnięciu przycisku "Uruchom obliczenia” generowane są dwie macierze o podanych przez użytkownika parametrach, które są następnie mnożone w. Pythonie oraz w CIC++ (kod mnożący wywoływany z pliku dl). Jeśli macierzy nie da się przemnożyć, ma zostać wyświetlony odpowiedni komunikat w oknie dialogowym (proszę użyć mechanizmu wyjątków).

* Implementacje w Pythonie i w C lub C++ mają być realizowane w dwóch klasach (MnozenieMacierzyCpp. MnozenieMacierzyPython) dziedziczących po klasie MnozenieMacierzy z metodą mnoz.
* Zapisywany jest czas obliczeń w pierwszym i drugim języku oraz czas przygotowania danych do przesłania do C/C++.
* Wyniki wpisywane są do poła z informacjami.
* Do wywoływania funkcji z dl należy stosować biblotekę ctypes (hllps:/docs.python.org/3.Gflioraryictypes.htm).

Testy

1. Wykonanie mnożenia (w Pythonie i przez dll):
2. [[1,0],[0,1]] ✖ [[2,3],[4,5]] = [[2,3],[4,5]]
3. 
4. Wykonanie mnożenia (w Pythonie i przez dll):
[[1,2,1],[4,-1,0]] ✖ [[0,1],[2,0],[-1,-1]] = [[-1,0],[-4,4]]

3. Wykonanie mnożenia (w Pythonie i przez dll):
[[1,2],[4,-2],[0,3]] ✖ [[0,1,-3],[2,-1,0]] = [[4,-1,-3],[-4,6,-12],[6,-3,0]]
  
4. Próba wykonania mnożenia macierzy 2x3 przez macierz 1x2 (oczekiwany komunikat o błędzie i możliwość kontynuowania pracy z programem bez ponownego uruchamiania.

5. Uzyskanie porównania czasów dla mnożenia macierzy 1x1, 10x10 50x50 (odpowiednio 100000, 1000 i 50 powtórzeń, liczby całkowite).

6. Uzyskanie porównania czasów dla mnożenia macierzy 200x200 (3 powtórzenia, liczby rzeczywiste).
