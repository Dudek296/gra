# Dziennik prac

## 2026-05-18

- Sprawdzono zawartość katalogu roboczego i znaleziono gotową wersję gry w pliku `gra_ciecie_wierzcholkowe_balans_1_3.html`.
- Dodano nową stronę `index.html` przeznaczoną dla GitHub Pages.
- Dodano poziomy trudności dla grafu dwumianowego: łatwy, normalny, trudny oraz własny.
- Dodano tryb grafu przecięć z oddzielnie rysowanymi wierzchołkami i cechami.
- W trybie grafu przecięć usuwanym obiektem są cechy, a nie wierzchołki.
- Dodano dokumentację projektu w plikach `PLAN.md` i `DZIENNIK.md`.
- Przygotowano lokalny commit `Initial GitHub Pages game` na gałęzi `main`.
- Uruchomiono lokalny podgląd strony pod adresem `http://127.0.0.1:8000/`.
- Utworzenie repozytorium GitHub i włączenie Pages czeka na autoryzację GitHub CLI.

## 2026-05-19

- Odświeżono autoryzację GitHub CLI dla konta `Dudek296`.
- Utworzono publiczne repozytorium `https://github.com/Dudek296/gra`.
- Wypchnięto gałąź `main` do GitHuba.
- Włączono GitHub Pages z gałęzi `main` i katalogu `/`.
- Potwierdzono dostępność strony pod adresem `https://Dudek296.github.io/gra/`.

## 2026-06-10

- Sprawdzono dostęp do GitHuba: zapisany token `gh` dla konta `Dudek296` jest nieważny i wymaga ponownego logowania.
- Dodano wizualizację wierzchołków spoza największej składowej jako małych, nieaktywnych punktów.
- Dodano licznik wierzchołków poza największą składową w panelu stanu gry.
- Wzmocniono wizualizację wierzchołków spoza największej składowej: są grupowane w swoje małe składowe i pokazują szare krawędzie między sobą.
- Przesunięto wierzchołki spoza największej składowej do bocznych pasów planszy, aby nie nachodziły na główną składową.
- Zmieniono etykiety wierzchołków głównej składowej na numerację lokalną od `1` do liczby widocznych wierzchołków tej składowej.
- Zmieniono regułę przycinania liści: pełna największa składowa jest używana bez przycinania, a liście są przycinane tylko wtedy, gdy dokładny solver nie radzi sobie z rozmiarem lub przekracza limit czasu.
- Przycięte awaryjnie liście pozostają widoczne jako małe, blade, nieinteraktywne wierzchołki z bladymi krawędziami.
- Wzmocniono widoczność awaryjnie przyciętych liści oraz ich połączeń z główną składową.
- Dodano w opisie trybu dwumianowego uzasadnienie, czemu liście mogą zostać wyłączone z ruchów.
- Dodano ustawienie `Pokazuj stopnie`, które zamienia etykiety wierzchołków z numerów na aktualne stopnie.
- Przy włączonym pokazywaniu stopni komunikat przykładowego optimum nie wypisuje indeksów usuwanych elementów.
- Dodano osobny tryb `Graf przecięć - beta`, zachowując poprzedni tryb grafu przecięć do porównania.
- W trybie beta cechy są rozmieszczone po bokach planszy, wierzchołki są grupowane według pierwszej cechy, a zwykłe krawędzie grafu przecięć są wyciszone.
- Poprawiono tryb `Graf przecięć - beta`: cechy wróciły na dół planszy, a wierzchołki są układane w kliki od lewej do prawej według pierwszej cechy.
- W zwykłym trybie grafu przecięć dodano większy odstęp między wierzchołkami a cechami oraz przycisk przełączający układ wierzchołków na kliki.

## 2026-06-17

- Usunięto osobny model `Graf przecięć - beta`; układ klik pozostał jako przełącznik w zwykłym grafie przecięć.
- Poprawiono układ klik: szare wierzchołki spoza największej składowej trafiają do górnego pasa, a aktywne kliki mają większe odstępy.
- Dodano drugi wariant celu gry: największa pozostała składowa ma być mniejsza niż połowa początkowej składowej w grze.
- Zwiększono pola trafienia elementów SVG i szerokość planszy na małych ekranach, żeby obsługa dotykowa była wygodniejsza.
- Doprecyzowano opisy celu `< 1/2`: próg jest warunkiem sukcesu, a wynikiem gry pozostaje minimalna liczba usuniętych elementów.
- Zmiana celu gry przelicza optimum na tej samej planszy zamiast losować nowy graf.
- Dodano uwagę przy wyborze celu, że do gry zalecane jest wygenerowanie nowej planszy, oraz przeskalowano poziomy trudności do `n=25/50/75`.
- Utworzono backup bieżącej wersji strony w `backups/index-2026-06-17-19b29d8.html`.
- Usunięto poziom trudności `Trudny`, zostawiając większe parametry jako możliwość w trybie `Własny`.
- Przeniesiono uwagę o zalecanym generowaniu nowej planszy pod dynamiczny komunikat w panelu `Stan gry`; pojawia się dopiero po zmianie celu.
- Przeniesiono ostrzeżenie o dużych parametrach do widocznej uwagi pod wyborem poziomu `Własny`.
- Dodano zwijaną podpowiedź po opisie warunku celu, dotyczącą zaczynania od wierzchołków wysokiego stopnia i hubów w sieciach.
- Uproszczono panel `Stan gry`: widoczne zostały próg celu i rozmiar największej składowej, a pozostałe statystyki trafiły pod przycisk `dla ciekawskich`.
- Utworzono backup wersji `43f03ba` w `backups/index-2026-06-17-43f03ba.html`.
- Rozbudowano podpowiedzi: dwie pierwsze opisują graf dwumianowy, druga doprecyzowuje szukanie optimum, a trzecia opisuje graf przecięć i cięcie połączeń między klikami.
- Usunięto spod podpowiedzi akapity o poziomach trudności, zostawiając opis liści w trybie dwumianowym.

## 2026-06-18

- Utworzono backup wersji `1d734b6` w `backups/index-2026-06-18-1d734b6.html`.
- Złagodzono poziom `Łatwy`: w grafie dwumianowym używa średniego stopnia około `2.3`, a w grafie przecięć parametru `nmp^2=2.3`.
- Skrócono tytuły podpowiedzi do samych nazw modeli grafów oraz schowano pola parametrów poza poziomem `Własny`, gdzie startują od ustawień normalnych.
- Skrócono tytuł strony do `Rozspójnianie grafu losowego`, przeniesiono uwagę poziomu `Własny` do panelu `Stan gry` i przywrócono numerowane tytuły podpowiedzi.
- Uproszczono etykiety celu `< 1/2` i modelu dwumianowego oraz zmieniono górny opis na stały opis obu modeli naraz.
- Dopisano we wstępie informację o największej składowej i szarych wierzchołkach poza nią; w układzie klik cechy są rozmieszczane od prawej do lewej według liczby wierzchołków.
- Dodano we wstępie zdanie, że graf dwumianowy i graf przecięć są klasycznymi przykładami grafów losowych.
