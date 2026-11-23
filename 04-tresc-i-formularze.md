# 04. Treść i formularze

## Język i treść

- Stosuj język zrozumiały dla odbiorców; rozwijaj skróty i objaśniaj terminy specjalistyczne, gdy są potrzebne.
- Pisz nagłówki i etykiety opisujące temat lub cel. Linki formułuj tak, aby ich cel był zrozumiały z kontekstu; unikaj niejednoznacznego „więcej”.
- Używaj poprawnego języka strony (`lang`) i oznaczaj fragmenty w innym języku. Zadbaj o kolejność treści, która pozostaje zrozumiała po odczycie liniowym lub bez stylów.
- Wyróżnienia wizualne nie mogą być jedynym sposobem przekazywania znaczenia.

Powiązane kryteria: [WCAG 2.2](https://www.w3.org/TR/WCAG22/) – 2.4.6 Nagłówki i etykiety (AA), 2.4.4 Cel linku w kontekście (A), 3.1.1 Język strony (A), 3.1.2 Język części (AA).

## Etykiety, instrukcje i pola

- Każde pole formularza, checkbox, przycisk opcji i lista wyboru ma widoczną etykietę opisującą jego cel. Powiąż ją programowo z kontrolką, najlepiej przez `<label for="...">` i zgodne `id`.
- Placeholder nie zastępuje etykiety: znika przy wpisywaniu i może mieć niewystarczający kontrast.
- Wskaż pola wymagane i opcjonalne oraz wymagany format danych. Umieść instrukcję tak, aby była dostępna również dla technologii asystujących.
- Grupuj powiązane kontrolki semantycznie (np. `fieldset` i `legend` dla grupy wyboru).
- **WCAG 3.3.2 Etykiety lub instrukcje, A** wymaga etykiet lub instrukcji, gdy treść wymaga danych wejściowych. W3C zaleca, by instrukcje formatów i wymagań były dostępne w kontekście pola.

Źródła: [W3C WAI: etykiety kontrolek](https://www.w3.org/WAI/tutorials/forms/labels/), [W3C WAI: instrukcje formularzy](https://www.w3.org/WAI/tutorials/forms/instructions/).

## Walidacja i obsługa błędów

- Waliduj dane i wyjaśnij problem prostym językiem. Wskaż pole, błąd i sposób poprawy; nie polegaj wyłącznie na kolorze.
- Jeśli wykryty zostaje błąd, opisz go tekstowo (**WCAG 3.3.1, A**). Jeśli znane są sugestie korekty, podaj je, chyba że narusza to bezpieczeństwo lub cel (**3.3.3, AA**).
- Dla transakcji prawnych/finansowych, zmian danych albo przesyłania odpowiedzi zapewnij wymagane zabezpieczenie: możliwość odwrócenia, sprawdzenia i korekty lub potwierdzenia (**3.3.4, AA**, zakres i wyjątki opisane w kryterium).
- Nie kasuj poprawnych wartości po błędzie walidacji. Przenieś fokus do błędu podsumowującego lub pierwszego błędnego pola, jeśli jest to zgodne z kontekstem, i zapewnij dostępne powiązanie komunikatu z polem.

Źródło: [WCAG 2.2 – kryteria 3.3](https://www.w3.org/TR/WCAG22/#input-assistance).

## Lista kontrolna

- [ ] Każda kontrolka ma zrozumiałą, programowo powiązaną nazwę.
- [ ] Wymagania i formaty są podane przed lub przy właściwym polu.
- [ ] Błędy są opisane tekstem i zawierają jasną ścieżkę naprawy.
- [ ] Formularz zachowuje dane po nieudanej walidacji.
- [ ] Etykiety, instrukcje i komunikaty są dostępne bez myszy i dla technologii asystujących.
