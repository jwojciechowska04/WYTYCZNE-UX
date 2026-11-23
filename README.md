# WYTYCZNE-UX
Jak korzystać z bazy

1. Zacznij od aspektu z mapy poniżej i otwórz powiązany plik.
2. Przy projektowaniu konkretnego elementu (np. formularza) sprawdź odpowiedni rozdział oraz kontrolną listę na końcu pliku.
3. Traktuj linki do standardów jako źródło normatywne. Linki do poradników objaśniających pomagają wdrożyć wymagania, ale nie zastępują standardu.
4. Przy zmianie standardów lub produktu sprawdź ponownie datę/wersję źródła. WCAG ma wersje i poziomy zgodności; w tej bazie użyto WCAG 2.2, poziom AA jako domyślnego punktu odniesienia dla dostępności.

## Mapa wiedzy

| Aspekt | Zakres | Materiał |
|---|---|---|
| Dostępność | WCAG 2.2 AA, kontrast, klawiatura, fokus, cele dotykowe, multimedia i alternatywy | [01-dostepnosc.md](01-dostepnosc.md) |
| Użyteczność i interakcje | Heurystyki, nawigacja, informacja zwrotna, błędy i kontrola użytkownika | [02-uzytecznosc.md](02-uzytecznosc.md) |
| Układ i responsywność | Małe ekrany, reflow, hierarchia, czytelność i stabilność układu | [03-uklad-i-responsywnosc.md](03-uklad-i-responsywnosc.md) |
| Treść i formularze | Język, etykiety, instrukcje, walidacja i komunikaty | [04-tresc-i-formularze.md](04-tresc-i-formularze.md) |
| Wydajność i ocena | Core Web Vitals, pomiary terenowe, testy eksperckie i z użytkownikami | [05-wydajnosc-i-ocena.md](05-wydajnosc-i-ocena.md) |

## Jak interpretować wytyczne

- **Wymaganie WCAG**: kryterium sukcesu testowane na poziomie A, AA albo AAA. Poziom i wyjątki są wskazane w opisie. Spełnienie kilku punktów nie oznacza automatycznie zgodności całej strony.
- **Dobra praktyka**: zalecenie użyteczności lub wydajności, które wspiera użytkownika, ale samo w sobie nie jest kryterium WCAG.
- **Wartość progowa**: liczba podana przez źródło, np. limit Core Web Vitals. Zachowaj warunki pomiaru, takie jak percentyl i typ danych.

## Szybka ścieżka przeglądu strony

1. Przejdź kluczowe zadania bez myszy, używając Tab, Shift+Tab, Enter, Spacja i Escape.
2. Sprawdź kontrast, tekst alternatywny, nagłówki, etykiety formularzy i skalowanie/zmianę szerokości.
3. Wykonaj najważniejsze zadanie na telefonie i przy powiększeniu treści.
4. Zmierz Core Web Vitals na danych terenowych, jeśli są dostępne.
5. Przeprowadź test użyteczności z osobami reprezentującymi grupy użytkowników; automat nie ocenia całego doświadczenia.

Szczegółowe procedury i listy kontrolne znajdują się w plikach tematycznych. Ta baza jest przewodnikiem projektowym, nie opinią prawną ani certyfikatem zgodności.
