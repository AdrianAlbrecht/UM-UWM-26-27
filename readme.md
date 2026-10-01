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

### Projekt – 70 pkt

- **Opis problemu i zbioru danych – 5 pkt**
- **Przygotowanie danych – 5 pkt**
- **Dobór algorytmów i uzasadnienie wyboru – 10 pkt**
- **Poprawne wykorzystanie / implementacja algorytmów – 20 pkt**
- **Eksperymenty z parametrami i konfiguracją algorytmów – 10 pkt**
- **Porównanie działania zastosowanych metod – 10 pkt**
- **Wnioski i krytyczna analiza rezultatów – 10 pkt**

### Obrona projektu – 30 pkt

- znajomość własnego projektu – **obligatoryjny warunek zaliczenia**,
- znajomość działania wykorzystanych algorytmów,
- umiejętność wyjaśnienia własnego kodu,
- umiejętność uzasadnienia zastosowanych rozwiązań,
- odpowiedzi na pytania dotyczące projektu.

Przykładowe pytania:

- Dlaczego zastosowano właśnie ten algorytm?
- Jak działa ten algorytm?
- Co oznacza wskazany parametr?
- Co stanie się po zwiększeniu jego wartości?
- Dlaczego w tym miejscu wykonywana jest taka operacja?
- Jak zmieniłby się rezultat przy innej inicjalizacji?
- Dlaczego dwa algorytmy zachowują się inaczej dla tych samych danych?
- Jakie są ograniczenia wykorzystanej metody?
- Co dokładnie robi wskazany fragment kodu?

**Do zaliczenia ćwiczeń laboratoryjnych wymagane jest minimum 51 pkt oraz pozytywna obrona projektu.**

Samo uzyskanie odpowiedniej liczby punktów za kod nie wystarcza, jeżeli osoba studiująca nie potrafi wyjaśnić działania własnego rozwiązania.

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

## Kontakt

**mgr inż. Adrian Albrecht** ([adrian.albrecht@uwm.edu.pl](mailto:adrian.albrecht@uwm.edu.pl)) </br>
Katedra Metod Matematycznych Informatyki  
Wydział Matematyki i Informatyki  
Uniwersytet Warmińsko-Mazurski w Olsztynie
