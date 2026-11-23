# 02. Użyteczność i interakcje

Poniższe heurystyki to zasady przeglądu interfejsu, a nie wymogi zgodności WCAG. Odnoszą się do całego doświadczenia, szczególnie do przepływów zadaniowych.

## 10 heurystyk Nielsena

1. **Pokazuj stan systemu**: po akcji informuj, co się dzieje (np. ładowanie, zapis, wynik).
2. **Mów językiem użytkownika**: używaj znanych pojęć i kolejności odpowiadającej realnemu zadaniu.
3. **Daj kontrolę i wyjście**: zapewnij anulowanie, cofnięcie lub łatwy powrót, gdy to możliwe.
4. **Zachowuj spójność**: ten sam wzorzec i termin powinien oznaczać to samo w całym serwisie.
5. **Zapobiegaj błędom**: waliduj wcześniej, ograniczaj ryzykowne pomyłki i jasno pokazuj konsekwencje.
6. **Rozpoznawanie zamiast zapamiętywania**: pokazuj opcje, kontekst i potrzebne informacje w miejscu działania.
7. **Obsługuj początkujących i zaawansowanych**: skróty i personalizacja mogą przyspieszać pracę, jeśli nie przeszkadzają nowym osobom.
8. **Projektuj oszczędnie**: każda zbędna informacja konkuruje z ważną.
9. **Pomagaj rozpoznać, zrozumieć i naprawić błąd**: komunikat mówi co się stało i jak postąpić dalej.
10. **Zapewnij pomoc**: instrukcje powinny być łatwe do znalezienia, zadaniowe i konkretne.

Źródło: [Nielsen Norman Group: 10 heurystyk użyteczności](https://www.nngroup.com/articles/ten-usability-heuristics/).

## Nawigacja i orientacja

- Stosuj nazwy kategorii zrozumiałe bez znajomości struktury organizacji. Wyróżnij bieżącą lokalizację i aktywny element nawigacji.
- Link powinien opisywać cel, zamiast powtarzać ogólne „kliknij tutaj”. Zapewnij spójne działanie odnośników i przycisków.
- Dla rozbudowanych stron udostępnij wyszukiwanie, filtry lub okruszki nawigacyjne, jeśli pomagają wykonać zadanie.
- Zachowaj przewidywalność: interakcja powinna mieć widoczny skutek, a długie działania – stan postępu.

Są to praktyki projektowe; konkretne wymagania dot. nazw, struktury i klawiatury opisuje [WCAG 2.2](https://www.w3.org/TR/WCAG22/).

## Informacja zwrotna i błędy

- Potwierdzaj istotne działania, np. zapis, wysłanie, dodanie do koszyka. Nie wymagaj dodatkowego potwierdzania działań łatwych do cofnięcia.
- Dla błędu wskaż pole lub krok, przyczynę i konkretną metodę naprawy. Zachowuj już wprowadzone dane.
- Przed nieodwracalnym usunięciem pokaż konsekwencję i pozwól zweryfikować wybór.
- Nie opieraj komunikatu wyłącznie na kolorze ani na krótkim czasie wyświetlania.

## Przegląd heurystyczny

Dla każdej heurystyki zapisz: ekran/przepływ, problem obserwowany przez użytkownika, wpływ na wykonanie zadania, wagę oraz proponowaną poprawkę. Traktuj wynik jako listę hipotez do weryfikacji, nie jako pomiar satysfakcji ani substytut testu z użytkownikami.
