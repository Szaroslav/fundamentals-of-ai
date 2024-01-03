# Laboratorium 7 - systemy rekomendacyjne
  Opracowanie do wejściówki

### 1. Globalne systemy rekomendacyjne.
  Globalne systemy rekomendacyjne biorą pod uwagę ogólne cechy przedmiotu i są oceniane dla całej społeczności, nie pod konkretnych użytkowników. Korzystają z nich typowo strony z wiadomościami, żeby ułożyć kolejność postów na stronie, np. HackerNews, Reddit. Przydają się też, gdy nie mamy dość informacji o użytkowniku, aby dokonać personalizacji.

### 2. Systemy collaborative filtering (CF) & content-based.
  - **Collaborative filtering (CF)** - oparte o historię interakcji użytkowników z przedmiotami, czyli zwykle o historię ocen. Stąd pochodzą np. rekomendacje "użytkownicy podobni do ciebie oglądali także X", gdzie podobieństwo mierzy się na podstawie tego, jak bardzo podobne mieliśmy w przeszłości oceny do innych użytkowników. Co ważne, takie podejście nie wymaga żadnej inżynierii cech, a jedynie zapamiętania historii ocen / transakcji / interakcji.
  - **Content based (CB)** - dużo bardziej podobne do klasycznego ML, tworzymy wektory cech dla przedmiotów, użytkowników i wykorzystujemy je w klasyfikacji (np. rekomendować lub nie) lub regresji (np. liczba gwiazdek).

### 3. Problem zimnego startu (cold start).
  Problem zimnego startu polega na podzbiorze użytkowników (najczęściej nowych), o których mało lub w ogóle nic nie wiemy.
  Można sobie z nim radzić na kilka sposobów:
    - rekomendować najpopularniejsze przedmioty;
    - rekomendować przedmioty o najwyższych ocenach;
    - użyć globalnego (niepersonalizowanego) systemu rekomendacyjnego, np. przewidywanie średniej dla przedmiotu;
    - używać systemu content-based, bo radzą sobie dobrze przy małej liczbie interakcji;
    - poprosić użytkownika przy pierwszym logowaniu o podanie pierwszych preferencji (nie zawsze możliwe).

### 4. Macierz interakcji, explicit vs implicit feedback.
  Macierz interakcji to macierz, gdzie wierszami są użytkownicy, natomiast kolumnami jakaś metryka interakcji, np. ocena przedmiotu.
  - **Explicit feedback** - kiedy użytkownicy jawnie podają oceny, np. ocena hotelu w skali 1-10, liczba gwiadek dla przedmiotu. Wymaga to większej proaktywności użytkowników, więc potencjalnie możemy mieć mniej danych, ale są często bardziej precyzyjne. Są też typowo prostsze teoretycznie (matematycznie), bo mają znany z góry, ograniczony zakres możliwych wartości.
  - **Implicit feedback** - kiedy jakość przedmiotu wyznaczają akcje użytkowników, np. liczba kliknięć, liczba udostępnień. Takie informacje można gromadzić automatycznie i bardzo łatwo, ale mogą być mało precyzyjne (np. przypadkowe kliknięcia, boty). Algorytmy dla takich problemów są też cięższe do zaprojektowania, bo mamy tylko wartości nieujemne i typowo nieograniczone z góry.

### 5. Podział losowy i czasowy (time split).
  - Podział losowy to podzielenie zbiorów danych w sposób losowy, w dokładnie taki sam sposób jak robiliśmy to przy poprzednich zadaniach.
  - Podział czasowy to wyodrębnienie najnowszych cech z całego zbioru.

### 6. CF oparte o sąsiedztwo (neighborhood-based).
  Z macierzy ocen $R$ znajdujemy podobnych użytkowników do nas albo przedmioty, które nam się podobają (np. wystawione przez nas opinie) i na podstawie tego dokonujemy rekomendacji.

### 7. CF oparte o rozkład macierzy (matrix factorization).
  Macierz ocen $R_{N \times M}$ przybliżamy za pomocą dwóch macierzy: macierzy użytkowników $W_{N \times K}$ i macierzy przedmiotów $U_{K \times N}$, gdzie $N$ to liczba użytkowników, a $M$ przedmiotów. Predykcji dokonujemy za pomocą iloczynu skalarnego wiersza $W$ z kolumną $U$.

### 8. Metryki jakości w systemach rekomendacyjnych, metryki @k, NDCG.
  - **Precision@k** - precyzja (liczba poprawnych przedmiotów podzielona przez liczbę wszystkich przedmiotów) na $k$ pierwszych przedmiotach, uporządkowanych w sposób dowolny.
  - **Recall@k** - czułość na $k$ pierwszych przedmiotach; liczba poprawnych przedmiotów w $k$ pierwszych przedmiotach podzielona przez **łączną** ich liczbę.
  - **MAP@k** - średnia precyzji na $k$ pierwszych przedmiotach: $\frac{1}{N}[\Sigma_i^K(P@i) \cdot R(i)$].
  - **NDCG (Normilized Discounted Cumulative Gain)** - $\frac{DCG}{IDCG}$.
