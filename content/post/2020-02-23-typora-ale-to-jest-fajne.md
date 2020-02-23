---
title: Typora, ależ to jest fajne!
author: sms
date: '2020-02-23'
slug: typora-ale-to-jest-fajne
categories:
  - Technologie
tags: []
description: ''
topics: []

---

Od zawsze moim marzeniem był edytor typu pustka kartka. Bez elementów, które odrywają uwagę i nadmiaru funkcji. Czysty ekran. No i w końcu znalazłem [Typora](https://typora.io). Pod wieloma względami dla mnie ideał.

![Typora Lorem Ipsum](/post/2020-02-23-typora-ale-to-jest-fajne_files/typora_lorem_ipsum.png)

Zacznijmy od tego do czego potrzebny mi jest w gruncie rzeczy specjalizowany edytor? Otóż spora część mojej pracy, to dokumenty w których jest zarówno tekst i grafika, ale również kod programu. Ten ostatni może być w dwóch przypadkach: jako ilustracja czegoś o czym piszę oraz jako po prostu kod, często niewidoczny dla użytkownika, który tworzy np. wykres z aktualnymi danymi. 

Piszę też "normalne" dokumenty i do tego celu, Typora pasuje mi wyśmienicie. Mogę tworzyć w niej dokument, a następnie zamienić go na format pdf, html czy po prostu docx - Worda.

W Typora są trzy elementy, które mnie do niej(iego?) przekonały:

- [Markdown](https://daringfireball.net/projects/markdown/) jako podstawowy sposób zapisywania dokumentów
- Minimalny interfejs, ale bogate funkcje konfiguracyjne
- Przemyślana koncepcja

Pewnie wielu czytających słowo "Markdown" powie: "yyyyy, WTF? ". Dlatego spieszę z wyjaśnieniem, bo to ważne. Markdown to taki bardzo uproszczony język znaczników, które są w odpowiedni sposób interpretowane. Zawiera kilkanaście różnych znaczników, umożliwiających wykonanie najczęściej stosowanych w edycji czynności. Na przykład styl H1 tytułu, punktatory, właściwości czcionki jak wytłuszczenie, kursywa, wstawianie obrazu etc.  Jest to tak proste, że Markdown można nauczyć 6-latka, który umie pisać i czytać.

No chyba nie rozjaśniłem, więc posłużę się przykładem: W markdown, jeśli chcesz wytłuścić wyraz np. "edytor" to używasz znacznika wytłuszczenia, którym są dwa znaki mnożenia "**" z obydwu stron wyrazu. Wygląda to tak:

```markdown
**edytor**
```

A efekt tak:

**edytor**

Co w tym jest fajnego?! Przecież łatwiej i szybciej jest jak w Wordzie kliknąć kombinację klawiszy CTRL+B? Pisząc zwykłe teksty, nazwijmy je biurowe, być może tak, ale gdy chcemy coś z tymi tekstami później zrobić, a szczególnie przetwarzać je posługując się napisanym programem, to już niezupełnie. Markdown to zwykły plik tekstowy, który można utworzyć czy edytować na każdym urządzeniu i w każdym systemie operacyjnym. Ta cecha sprawia, że przy pomocy różnych narzędzi np. [Pandoc](https://pandoc.org/) możemy dowolny plik Markdown zamienić na dowolny inny np. Word, PDF etc. bez utraty najważniejszych atrybutów tekstu. Jeszcze lepiej wygląda to w pracach naukowych. Czasopisma naukowe bardzo często żądają plików w LaTex, Markdown albo formatach zwykłych edytorów tekstów.  Mając tekst napisany w Markdown bez problemu zamienimy go (np. Pandoc-iem) na dowolny inny. To pestka.

Pandoc to program, który nie ma interfejsu i polecenia wprowadzamy w terminalu. Na przykład jeśli chciałbym zamienić dokument w formacie Markdown (md) na PDF to piszę w terminalu:

```
pandoc -s -o doc.pdf doc.md
```

i po chwili mam gotowego pdfa. Pisanie poleceń by zamienić plik z jednego formatu na drugi i gdy mamy do czynienia z jednym dokumentem, wydaje się uciążliwa. Dlatego tak naprawdę możliwość taką docenią ci, którzy np. chcą zamienić w ten sposób cały folder dokumentów, albo są programistami i wykorzystują takie funkcje w swoich programach. 

Wróćmy jednak do Typora, bo wstawianie znaczników Markdown, nawet jeśli proste, to jednak np. w Notatniku Windows może być żmudne. No i tu niezastąpione są edytory Markdown, które łączą w sobie wygodę "normalnych" edytorów, z funkcjami (i ograniczeniami) Markdown. 

Zacznijmy od wspomnianej wygody. W Typorze mogę, ale nie muszę używać tagów Markdown. Na przykład by wytłuścić wyraz czy fragment tekstu mogę po prostu zaznaczyć wyraz i nacisnąć klawisze <CTRL>+B, a edytor automatycznie zamieni ten fragment na odpowiedni tag Markdown. Oznacza to, że mogę pisać mniej więcej tak jak w normalnym edytorze i mieć wynik w formacie Markdown.

Druga rzecz: tryb pisania. Mam do wyboru trzy tryby: 

- zwykły, w którym piszę normalnie tak jak w każdym edytorze tekstów,
- maszyny do pisania, w którym po każdej nowej linii, tekst podnosi się do góry (jak kartka w maszynie do pisania). Szkoda, że nie dodano charakterystycznego dla maszyny do pisania dźwięku uderzania w papier.
- skupienia - mój ulubiony - gdzie wyraźnie wyświetlana jest akapit w której aktualnie jest kursor, a pozostała część tekstu jest "wyszarzona".

![Typora - tryb skupienia](/post/2020-02-23-typora-ale-to-jest-fajne_files/typora_tryb_skupienia.png)

Trzecia rzecz: panel boczny w którym wyświetlane są nazwy plików w aktualnym folderze na zmianę z konspektem dokumentu. Bardzo przydatne.

![Typora - panel boczny](/post/2020-02-23-typora-ale-to-jest-fajne_files/typora_panel_boczny.png)

Czwarta, chociaż chyba powinna być pierwsza:-) : Podgląd na żywo wyglądu dokumentu. Dla osób korzystających z normalnego edytora tekstów, to żadne ajwaj, ale dla tworzących dokumenty w Markdown, to duże ułatwienie. Piszę sobie w miarę normalnie, widzę jak mój tekst wygląda po każdej zmianie i wiem, że dokument tworzony jest w Markdown.

Piąta, to... licznik (w dolnym po prawej rogu ekranu), który pokazuje m.in. ile minut trwało będzie przeczytanie tekstu.

Szósta i ostatnia z tych, co mnie się przydają, to niesamowite możliwości konfiguracji. Nie podoba mi się standardowy font, dwie linijki w css i mam ten, który chcę. Czytam wolniej/szybciej niż pokazuje licznik, o którym wspomniałem? Można zdefiniować indywidualną szybkość wyrażoną w słowach na minutę. Nie podoba mi się skórka programu? Mogę ją zmienić na jedną z 4 dostępnych, albo zrobić swoją własną, co jest naprawdę bardzo proste.

Typora  ma jeszcze dziesiątki funkcji o których nie wspominam, bo używam je rzadziej. Ma też jedną wadę, z której jednak usprawiedliwiam jej twórców: brak wyrównania akapitu do lewej, prawej czy centrowania. Może ktoś powiedzieć: no jak to, edytor tekstu nie ma wyrównania? Ano nie ma, bo nie takiej funkcji w standardzie Markdown. Tak naprawdę to piszący teksty rzadko ją używają, bo layout to domena DTP, a nie autorów. Jeśli jednak komuś tego akurat bardzo brakuje, to można np. centrowanie tekstu zrobić... wykorzystując zdefiniowaną w css klasę. Tu centrowanie.

```
<p style="text-align:center">
Jakiś tekst
</p>
```

Kompletnie zapomniałem o trzech elementach, z których dwa są naprawdę często używane, czyli wstawianiu zdjęć, wideo i... diagramów.

Pierwsze dwa, czyli zdjęcie i wideo wstawia się bajecznie łatwo, bo po prostu wystarczy w odpowiednie miejsce przenieść i upuścić plik zawierający zdjęcie czy wideo. Typora ma nawet w konfiguracji miejsce, gdzie możemy zdefiniować docelowy folder dla zdjęć umieszonych w tekście. Można też zarządzić by plik ze zdjęciem automatycznie został skopiowany do określonego folderu. Podobnie jest z plikami wideo. 

Jeśli chodzi o diagramy, to można je tworzyć bezpośrednio w edytorze. Nie są to kombajny z milionem funkcji, ale te najważniejsze można użyć.  Mnie się podoba.

Reasumująć: prosty, ale o w gruncie rzeczy dużych możliwościach. Konfigurowalny, raczej dla myślących i tych co wiedzą czego chcą. Czuję, że na dłużej u mnie zagości.


