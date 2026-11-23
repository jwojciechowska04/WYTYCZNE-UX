# 01. Dostępność

## Punkt odniesienia

Używaj **WCAG 2.2, poziom AA** jako domyślnego celu projektowego. WCAG to standard W3C z testowalnymi kryteriami sukcesu. Poziomy A, AA i AAA są narastające; osiągnięcie poziomu AA wymaga spełnienia kryteriów A i AA. Zgodność ocenia się dla kompletnych stron i całych procesów, nie tylko pojedynczego widoku.

Źródła: [WCAG 2.2 – standard W3C](https://www.w3.org/TR/WCAG22/), [How to Meet WCAG 2.2 – szybka lista kryteriów](https://www.w3.org/WAI/WCAG22/quickref/).

## Tekst, kolor i obrazy

- **WCAG 1.4.3 Kontrast (minimum), AA**: kontrast tekstu i obrazów tekstu wynosi co najmniej **4,5:1**. Dla dużego tekstu (co najmniej 18 pt zwykłego lub 14 pt pogrubionego) minimum wynosi **3:1**. Nie zaokrąglaj wyniku w górę: 4,499:1 nie spełnia 4,5:1.
- Nie przekazuj informacji wyłącznie kolorem. Dodaj tekst, kształt, wzór lub ikonę, zależnie od kontekstu (**1.4.1 Użycie koloru, A**).
- Zapewnij tekst alternatywny dla treściowych obrazów. Obrazy dekoracyjne pomijaj w drzewie dostępności (np. pusty `alt=""`); dla złożonych wykresów podaj równoważne dane/opis (**1.1.1 Treść nietekstowa, A**).
- Nie umieszczaj tekstu jako obrazu, jeśli tę samą prezentację można osiągnąć zwykłym tekstem (**1.4.5 Obrazy tekstu, AA**, z wyjątkami).

Źródła: [W3C: kontrast 1.4.3](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html), [WCAG Quick Reference](https://www.w3.org/WAI/WCAG22/quickref/).

## Klawiatura, fokus i ruch

- **WCAG 2.1.1 (A)**: każdą funkcję obsługuj klawiaturą, bez konieczności korzystania z określonego czasu pojedynczego naciśnięcia (poza wyjątkami, np. rysowaniem odręcznym).
- **WCAG 2.4.7 (AA)**: fokus klawiatury musi być widoczny. Nie usuwaj obrysu bez zapewnienia równie widocznego wskaźnika.
- **WCAG 2.4.11 (AA)**: element z fokusem nie może być całkowicie zasłonięty przez treść utworzoną przez autora strony (np. przyklejony pasek).
- Utrzymuj kolejność fokusu zgodną z kolejnością znaczenia i obsługi (**2.4.3, A**). Dla nawigacji do wielu obszarów zapewnij możliwość ich pominięcia (**2.4.1, A**).
- Nie uruchamiaj funkcji wyłącznie po najechaniu wskaźnikiem ani po samym otrzymaniu fokusu (**3.2.1, A**).

Źródła: [WCAG 2.2](https://www.w3.org/TR/WCAG22/), [W3C: Fokus niezasłonięty](https://www.w3.org/WAI/WCAG22/Understanding/focus-not-obscured-minimum.html).

## Cele kliknięcia i dotyku

- **WCAG 2.5.8 Cel (minimum), AA**: cel wskaźnika ma co najmniej **24 × 24 CSS px** albo spełnia wyjątek dotyczący odstępu/ekwiwalentu/innych sytuacji wymienionych w kryterium.
- 44 × 44 CSS px to kryterium **AAA 2.5.5**, nie wymóg poziomu AA. Większy obszar klikalny jest jednak użytecznym zaleceniem dla obsługi dotykowej.
- Gest przeciągania musi mieć alternatywę obsługi jednym wskaźnikiem, która nie wymaga przeciągania (**2.5.7, AA**).

Źródła: [W3C: 2.5.8 – objaśnienie](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum), [WCAG 2.2](https://www.w3.org/TR/WCAG22/).

## Struktura, język i multimedia

- Ustal język strony w kodzie, np. `<html lang="pl">` (**3.1.1, A**); oznaczaj także fragmenty w innym języku (**3.1.2, AA**).
- Używaj semantycznych elementów HTML, logicznych nagłówków, etykiet i nazw kontrolek. Nazwa widoczna powinna być częścią nazwy dostępnej (**2.5.3, A**).
- Dla nagranych materiałów audio zapewnij napisy (**1.2.2, A**); dla nagranego wideo z istotną ścieżką wizualną zapewnij audiodeskrypcję lub równoważną alternatywę zgodnie z kryterium (**1.2.5, AA**). Dla transmisji na żywo obowiązują osobne kryteria.
- Nie twórz treści błyskających częściej niż dopuszczają progi WCAG (**2.3.1, A**); oferuj kontrolę nad ruchem odtwarzanym automatycznie, gdy wymagają tego kryteria.

## Lista kontrolna

- [ ] Krytyczne ścieżki działają samą klawiaturą, a fokus widać i nie znika pod stałymi elementami.
- [ ] Teksty i komponenty mają wymagany kontrast; błędy nie są kodowane jedynie kolorem.
- [ ] Formularze mają etykiety programowo powiązane z polami.
- [ ] Strona ma język, sensowną strukturę nagłówków i alternatywy dla treści nietekstowych.
- [ ] Cele interakcji spełniają 24 × 24 CSS px lub udokumentowany wyjątek.
- [ ] Automatyczny skan jest uzupełniony ręcznym przeglądem klawiaturą i czytnikiem ekranu.
