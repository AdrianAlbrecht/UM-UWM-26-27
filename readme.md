# Uczenie Maszynowe UWM, semestr 5, rok akademicki 2026/27

## 1. Cel i zakres przedmiotu

Celem przedmiotu jest zapoznanie osób studiujących z podstawowymi pojęciami, metodami oraz wybranymi algorytmami **uczenia maszynowego**, ze szczególnym naciskiem na zrozumienie sposobu działania poszczególnych algorytmów, ich matematycznych i informatycznych podstaw oraz praktycznej implementacji.

W trakcie ćwiczeń laboratoryjnych część algorytmów będzie implementowana **samodzielnie od podstaw**, natomiast w przypadku bardziej rozbudowanych metod wykorzystywane będą również istniejące implementacje dostępne w bibliotekach uczenia maszynowego.

Celem takiego podejścia jest zarówno poznanie mechanizmu działania algorytmu, jak również zdobycie umiejętności jego poprawnego wykorzystania, konfiguracji oraz interpretacji uzyskiwanych rezultatów.

Jest to zgodne z efektami uczenia się określonymi w sylabusie, według których osoba studiująca powinna potrafić zarówno zaimplementować wybrane modele uczenia maszynowego, jak i wykorzystywać istniejące implementacje oraz dobierać odpowiednie algorytmy do rozwiązywanego problemu. 

W trakcie zajęć poruszone zostaną m.in.:

- przygotowanie danych na potrzeby algorytmów uczenia maszynowego,
- redukcja wymiarowości za pomocą **Principal Component Analysis (PCA)**,
- matematyczne podstawy PCA oraz samodzielna implementacja tego algorytmu,
- **Support Vector Machines (SVM)**,
- **reguła uczenia Hebba**,
- **sieć Hopfielda** jako przykład pamięci asocjacyjnej,
- drzewa decyzyjne,
- lasy losowe,
- metody zespołowe,
- **bagging**,
- **boosting**, w szczególności AdaBoost,
- algorytm **K-Means**,
- algorytm **Fuzzy C-Means**,
- podstawowe elementy logiki rozmytej niezbędne do zrozumienia Fuzzy C-Means,
- dobór parametrów i hiperparametrów wybranych algorytmów,
- analiza wpływu parametrów na działanie algorytmu,
- porównywanie sposobu działania różnych metod,
- analiza zalet, ograniczeń i typowych zastosowań poszczególnych algorytmów.

Na ćwiczeniach nie będzie realizowany pełny blok dotyczący współczesnych sieci neuronowych. **Reguła Hebba i sieć Hopfielda stanowią wyjątek**, realizowany jako klasyczne mechanizmy uczenia i pamięci asocjacyjnej.

---

## 2. Oprogramowanie

Na zajęciach wykorzystywane będzie przede wszystkim środowisko umożliwiające implementację i analizę algorytmów uczenia maszynowego.

W przypadku większości przykładów oraz materiałów prowadzącego preferowany będzie **Python 3.10 lub nowszy**.

Zalecane oprogramowanie:

- **Python 3.10+**,
- **Visual Studio Code**, PyCharm lub inne IDE obsługujące wybrany język,
- biblioteki Python, m.in.:
  - NumPy,
  - pandas,
  - matplotlib,
  - scikit-learn,
- opcjonalnie Git do zarządzania kodem projektu.

W zależności od realizowanego zagadnienia konieczna może być instalacja dodatkowych bibliotek. Informacja taka będzie przekazywana na odpowiednich zajęciach.

Sylabus zakłada znajomość podstaw programowania, operacji macierzowych oraz umiejętność korzystania z bibliotek danego języka programowania i ich dokumentacji.

---

## 3. Sposób prowadzenia zajęć

Zajęcia będą miały charakter praktyczny.

W zależności od omawianego zagadnienia stosowane będą dwa podejścia.

### A. Implementacja algorytmu od podstaw

Dla wybranych algorytmów celem zajęć jest dokładne poznanie sposobu ich działania.

W takim przypadku **nie korzystamy z gotowej implementacji danego algorytmu jako rozwiązania zadania**.

Dotyczy to w szczególności algorytmów wskazanych przez prowadzącego jako zadania implementacyjne, np. **PCA**.

W implementacji można korzystać z podstawowych bibliotek matematycznych i narzędzi programistycznych, jednak właściwa logika algorytmu powinna zostać zaimplementowana przez osobę studiującą.

### B. Wykorzystanie istniejących implementacji

W przypadku pozostałych algorytmów nacisk zostanie położony na:

- zrozumienie ich działania,
- poprawny dobór metody,
- konfigurację parametrów,
- przeprowadzanie eksperymentów,
- obserwację wpływu parametrów na działanie algorytmu,
- interpretację uzyskanych rezultatów,
- porównanie zachowania różnych metod.

Dotyczy to m.in. Random Forest, AdaBoost, K-Means oraz innych bardziej zaawansowanych algorytmów dostępnych w popularnych bibliotekach uczenia maszynowego.

Takie rozdzielenie odpowiada dwóm efektom określonym w sylabusie: umiejętności samodzielnej implementacji wybranych modeli oraz umiejętności korzystania z istniejących implementacji.

---

## 4. Sztuczna inteligencja i samodzielność pracy

Narzędzia sztucznej inteligencji są współcześnie częścią warsztatu programisty i **nie obowiązuje ogólny zakaz ich używania podczas całego przedmiotu**.

Istnieje jednak istotne rozróżnienie pomiędzy zadaniami, których celem jest **poznanie działania konkretnego algorytmu**, a zadaniami, których celem jest jego praktyczne zastosowanie.

### Zadania implementacyjne

W zadaniach wyraźnie oznaczonych jako **implementacja algorytmu od podstaw** kod implementujący właściwy algorytm musi zostać napisany samodzielnie.

W takich zadaniach **niedopuszczalne jest wygenerowanie implementacji algorytmu przez ChatGPT, Codex, Gemini, Copilot lub inne narzędzie generatywnej AI i przedstawienie jej jako własnej implementacji**.

Celem tych ćwiczeń nie jest możliwie szybkie uzyskanie działającego programu, ale **zrozumienie działania algorytmu**.

Można korzystać z:

- dokumentacji języka programowania,
- dokumentacji bibliotek matematycznych,
- materiałów dydaktycznych,
- literatury,
- własnych notatek.

### Pozostałe zadania i projekt

W zadaniach polegających na praktycznym wykorzystaniu istniejących algorytmów korzystanie z narzędzi AI jest dopuszczalne.

Każde istotne wykorzystanie AI powinno jednak zostać opisane, np.:

- jakie narzędzie zostało wykorzystane,
- do czego zostało wykorzystane,
- jaki był zakres wygenerowanego rozwiązania,
- co zostało wykonane samodzielnie,
- jakie elementy zostały zmodyfikowane,
- w jaki sposób sprawdzono poprawność rozwiązania.

**Znajomość własnego kodu jest obligatoryjnym warunkiem zaliczenia.**

Osoba studiująca musi być w stanie wyjaśnić:

- co robi wskazany fragment programu,
- jak działa wykorzystany algorytm,
- dlaczego zastosowano właśnie tę metodę,
- jakie znaczenie mają najważniejsze parametry,
- jak zmiana parametrów wpływa na działanie algorytmu,
- jakie są zalety i ograniczenia zastosowanego rozwiązania,
- jakie wnioski wynikają z przeprowadzonego eksperymentu.

Argument:

> „AI tak wygenerowało”

nie stanowi uzasadnienia rozwiązania.

Wszystko jest dla ludzi, ale z rozwagą. :)

---

## 5. Zakres materiału (ćwiczenia)

### 1. Principal Component Analysis
- problem wysokiej wymiarowości,
- redukcja wymiarowości,
- centrowanie danych,
- macierz kowariancji,
- wartości własne,
- wektory własne,
- główne składowe,
- implementacja PCA od podstaw,
- wpływ liczby głównych składowych na reprezentację danych.

### 2. Support Vector Machines
- klasyfikator liniowy,
- hiperpłaszczyzna separująca,
- margines,
- wektory wspierające,
- przypadek danych liniowo nierozdzielnych,
- funkcje jądra,
- kernel trick,
- wpływ parametrów na granicę decyzyjną.

### 3. Reguła Hebba
- podstawowa idea uczenia hebbowskiego,
- zależność pomiędzy aktywnością elementów a zmianą wag,
- zapis reguły uczenia,
- implementacja prostego przykładu,
- wpływ próbek uczących na wartości wag,
- ograniczenia klasycznej reguły Hebba.

W tym bloku nacisk zostanie położony przede wszystkim na **samodzielne prześledzenie mechanizmu aktualizacji wag**, a nie korzystanie z gotowego modelu.

### 4. Sieć Hopfielda
- idea pamięci asocjacyjnej,
- architektura sieci Hopfielda,
- reprezentacja wzorców,
- wyznaczanie wag,
- wykorzystanie reguły Hebba do zapamiętywania wzorców,
- aktualizacja stanów neuronów,
- stany stabilne,
- odtwarzanie wzorca na podstawie danych niepełnych lub zaszumionych,
- pojemność i ograniczenia sieci,
- atraktory oraz możliwość występowania stanów niepożądanych.

Sieć Hopfielda będzie analizowana jako **klasyczny przykład pamięci asocjacyjnej**, a nie jako wprowadzenie do szerokiego zagadnienia współczesnych sieci neuronowych.

### 5. Drzewa decyzyjne
- budowa drzewa,
- podział przestrzeni cech,
- kryteria wyboru podziału,
- głębokość drzewa,
- wpływ parametrów na strukturę drzewa,
- interpretacja struktury modelu,
- zalety i ograniczenia drzew.

### 6. Metody zespołowe
- idea ensemble learning,
- łączenie wielu modeli,
- bagging,
- bootstrap,
- Random Forest,
- wpływ losowości na tworzenie zespołu modeli.

### 7. Boosting
- podstawowa idea boostingu,
- klasyfikatory słabe i silne,
- sekwencyjne tworzenie modeli,
- AdaBoost,
- zmiana znaczenia poszczególnych obserwacji podczas kolejnych etapów uczenia,
- budowanie modelu zespołowego.

### 8. K-Means
- uczenie bez nadzoru,
- grupowanie danych,
- centroidy,
- przypisywanie obserwacji do klastrów,
- aktualizacja centroidów,
- warunek zakończenia algorytmu,
- inicjalizacja centroidów,
- wpływ inicjalizacji na wynik,
- ograniczenia K-Means.

### 9. Fuzzy C-Means
- podstawy logiki rozmytej,
- zbiory rozmyte,
- stopień przynależności,
- rozmyte przypisanie obserwacji do klastrów,
- wyznaczanie centroidów,
- parametr rozmycia,
- porównanie K-Means i Fuzzy C-Means.

### 10. Porównywanie algorytmów
- różnice w sposobie działania poszczególnych metod,
- wpływ struktury danych na zachowanie algorytmu,
- wpływ parametrów na uzyskane rozwiązanie,
- wymagania obliczeniowe,
- interpretowalność rozwiązania,
- typowe zastosowania,
- ograniczenia poszczególnych metod.

## 6. Zakres nieobjęty ćwiczeniami laboratoryjnymi

W ramach ćwiczeń laboratoryjnych nie będą szczegółowo realizowane zagadnienia należące do innych przedmiotów, w szczególności:

- współczesne sztuczne sieci neuronowe,
- sieci wielowarstwowe,
- backpropagation,
- CNN,
- RNN,
- LSTM,
- architektury głębokiego uczenia,
- szczegółowe zagadnienia trenowania sieci neuronowych,
- accuracy, precision, recall i F1-score,
- ROC/AUC,
- szczegółowa analiza macierzy pomyłek,
- metryki regresji,
- walidacja krzyżowa,
- szczegółowe procedury ewaluacji jakości modeli,
- dobór modeli oparty na procedurach walidacyjnych.

**Wyjątek stanowią reguła Hebba oraz sieć Hopfielda**, które zostaną zrealizowane jako klasyczne algorytmy wskazane w zakresie przedmiotu przez osobę odpowiedzialną za jego realizację.

Formalny sylabus zawiera szerszy zakres dotyczący m.in. ewaluacji i walidacji modeli, natomiast w ramach laboratoriów treści zostały rozdzielone pomiędzy poszczególne przedmioty.

## 7. Harmonogram zajęć

Przedmiot obejmuje **30 godzin ćwiczeń laboratoryjnych**, czyli 15 spotkań po 2 godziny.

### 1. Zajęcia organizacyjne + PCA
- zasady zajęć,
- organizacja pracy,
- podstawowe pojęcia,
- matematyczne podstawy PCA,
- rozpoczęcie implementacji.

### 2. PCA
- implementacja algorytmu,
- wartości i wektory własne,
- redukcja wymiarowości,
- eksperymenty na danych.

### 3. Support Vector Machines
- hiperpłaszczyzna,
- margines,
- wektory wspierające,
- klasyfikacja liniowa.

### 4. Support Vector Machines
- dane nieliniowe,
- funkcje jądra,
- kernel trick,
- wpływ parametrów na działanie SVM.

### 5. Reguła Hebba
- idea uczenia hebbowskiego,
- zapis matematyczny,
- aktualizacja wag,
- samodzielna implementacja prostego przykładu.

### 6. Sieć Hopfielda
- pamięć asocjacyjna,
- tworzenie macierzy wag,
- zapamiętywanie wzorców,
- odtwarzanie wzorców zaszumionych,
- stany stabilne i ograniczenia sieci.

### 7. Drzewa decyzyjne
- konstrukcja drzewa,
- kryteria podziału,
- struktura drzewa,
- wpływ parametrów.

### 8. Bagging
- idea metod zespołowych,
- bootstrap,
- tworzenie zespołu modeli,
- porównanie z pojedynczym modelem.

### 9. Random Forest
- losowanie próbek,
- losowanie cech,
- budowa lasu,
- wpływ parametrów algorytmu.

### 10. Boosting / AdaBoost
- klasyfikatory słabe,
- sekwencyjne budowanie modeli,
- zmiana wag obserwacji,
- działanie AdaBoost.

### 11. K-Means
- centroidy,
- przypisywanie danych,
- aktualizacja centroidów,
- kolejne iteracje algorytmu.
- inicjalizacja centroidów,
- różne wartości K,
- wpływ danych i inicjalizacji na rezultat,
- ograniczenia algorytmu.

### 12. Fuzzy C-Means
- podstawy logiki rozmytej,
- stopnie przynależności,
- rozmyte grupowanie,
- porównanie z K-Means.

### 13. Praca nad projektami
- konsultacje,
- implementacja,
- eksperymenty,
- analiza działania zastosowanych algorytmów.

### 14 - 15. Prezentacja i obrona projektów
- prezentacja rozwiązania,
- pytania dotyczące działania algorytmów,
- obrona projektu,
- zaliczenie ćwiczeń laboratoryjnych.

Harmonogram może ulec zmianie w zależności od tempa realizacji materiału.

---

## 8. Warunki zaliczenia przedmiotu

Zgodnie z sylabusem formą weryfikacji ćwiczeń laboratoryjnych jest **projekt programistyczny dotyczący zagadnień poruszanych na ćwiczeniach i wykładzie**. 

Projekt wykonywany jest **indywidualnie**.

Projekt powinien przedstawiać rozwiązanie wybranego problemu z wykorzystaniem metod uczenia maszynowego omawianych podczas zajęć.

Oceniane będą przede wszystkim:

- poprawność przygotowania rozwiązania,
- znajomość zastosowanych algorytmów,
- prawidłowe wykorzystanie wybranych metod,
- dobór algorytmów odpowiednich do problemu,
- uzasadnienie wyboru algorytmów,
- przeprowadzenie eksperymentów,
- analiza wpływu parametrów na działanie algorytmów,
- porównanie zachowania różnych metod,
- jakość kodu programistycznego,
- czytelność rozwiązania,
- sens przeprowadzonych eksperymentów,
- jakość i samodzielność wniosków.

**Projekt oddany po wyznaczonym terminie nie zostanie sprawdzony. W wyjątkowych przypadkach (usprawiedliwionych) istnieje możliwość indywidualnego przedłużenia terminu.** 

---

## 9. Punktacja i zakres projektu

### 9.1. Charakter projektu

Podstawą zaliczenia laboratoriów jest **indywidualny projekt programistyczny stanowiący portfolio implementacji i eksperymentów dotyczących algorytmów uczenia maszynowego omawianych podczas zajęć**.

Celem projektu jest pokazanie, że student:

- rozumie zasadę działania omawianych algorytmów,
- potrafi zaimplementować wybrane algorytmy samodzielnie,
- potrafi korzystać z istniejących implementacji bibliotecznych,
- potrafi porównać własną implementację z gotowym rozwiązaniem,
- rozumie znaczenie parametrów i hiperparametrów algorytmu,
- potrafi przeprowadzić eksperyment i zinterpretować jego wynik,
- potrafi wskazać ograniczenia zastosowanych metod,
- potrafi dobrać metodę do określonego problemu i uzasadnić swój wybór.

Projekt wykonywany jest **indywidualnie**.

Projekt obejmuje wszystkie główne algorytmy realizowane podczas laboratoriów:

1. PCA,
2. liniowy SVM,
3. regułę Hebba,
4. sieć Hopfielda,
5. drzewo decyzyjne,
6. Bagging,
7. Random Forest,
8. AdaBoost,
9. K-Means,
10. Fuzzy C-Means.

Nie wszystkie algorytmy muszą zostać zaimplementowane samodzielnie. Szczegółowy zakres opisano poniżej.

---

### 9.2. Własne implementacje

Student przygotowuje **8 własnych implementacji algorytmów**.

#### Implementacje obowiązkowe

Każdy student musi samodzielnie zaimplementować:

1. **PCA**,
2. **regułę Hebba**,
3. **sieć Hopfielda**,
4. **drzewo decyzyjne**,
5. **Bagging**,
6. **K-Means**.

#### Implementacje do wyboru

Dodatkowo student wybiera **2 z 4** następujących algorytmów:

- liniowy SVM,
- Random Forest,
- AdaBoost,
- Fuzzy C-Means.

Przy czym **co najmniej jedna z dwóch wybranych implementacji musi należeć do metod zespołowych**, czyli musi to być:

- Random Forest

lub

- AdaBoost.

Przykładowe poprawne zestawy:

```text
SVM + Random Forest
SVM + AdaBoost
Random Forest + AdaBoost
Random Forest + Fuzzy C-Means
AdaBoost + Fuzzy C-Means
```

Nie spełnia tego wymagania zestaw:

```text
SVM + Fuzzy C-Means
```

ponieważ nie zawiera rozszerzonej metody zespołowej.

Łącznie student przygotowuje więc:

```text
6 implementacji obowiązkowych
+
2 implementacje do wyboru
=
8 własnych implementacji
```

Pozostałe **2 algorytmy również muszą znaleźć się w projekcie**, ale nie wymagają własnej implementacji. Dla nich obowiązuje wykorzystanie odpowiedniej implementacji bibliotecznej, przeprowadzenie eksperymentu oraz przygotowanie wniosków.

---

### 9.3. Wymagania dotyczące własnych implementacji

Własne implementacje powinny być wydzielone jako osobne moduły lub logicznie odseparowane części projektu.

Przykładowa struktura:

```text
project/
│
├── implementations/
│   ├── myPCA.py
│   ├── myHebb.py
│   ├── myHopfield.py
│   ├── myDecisionTree.py
│   ├── myBagging.py
│   ├── myKMeans.py
│   ├── wybrany_algorytm_1.py
│   └── wybrany_algorytm_2.py
│
├── experiments/
│   ├── PCA.ipynb
│   ├── SVM.ipynb
│   ├── Hebb.ipynb
│   ├── Hopfield.ipynb
│   ├── DecisionTree.ipynb
│   ├── Bagging.ipynb
│   ├── RandomForest.ipynb
│   ├── AdaBoost.ipynb
│   ├── KMeans.ipynb
│   └── FuzzyCMeans.ipynb
│
└── README.md
```

Dopuszczalna jest inna organizacja projektu, jeżeli pozostaje czytelna i jednoznacznie rozdziela własne implementacje od kodu eksperymentalnego.

Własna implementacja **nie może wykorzystywać wewnętrznie gotowej implementacji tego samego algorytmu**.

Przykładowo własny:

```python
MyDecisionTreeClassifier
```

nie może realizować działania poprzez:

```python
DecisionTreeClassifier(...)
```

a własny:

```python
MyLinearSVM
```

nie może wykorzystywać:

```python
SVC(...)
```

jako właściwego mechanizmu uczenia.

Analogicznie własny `MyKMeans` nie może wewnętrznie korzystać z `sklearn.cluster.KMeans`, a własny `MyAdaBoostClassifier` z `sklearn.ensemble.AdaBoostClassifier`.

Nie jest wymagane odtworzenie wszystkich możliwości profesjonalnych bibliotek.

Własna implementacja może być świadomie uproszczona, pod warunkiem że student potrafi:

- wskazać zastosowane uproszczenia,
- wyjaśnić ich konsekwencje,
- wskazać funkcjonalności dostępne w profesjonalnej bibliotece, których nie posiada własne rozwiązanie.

---

### 9.4. Implementacje biblioteczne

**Wszystkie 10 algorytmów** powinno zostać wykorzystanych w części eksperymentalnej projektu.

Dla 8 algorytmów posiadających własną implementację należy przeprowadzić porównanie:

```text
własna implementacja
vs.
implementacja biblioteczna
```

Przykładowo:

```text
MyPCA
vs.
sklearn.decomposition.PCA

MyLinearSVM
vs.
sklearn.svm.SVC

MyDecisionTreeClassifier
vs.
sklearn.tree.DecisionTreeClassifier

MyBaggingClassifier
vs.
sklearn.ensemble.BaggingClassifier

MyRandomForestClassifier
vs.
sklearn.ensemble.RandomForestClassifier

MyAdaBoostClassifier
vs.
sklearn.ensemble.AdaBoostClassifier

MyKMeans
vs.
sklearn.cluster.KMeans

MyFuzzyCMeans
vs.
skfuzzy.cluster.cmeans
```

Dla algorytmów, których student **nie wybrał do własnej implementacji**, należy:

1. użyć odpowiedniej gotowej implementacji,
2. przeprowadzić przynajmniej jeden eksperyment,
3. wyjaśnić zasadę działania algorytmu,
4. przeanalizować wpływ wybranego parametru,
5. wskazać najważniejsze ograniczenia,
6. sformułować własne wnioski.

Oznacza to, że w projekcie powinny znaleźć się wszystkie algorytmy z przedmiotu, ale tylko 8 z nich wymaga własnej implementacji.

---

### 9.5. Porównanie własnej implementacji z biblioteką

Porównanie powinno być wykonane na **tych samych danych wejściowych** oraz, na ile jest to możliwe, przy odpowiadającej sobie konfiguracji obu metod.

Celem porównania nie jest wykazanie, że własna implementacja jest szybsza lub lepsza od profesjonalnej biblioteki.

Student powinien przede wszystkim odpowiedzieć na pytania:

- Czy obie implementacje realizują tę samą ideę algorytmu?
- Czy dla tych samych danych zachowują się podobnie?
- Jakie różnice można zaobserwować?
- Z czego mogą wynikać te różnice?
- Jakie uproszczenia posiada własna implementacja?
- Jakie dodatkowe możliwości oferuje gotowa biblioteka?
- Czy różnice wynikają z samego algorytmu, czy ze szczegółów implementacji?

Nie jest wymagane uzyskanie identycznych wyników.

Przykładowo różne implementacje mogą:

- inaczej inicjalizować model,
- inaczej rozstrzygać remisy,
- korzystać z innych warunków stopu,
- stosować dodatkowe optymalizacje,
- implementować bardziej rozbudowaną wersję algorytmu.

Student powinien umieć takie różnice zauważyć i wyjaśnić.

---

### 9.6. Eksperymenty

Projekt nie może ograniczać się wyłącznie do jednorazowego uruchomienia algorytmu.

Dla **każdego z 10 algorytmów** należy przygotować **co najmniej jeden eksperyment pokazujący wpływ wybranego parametru, hiperparametru lub właściwości algorytmu na jego zachowanie**.

Przykładowo:

| Algorytm | Przykładowe eksperymenty |
|---|---|
| PCA | liczba składowych, udział zachowanej zmienności, rekonstrukcja danych |
| SVM | parametr `C`, learning rate, liczba iteracji, kształt granicy decyzyjnej |
| Reguła Hebba | learning rate, liczba epok, skala cech |
| Sieć Hopfielda | poziom szumu, liczba zapamiętywanych wzorców, sposób aktualizacji neuronów |
| Drzewo decyzyjne | `max_depth`, `min_samples_split`, kryterium podziału |
| Bagging | `n_estimators`, `max_samples`, bootstrap |
| Random Forest | `n_estimators`, `max_features`, głębokość drzew |
| AdaBoost | `n_estimators`, `learning_rate`, zmiany wag obserwacji |
| K-Means | liczba klastrów, inicjalizacja centroidów, skala cech |
| Fuzzy C-Means | liczba klastrów, parametr `m`, FPC, stopień rozmycia |

W miarę możliwości student powinien **przed wykonaniem eksperymentu określić spodziewany efekt zmiany danego parametru**, a następnie porównać przewidywanie z otrzymanym wynikiem.

Oceniana jest przede wszystkim:

- interpretacja zachowania algorytmu,
- poprawność wnioskowania,
- znajomość wpływu parametrów,
- umiejętność wskazania ograniczeń.

Samo wygenerowanie wykresu lub tabeli nie jest wystarczające.

---

### 9.7. Część syntetyczna projektu

Projekt powinien zawierać również część łączącą wiedzę z całego semestru.

Student wybiera jeden problem lub zbiór danych i wskazuje **co najmniej dwie poznane podczas zajęć metody**, które można sensownie zastosować do jego analizy.

Należy uzasadnić:

- dlaczego wybrane metody pasują do danego problemu,
- czego oczekuje się po każdej z nich,
- czym różni się sposób ich działania,
- jakie są ich najważniejsze ograniczenia,
- dlaczego inne poznane podczas zajęć metody mogą być w danym przypadku mniej odpowiednie.

Nie jest wymagane wskazanie jednego „najlepszego” algorytmu.

Oceniana jest przede wszystkim **poprawność argumentacji i zrozumienie właściwości poszczególnych metod**.

---

### 9.8. Wnioski

Każda część projektu powinna zakończyć się krótkimi wnioskami.

Wnioski nie powinny ograniczać się do stwierdzeń:

```text
program działa,
biblioteka zwróciła podobny wynik,
parametr zmienił wykres.
```

Student powinien odnieść się między innymi do:

- zachowania własnej implementacji,
- zgodności lub różnic względem implementacji bibliotecznej,
- wpływu parametrów na działanie algorytmu,
- ograniczeń własnego rozwiązania,
- ograniczeń samego algorytmu,
- przypadków, w których zastosowanie danej metody jest uzasadnione,
- przypadków, w których dana metoda może działać niewłaściwie lub być niewystarczająca.

Dla dwóch algorytmów, które nie zostały zaimplementowane samodzielnie, wnioski powinny dotyczyć:

- działania wersji bibliotecznej,
- wpływu parametrów,
- zachowania algorytmu podczas eksperymentu,
- najważniejszych ograniczeń.

Wnioski powinny być wynikiem przeprowadzonych eksperymentów i własnej analizy.

---

### 9.9. Punktacja projektu

Za projekt można uzyskać maksymalnie **70 punktów**.

| Element | Punkty |
|---|---:|
| Poprawność i kompletność 8 własnych implementacji | 25 pkt |
| Wykorzystanie bibliotek i porównanie implementacji | 15 pkt |
| Eksperymenty dla wszystkich 10 algorytmów | 10 pkt |
| Dobór metod do problemu i uzasadnienie wyboru | 10 pkt |
| Jakość kodu, dokumentacja, wnioski i krytyczna analiza | 10 pkt |
| **Razem** | **70 pkt** |

#### Poprawność i kompletność własnych implementacji — 25 pkt

Oceniane są:

- kompletność 6 implementacji obowiązkowych,
- kompletność 2 poprawnie wybranych implementacji dodatkowych,
- obecność co najmniej jednej własnej implementacji `Random Forest` lub `AdaBoost`,
- poprawność działania,
- zgodność implementacji z omawianym algorytmem,
- samodzielna realizacja właściwej logiki algorytmu,
- czytelność rozwiązania,
- obsługa podstawowych przypadków brzegowych,
- umiejętność wskazania zastosowanych uproszczeń.

Brak wymaganej implementacji powoduje utratę punktów w tej kategorii.

Nie jest wymagane odtworzenie pełnej funkcjonalności profesjonalnych bibliotek.

#### Wykorzystanie bibliotek i porównanie implementacji — 15 pkt

Oceniane są:

- obecność wszystkich 10 algorytmów w projekcie,
- poprawne wykorzystanie implementacji bibliotecznych,
- porównanie 8 własnych implementacji z bibliotekami,
- wykorzystanie wersji bibliotecznych dla 2 algorytmów niewybranych do implementacji,
- porównanie obu implementacji na tych samych danych,
- odpowiednia konfiguracja porównywanych metod,
- wskazanie podobieństw i różnic,
- wyjaśnienie możliwych przyczyn różnic,
- wskazanie możliwości obecnych w bibliotece, których nie posiada własna implementacja.

#### Eksperymenty — 10 pkt

Oceniane są:

- wykonanie eksperymentu dla każdego z 10 algorytmów,
- sensowny dobór badanych parametrów,
- przewidywanie wpływu zmian parametrów,
- interpretacja otrzymanych wyników,
- wyciągnięcie własnych wniosków.

#### Dobór metod — 10 pkt

Oceniane są:

- dopasowanie metod do wybranego problemu,
- poprawne uzasadnienie wyboru,
- rozumienie różnic pomiędzy algorytmami,
- rozumienie ograniczeń zastosowanych metod,
- umiejętność wskazania metod mniej odpowiednich dla danego problemu.

#### Kod, dokumentacja i wnioski — 10 pkt

Oceniane są:

- czytelność kodu,
- logiczna organizacja projektu,
- nazewnictwo,
- dokumentacja,
- możliwość uruchomienia projektu,
- jakość własnych wniosków,
- krytyczna analiza rezultatów.

---

### 9.10. Obrona projektu

Za obronę projektu można uzyskać maksymalnie **30 punktów**.

Obrona trwa około **10–15 minut**.

Student powinien być przygotowany na pytania dotyczące **dowolnego z 10 algorytmów znajdujących się w projekcie**, niezależnie od tego, czy został on zaimplementowany samodzielnie.

W przypadku algorytmów posiadających własną implementację student powinien być przygotowany na:

- wyjaśnienie działania własnego rozwiązania,
- omówienie wskazanego fragmentu kodu,
- wyjaśnienie matematycznej lub algorytmicznej podstawy metody,
- wskazanie miejsca realizującego kluczowy element algorytmu,
- wyjaśnienie znaczenia parametrów,
- porównanie własnej implementacji z wersją biblioteczną,
- wskazanie zastosowanych uproszczeń,
- wykonanie niewielkiej modyfikacji kodu.

W przypadku dwóch algorytmów niewybranych do własnej implementacji student powinien być przygotowany na:

- wyjaśnienie sposobu działania algorytmu,
- wyjaśnienie znaczenia najważniejszych parametrów,
- omówienie przeprowadzonego eksperymentu,
- interpretację uzyskanych wyników,
- wskazanie ograniczeń algorytmu,
- wyjaśnienie działania wykorzystanej implementacji bibliotecznej na poziomie jej interfejsu i parametrów.

Przykładowe pytania podczas obrony:

```text
Co stanie się po zmniejszeniu liczby komponentów PCA?

Co zmieni zwiększenie C w SVM?

Dlaczego reguła Hebba nie rozwiązuje problemu XOR?

Co może się stać w sieci Hopfielda po zapisaniu większej liczby podobnych wzorców?

Co zmieni max_depth=1 w drzewie decyzyjnym?

W którym miejscu własnego drzewa wybierany jest najlepszy podział?

Na czym polega bootstrap w Baggingu?

Czym Random Forest różni się od zwykłego Baggingu drzew?

Dlaczego w Random Forest losujemy cechy przy każdym węźle?

Dlaczego AdaBoost zwiększa wagi błędnie sklasyfikowanych obserwacji?

Co zmieni zwiększenie liczby klastrów w K-Means?

Dlaczego skala cech ma znaczenie w K-Means?

Co oznacza parametr m w Fuzzy C-Means?

Czym różni się przynależność do klastra w K-Means i Fuzzy C-Means?

Dlaczego wynik własnej implementacji różni się od wyniku biblioteki?

Jakiego zachowania oczekujesz po zmianie wskazanego parametru i dlaczego?
```

Samo posiadanie działającego programu nie jest wystarczające do zaliczenia.

Student musi rozumieć:

- napisany przez siebie kod,
- działanie wszystkich 10 algorytmów objętych projektem,
- znaczenie ich najważniejszych parametrów,
- sposób przeprowadzenia eksperymentów,
- wykorzystane implementacje biblioteczne,
- przedstawione wnioski.

Brak możliwości wyjaśnienia własnej implementacji może skutkować niezaliczeniem obrony niezależnie od liczby punktów uzyskanych za przesłany kod.

Student może również otrzymać pytanie dotyczące algorytmu, którego **nie implementował samodzielnie**, ponieważ wszystkie 10 algorytmów należy do zakresu projektu i przedmiotu.

---

### 9.11. Warunek zaliczenia

Łącznie można uzyskać:

```text
Projekt: 70 pkt
Obrona:  30 pkt
----------------
Razem:  100 pkt
```

Do zaliczenia laboratoriów wymagane jest:

- uzyskanie co najmniej **51 punktów na 100 możliwych**,
- uzyskanie pozytywnego wyniku z obrony projektu,
- oddanie projektu w terminie określonym w harmonogramie zajęć.

Projekt należy oddać w formie umożliwiającej jego uruchomienie i sprawdzenie.

Student odpowiada za poprawność, kompletność oraz znajomość całego kodu znajdującego się w oddanym projekcie.

Wymagany zakres projektu można podsumować następująco:

```text
10 algorytmów w projekcie
│
├── 8 własnych implementacji
│   │
│   ├── 6 obowiązkowych:
│   │   ├── PCA
│   │   ├── Hebb
│   │   ├── Hopfield
│   │   ├── Decision Tree
│   │   ├── Bagging
│   │   └── K-Means
│   │
│   └── 2 z 4:
│       ├── SVM
│       ├── Random Forest
│       ├── AdaBoost
│       └── Fuzzy C-Means
│
│       przy czym co najmniej jedno z:
│       Random Forest / AdaBoost
│
└── pozostałe 2 algorytmy:
    ├── implementacja biblioteczna
    ├── eksperyment
    ├── analiza
    └── wnioski
```

---

## 10. Obecność i praca na zajęciach

Na zajęciach sprawdzana będzie obecność.

Ćwiczenia mają charakter praktyczny i znaczna część materiału będzie realizowana bezpośrednio podczas zajęć, dlatego regularny udział jest istotnym elementem realizacji przedmiotu.

Zadania wskazane przez prowadzącego jako obowiązkowe powinny zostać wykonane w wyznaczonym terminie.

Szczegółowe zasady dotyczące dopuszczalnej liczby nieobecności oraz ich usprawiedliwiania wynikają z obowiązujących zasad organizacji studiów na UWM.

## 11. Terminarz (może ulec zmianie)

* 05.10.2026r. - Zajęcia organizacyjne + PCA
* 12.10.2026r. - PCA
* 19.10.2026r. - Support Vector Machines
* 26.10.2026r. - Support Vector Machines
* 02.11.2026r. - **DZIEŃ REKTORSKI**
* 09.11.2026r. - Reguła Hebba
* 16.11.2026r. - Sieć Hopfielda
* 23.11.2026r. - Drzewa decyzyjne
* 30.11.2026r. - Bagging
* 07.12.2026r. - Random Forest
* 14.12.2026r. - Boosting / AdaBoost
* 21.12.2026r. - K-Means
* **PRZERWA ŚWIĄTECZNA**
* 07.01.2027r. (**CZWARTEK**) - Fuzzy C-Means
* 11.01.2027r. - Praca nad projektami
    * OSTATECZNY TERMIN PRZESYŁANIA PROJEKTÓW DO KOŃCA TEGO DNIA (11.01.2027r., godz. 23:59)
* 18.01.2027r. - Prezentacja i obrona projektów
* 25.01.2027r. - Prezentacja i obrona projektów

## 12. Obrony projektów

Obrony projektów będą miały charakter publiczny, to znaczy każdy broni się na zajęciach przed resztą swojej grupy. 

Szanując Państwa czas, obrony będą podzielone na dwa dni (dwa ostatnie zajęcia), na które na każdy z nich będą wystawione zapisy (prawdopdobnie przez formularz w Excelu wystawiony na MSTeams). W dniach obron, jeżeli osoba studiująca nie jest zapisana na dany dzień, nie musi się wyjątkowo pojawić na zajęciach (jednak zachęcam :) ). 

Na każdą osobą studiującą przypada około 10-15 minut na obronę. Na zapisach na dany termin obowiązuje zasada "kto pierwszy, ten lepszy".

## 13. Oceny a punktacja

* 2.0 -> od 0  do 50 pkt
* 3.0 -> od 51 do 60 pkt
* 3.5 -> od 61 do 70 pkt
* 4.0 -> od 71 do 80 pkt
* 4.5 -> od 81 do 90 pkt
* 5.0 -> od 91 do 100 pkt

---

> # WAŻNA INFORMACJA
>
> **Celem zajęć nie jest wyłącznie uzyskanie działającego programu.**
>
> Osoba studiująca powinna przede wszystkim rozumieć zastosowane algorytmy, potrafić wyjaśnić ich sposób działania, wskazać znaczenie najważniejszych parametrów oraz krytycznie przeanalizować zachowanie zastosowanej metody.
>
> W przypadku zadań oznaczonych jako **samodzielna implementacja algorytmu** wykorzystanie kodu wygenerowanego przez AI jako własnej implementacji jest niedopuszczalne.
>
> W pozostałych przypadkach narzędzia AI mogą być wykorzystywane jako narzędzie wspomagające, ale osoba studiująca ponosi pełną odpowiedzialność za wykorzystane rozwiązanie i musi potrafić je wyjaśnić jak i samodzielnie zmodyfikować.

## Konsultacje
* Sala: E1/20 (bądź inna ustalona wcześniej)
* Terminy:
    * Wt.: 11:30 - 13:00
    * Śr.: 16:00 - 18:00

## Kontakt

**mgr inż. Adrian Albrecht** ([adrian.albrecht@uwm.edu.pl](mailto:adrian.albrecht@uwm.edu.pl)) </br>
Katedra Metod Matematycznych Informatyki  
Wydział Matematyki i Informatyki  
Uniwersytet Warmińsko-Mazurski w Olsztynie
