# Laboratorium 5 - przetwarzanie języka naturalnego
Opracowanie do wejściówki

### 1. Działanie rekurencyjnych sieci neuronowych.


### 2. Działanie mechanizmu atencji.


### 3. Statyczne osadzenia słów.


### 4. Model językowy, w tym znakowy model językowy.


### 5. Pre-trening w kontekście modeli językowych.


### 6. Wsteczna propagacja błędu w czasie.
**Propagacja wsteczna** (ang. _backpropagation_ lub _backward propagation of errors_) – podstawowy algorytm uczenia nadzorowanego wielowarstwowych, jednokierunkowych sieci neuronowych. Oparty jest na błędzie warstwy wyjściowej, który jest przesyłany wstecz i wykorzystywany do zmiany wartości wag w poprzednich warstwach.

### 7. Długa pamięć krótkotrwałą (LSTM).
**Długa pamięć krótkotrwała (LSTM)** to rodzaj rekurencyjnej sieci neuronowej (RNN), która służy do modelowania zależności czasowych w danych. W szczególności może "pamiętać" przeszłe zdarzenia lub zależności z wcześniej obserwowanych czasów. LSTM to rodzaj sieci zaprojektowanej specjalnie, aby pomóc komputerowi zapamiętać informacje na dłużej niż jest to zwykle możliwe w przypadku rekurencyjnej sieci neuronowej. Model długiej pamięci krótkotrwałej działa przy użyciu "komórek", które przechowują informacje przez długi czas; po wykryciu nowego wejścia tworzone są nowe komórki, które łączą się z istniejącymi komórkami.

### 8. Architektura modeli: GPT, BERT.
- **GPT**:

  Model GPT (ang. _Generative Pre-trained Transformer_) jest oparty na architekturze Transformer, która jest szeroko stosowana w modelach NLP. W przeciwieństwie do wielu innych modeli, GPT jest wstępnie uczony na dużych zbiorach danych, co oznacza, że już posiada pewną zdolność generowania tekstu. GPT jest często używany w aplikacjach takich jak chatboty, samouczące się systemy odpowiedzi i generowanie tekstów. Transformery opierają się na _samo-atencji_, co oznacza, że model określa wagę słów w zdaniach, dzięki czemu lepiej rozumie ich kontekst.

- **BERT**:

  Model BERT (ang. _Bidirectional Encoder Representations From Transformers_), polega na nauce kontesktu słów, bazując na otoczeniu danego słowa.



### 9. Duże modele językowe (LLMs).
**LLM**, czyli **Large Language Model**, jest typem algorytmu sztucznej inteligencji (AI), który wykorzystuje techniki deep learningu i ogromne zbiory danych do zrozumienia, podsumowania, generowania i przewidywania nowych treści. Współczesne LLM wykorzystują sieci neuronowe transformer, zwane powszechnie transformerami. Dzięki dużej liczbie parametrów i modelowi transformera, LLM są w stanie zrozumieć i generować dokładne odpowiedzi bardzo szybko.
