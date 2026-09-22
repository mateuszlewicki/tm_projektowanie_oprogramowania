# Git i Github

## Przydatne linki

#### Git

- https://git-scm.com/learn
- https://git-scm.com/cheat-sheet
- https://git-scm.com/videos
- https://learn.microsoft.com/en-us/training/modules/intro-to-git/
- https://learngitbranching.js.org
- https://ohmygit.org
- https://git-scm.com/book/en/v2
- https://roadmap.sh/git
- https://rogerdudler.github.io/git-guide/
- https://git-scm.com/docs/gitignore


#### GitHub 
- https://docs.github.com/en/get-started/using-github/hello-world
- https://learn.microsoft.com/en-us/contribute/content/git-github-fundamentals

#### Kontrola wersji
- https://git-scm.com/book/pl/v2/Pierwsze-kroki-Wprowadzenie-do-kontroli-wersji
- https://www.atlassian.com/pl/git/tutorials/what-is-version-control
- https://github.com/resources/articles/what-are-code-repositories
- https://github.com/resources/articles/what-is-version-control

#### Visual Studio Code i git
- https://code.visualstudio.com/docs/sourcecontrol/repos-remotes

#### Warto znać!
- https://www.conventionalcommits.org/en/v1.0.0/
- https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716


## Kontrola wersji,
nazywana również kontrolą źródła, to praktyka polegająca na śledzeniu zmian w kodzie oprogramowania i zarządzaniu tymi zmianami. Systemy kontroli wersji to narzędzia programowe, które pomagają zespołom tworzącym oprogramowanie zarządzać zmianami w kodzie źródłowym na przestrzeni czasu

![SCM](img/img1.jpg)

## Git
jest obecnie najczęściej stosowanym nowoczesnym systemem kontroli wersji na świecie. Jest to dojrzały, aktywnie prowadzony projekt open source zainicjowany w 2005 roku przez Linusa Torvaldsa, słynnego twórcę jądra systemu operacyjnego Linux.

### .gitignore

Plik .gitignore określa nieśledzone pliki, które Git powinien ignorować. Pliki już śledzone przez Git nie podlegają tym regułom.

Każda linia w pliku .gitignore definiuje wzorzec. Podczas rozstrzygania, czy dana ścieżka ma zostać zignorowana, Git sprawdza wzorce z różnych źródeł według kolejności priorytetów — od najwyższego do najniższego (w ramach tego samego poziomu priorytetu decyduje ostatni pasujący wzorzec):

1. Wzorce odczytane z wiersza poleceń dla komend, które to obsługują.
2. Wzorce odczytane z pliku .gitignore znajdującego się w tym samym katalogu co ścieżka lub w dowolnym katalogu nadrzędnym (aż do głównego katalogu roboczego). Wzorce z plików na wyższych poziomach są nadpisywane przez te na niższych poziomach, aż do katalogu zawierającego dany plik. Wzorce te są dopasowywane względnie do lokalizacji danego pliku .gitignore. Projekt zazwyczaj zawiera takie pliki .gitignore w swoim repozytorium z wzorcami dla plików generowanych podczas budowania projektu.
3. Wzorce odczytane z pliku `$GIT_COMMON_DIR/info/exclude`.
4. Wzorce odczytane z pliku określonego przez zmienną konfiguracji `core.excludesFile`.

### git clone
Pobiera całe zdalne repozytorium z serwera na lokalny dysk komputera. Tworzy pełną kopię projektu wraz z pełną historią zmian i gałęziami.
Przykładowa komenda: `git clone https://github.com/mateuszlewicki/tm_projektowanie_oprogramowania.git`

### git commit

Zapisuje stan plików z obszaru roboczego w historii repozytorium jako nową migawkę. Każdy zapis wymaga dołączenia krótkiego komunikatu objaśniającego wprowadzone zmiany.

Przykładowa komenda: `git commit -m "Dodano funkcję logowania"`

### git add

Dodaje zmienione lub nowe pliki do obszaru roboczego (tzw. staging area). Pozwala na precyzyjne wyselekcjonowanie modyfikacji przeznaczonych do zapisania.

Przykładowa komenda: `git add plik.txt` lub `git add .` lub `git add -A` (wszystkie pliki).

### git push

Wysyła lokalne zatwierdzone zmiany na serwer zdalny (np. GitHub, GitLab, Bitbucket), udostępniając je innym uczestnikom projektu.
Przykładowa komenda: `git push origin main`

### git checkout

Umożliwia przełączanie się między gałęziami (branches) oraz przywracanie wcześniej zapisanych wersji plików. W nowszych wersjach Gita do przełączania gałęzi stosuje się polecenie `git switch`.

Przykładowa komenda: `git checkout nowa-galaz` (lub utworzenie nowej gałęzi: `git checkout -b nowa-galaz`)

## Pull Request

Funkcja platform hostingowych (np. GitHub, GitLab), stanowiąca formalną prośbę o włączenie zmian z osobnej gałęzi do głównego kodu projektu. Służy do przeprowadzania przeglądu kodu (code review), zgłaszania uwag oraz testowania przed scaleniem.