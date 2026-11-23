# 03. Układ i responsywność

## Dostosowanie do ekranu

- Projektuj treść tak, by działała przy różnych szerokościach, orientacjach, powiększeniu i metodach wejścia. Breakpointy dobieraj do momentu, w którym treść przestaje działać, nie do konkretnych modeli urządzeń.
- Ustaw poprawny viewport, zwykle `<meta name="viewport" content="width=device-width, initial-scale=1">`; nie blokuj powiększania przez użytkownika.
- **WCAG 1.4.10 Reflow, AA**: przy szerokości odpowiadającej 320 CSS px dla przewijanej pionowo treści (lub wysokości odpowiadającej 256 CSS px dla przewijanej poziomo) treść powinna być prezentowana bez przewijania w dwóch kierunkach, z wyjątkami dla treści wymagających układu dwuwymiarowego.
- **WCAG 1.4.4 Resize Text, AA**: tekst można powiększyć do 200% bez utraty treści lub funkcji.
- **WCAG 1.4.12 Text Spacing, AA**: po ustawieniu wartości odstępów podanych w kryterium (m.in. wysokość linii 1,5× rozmiar czcionki, odstęp po akapicie 2×) nie może dochodzić do utraty treści ani funkcji.

Źródła: [W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/), [MDN: Responsive design](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Responsive_Design).

## Hierarchia i czytelność

- Najważniejsze działanie i informację umieść w czytelnej hierarchii. Używaj nagłówków opisujących zawartość kolejnych sekcji.
- Utrzymuj czytelny kontrast, dostateczny rozmiar tekstu i odstępy; testuj faktyczny tekst na faktycznym tle.
- Nie koduj informacji samym położeniem, kształtem, kolorem lub dźwiękiem; dodaj tekstowe wskazówki tam, gdzie są potrzebne.
- Stosuj elastyczne układy i obrazy, które nie wymuszają poziomego przewijania całego widoku. Tabele i diagramy mogą wymagać własnego, ograniczonego sposobu prezentacji.

## Stabilność wizualna

- Rezerwuj miejsce na obrazy, reklamy i inne elementy ładowane później, by uniknąć nieoczekiwanych przesunięć treści.
- Nie przesuwaj fokusu ani nie zmieniaj kontekstu bez działania użytkownika.
- Sprawdź układ w wąskim widoku, przy powiększeniu 200% oraz przy powiększeniu tekstu/niestandardowych odstępach.

## Lista kontrolna

- [ ] Brak poziomego przewijania strony przy szerokości 320 CSS px, poza uzasadnionymi wyjątkami WCAG.
- [ ] Treść działa po powiększeniu do 200% i zwiększeniu odstępów.
- [ ] Elementy ładowane asynchronicznie nie powodują zaskakujących przeskoków.
- [ ] Kluczowe zadanie można wykonać zarówno na małym, jak i dużym ekranie.
