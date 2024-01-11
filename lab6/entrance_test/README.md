# Laboratorium 6 - podejmowanie decyzji
Opracowanie do wejściówki

### 1. Równowaga Nasha.
  Stan, gdzie zmiana strategi nie powoduje zwiększenia własnej oczekiwanej wygranej na podstawie aktualnej sytuacji, podczas gdy inni gracze zostają przy swoim planie działania.

### 2. Gra o sumie stałej.
  Gra, w której zysk jednego gracza oznacza stratę drugiego. Przypadkiem szególnym jest **gra o sumie zerowej**.

### 3. Strategie gry: optymalna, mieszana, czysta, oparta o heurystykę.
  Strategia to kompletny opis postępowania gracza w każdej sytuacji, w jakiej może się znaleźć.
  Rodzaje strategii:
  - **Mieszana** - strategia, która określa prawdopodobieństwa podjęcia konkretnego wyboru.
  - **Czysta (prosta)** - gracz dokonuje tylko jednego wyboru z prawdopodobieństwem jeden przez całą rozgrywkę.
  - **Oparta o heurystykę** - wykorzystanie wiedzy o problemie, dzięki czemu wyboru dokonujemy na podstawie aktualnego stanu gry.

### 4. Reprezentacja rozgrywki/drzewo gry.
  Reprezentacja opisująca każdy możliwy stan gry, np. kółko i krzyżyk z poszczególnymi pozycjami znaków, na początku zaczynamy od pustej planszy, na następnym poziomie mamy opisane 9 możliwych wyborów krzyżyka.

### 5. Algorytmy minmax, twierdzenie o minimaksie.
  Algorytm, który minimalizuje on nasze maksymalne straty lub maksymalizuje minimalne zyski.
  **Twierdzenie o minimaksie** mówi o tym, że gracz A może osiągnąć zysk najwyżej P, znając strategię gracza B, gracz B może osiągnąć najwyżej zysk -P, znając strategię gracza A.

### 6. Algorytm alpha-beta pruning.
  Optymalizacja algorytmu minimax, polegająca na pomijaniu odgałęzień drzewa, gdy wiemy, że nie da ona lepszego wyniku niż obecny. Zapisuje najlepszy wynik gracza maksymalizującego w zmiennej $\alpha$ i najlepszy gracza minimalizującego w zmiennej $\beta$, gdy $\alpha > \beta$ to ucinamy odnogę.

### 7. Algorytm monte carlo tree search z wariantem "pure".


### 8. Grafowa i drzewiasta strategia poszukiwania rozwiązań.


### 9. Dylemat więźnia.


### 10. Algorytm A*.
