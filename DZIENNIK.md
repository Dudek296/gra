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
