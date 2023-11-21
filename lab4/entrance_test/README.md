# Laboratorium 4 - konwolucyjne sieci neuronowe
Opracowanie do wejściówki


### 1. Operacja konwolucji (splotu).


### 2. Warstwa konwolucyjna w sieci neuronowej.


### 3. Warstwa poolingowa.


### 4. Budowa typowej sieci konwolucyjnej (np. LeNet).


### 5. Detekcja obiektów.
Za pomocą konwolucyjnych sieci neuronowych jesteśmy w stanie z wysoką wydajnością rozponznawać obiekty. W porównaniu do MLP, gdzie tworząc warstwy dla macierzy pojedynczych pikseli, sieć połączeń potrafi być naprawdę duża, dodatkowo sieci MLP nie radzą sobie ze zmianą położenia obiektu.

### 6. Wybór bounding-boxów, kandydatury, confidence levels.
Bounding-boxy wybieramy w zależności od problematyki, dla której konstruujemy model. Ogólnymi zasadami przy ich wyborze są: konsekwencja i jak najbardziej dokładne dopasowanie ich granic (tak, aby zminimalizować niepotrzebny szum).

### 7. Fine-tuning i pre-trening, wykorzystywanie gotowych sieci.
Fine-tuning to przeniesienie uczenia w postaci określenia wag innego przetrenowanego już modelu, korzystając z nowego zbioru danych, może być przeprowadzony na całej sieci neoronowej lub jej podzbiorze. Sieć, która została wykorzystana do obliczenia początkowych wag użytych w drugim treningu jest siecią pre-treningową. Do takiego tuningu można także skorzystać z gotowych już sieci neuronowych, które realizują podobne zadanie.
