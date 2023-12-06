# Laboratorium 5 - przetwarzanie języka naturalnego
Opracowanie do wejściówki

### 1. Działanie rekurencyjnych sieci neuronowych.
W rekurencyjnej sieci neuronowej istnieje przynajmniej jedna warstwia neuronów, które oprócz połączeń z kolejną warstwą są połączone same ze sobą. Taka budowa sieci sprawia, że dane które pojawiają się na wyjściu wcześniej wpływają na wyniki sieci dla danych które pojawiły się później. Takie sieci przydają się do analizy danych sekwencyjnych.

### 2. Działanie mechanizmu atencji.
Dane są kodowane a następnie wprowadzane do fragmentu sieci neuronowej z mechanizmem atencji. W tym fragmencie sieci danym wejściowym przyporządkowane są wagi (określane na podstawie korelacji między tymi danymi), które określają które dane są najważniejsze. Następnie otrzymane wartości są wyprowadzane z mechanizmu atencji I wpływają na aktywacje kolejnych neuronów.

### 3. Statyczne osadzenia słów.
Sposób reprezentacja słowa w sieci neuronowj, zazwyczaj za pomocą wektora. Słowa o zbliżonym znaczeniu znajdują się bliżej siebie w przestrzeni.

### 4. Model językowy, w tym znakowy model językowy.
Model który określa prawdopodobieństwo wystąpienia określonego słowa w zdaniu. W przypadku znakowego modelu językowego – określonego znaku. Znakowy model językowy ma tą przewagę że łatwiej radzi sobie z dowolnymi słowami, I interpunkcją, jednak zazwyczaj wymaga większych modeli.

### 5. Pre-trening w kontekście modeli językowych.
Najlepiej do tworzenia uniwersalnych pre treningowanych sieci nadają się znakowe modele językowe które są bardzo eleastyczne, wymagają niewielkiego fine-tuneingu do poprawnego przewidywania wyników w danym zakresie.

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
