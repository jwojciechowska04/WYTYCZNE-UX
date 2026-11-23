# 05. Wydajność i ocena

## Core Web Vitals

Google definiuje trzy Core Web Vitals opisujące doświadczenie wczytywania, responsywności i stabilności wizualnej. Celem dla **75. percentyla odsłon** jest osiągnięcie wartości „dobrej” dla każdego wskaźnika:

| Wskaźnik | Co mierzy | Dobra wartość |
|---|---|---:|
| LCP (Largest Contentful Paint) | czas wyświetlenia największego elementu treści | ≤ 2,5 s |
| INP (Interaction to Next Paint) | opóźnienie reakcji interfejsu na interakcje | ≤ 200 ms |
| CLS (Cumulative Layout Shift) | nieoczekiwane przesunięcia treści | ≤ 0,1 |

„Dobra wartość” to próg źródła Google, nie gwarancja użyteczności ani wymóg WCAG. Oceniaj percentyl 75, oddzielnie dla urządzeń/stron, jeśli dane na to pozwalają. Dane terenowe opisują rzeczywistych użytkowników; test laboratoryjny pomaga odtworzyć i diagnozować problemy, ale nie zastępuje pola.

Źródła: [Google Search Central: Core Web Vitals](https://developers.google.com/search/docs/appearance/core-web-vitals), [web.dev: metodologia progów](https://web.dev/articles/defining-core-web-vitals-thresholds).

## Praktyczne kierunki poprawy

- Zmniejsz rozmiar obrazów i dostarczaj odpowiednią rozdzielczość; nie ładuj obrazów poza ekranem bez potrzeby.
- Ogranicz zasoby blokujące renderowanie i ciężki JavaScript; dziel kod oraz odkładaj niekrytyczne zasoby.
- Ustal wymiary mediów i rezerwuj przestrzeń przed ich załadowaniem, by ograniczyć CLS.
- Szybko udostępnij główną treść; sprawdź serwer, zasoby krytyczne i czas renderowania elementu LCP.
- Zmierz reakcję na rzeczywiste interakcje i przenieś długie zadania poza główny wątek, gdzie to możliwe.

Szczegóły wskaźników i technik: [LCP](https://web.dev/articles/lcp), [INP](https://web.dev/articles/inp), [CLS](https://web.dev/articles/cls).

## Ocena użyteczności i dostępności

Użyj kilku metod, bo każda wykrywa inny typ problemów:

1. **Automatyczne sprawdzenia**: semantyka, brakujące nazwy, część problemów kontrastu. To narzędzie do wykrywania, nie dowód pełnej dostępności.
2. **Ręczny przegląd**: klawiatura, widoczność i kolejność fokusu, powiększenie, reflow, komunikaty błędów i tekst alternatywny.
3. **Testy z czytnikiem ekranu**: sprawdź nazwy, role, stany, kolejność i przepływy zadań.
4. **Testy z użytkownikami**: obserwuj, czy osoby z grup docelowych kończą realistyczne zadania. Rejestruj trudności i kontekst, nie tylko deklarowane opinie.
5. **Dane produkcyjne**: porzucone formularze, wyszukiwania bez wyników, błędy i Core Web Vitals mogą wskazać miejsca wymagające dalszej diagnozy.

W3C przypomina, że narzędzia oceny wspierają, ale nie rozstrzygają same o dostępności. Zobacz [WAI: ocena dostępności](https://www.w3.org/WAI/test-evaluate/).

## Minimalny raport przeglądu

Zapisz datę, wersję strony, przeglądarkę/urządzenie, zadanie, metodę i kryterium, obserwowany problem, wpływ na użytkownika, priorytet oraz poprawkę. Dla pomiarów wydajności podaj, czy wynik pochodzi z danych terenowych czy laboratoryjnych oraz percentyl.
