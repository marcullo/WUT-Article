# WUT Article - LaTeX

######  [Demo :arrow_down:][link-download-latex]

Szablon LaTeX artykułu z treścią: *Zasady składania artykułu z wykorzystaniem zmodyfikowanego szablonu LNCS*.

**Środowisko testowe**:

- `Ubuntu 18.04.3 LTS`
- `TeXstudio 2.12.16`

## Instalacja

1. Zainstaluj *TeXStudio*.

```shell
apt-get install texstudio texlive texlive-lang-polish texlive-latex-extra texlive-science
```

2. [Zainstaluj pakiet][package-installation], gdyby jeszcze któregoś brakowało.

## Konfiguracja

1. Wczytaj plik `main.tex`.

W folderze `sections` znajdziesz poszczególne sekcje artykułu. Do folderu `media` powinny trafić elementy multimedialne, np. obrazki. W `class/class.cls` zastaniesz zmodyfikowaną klasę: dodałem `% Polish section` z polskimi słowami kluczowymi.

2. Upewnij się w ustawieniach, że domyślnym kompilatorem jest PdfLaTeX.
3. Skompiluj.

**Uwaga**: W niektórych sytuacjach wymagana jest ręczna modyfikacja odstępów pionowych (np. poprzez `\vspace`). Przy korzystaniu z szablonu zalecany jest zdrowy rozsądek i samodzielne dopracowanie ostatecznego wyglądu dokumentu, głównie pod względem odstępów pionowych.

## Redakcja

### Personalizacja

Zamień autora `Gall Anonim` (`\author`, `\authorrunning`) i jego adres e-mail (`\email`) na Twoje dane.

### Słowa kluczowe

Słowa z poniższego zestawu są predefiniowane. Użycie: np. `\theorem{Teoria Wszechświata}` → `Teoria 1. Teoria Wszechświata`.

```
Streszczenie  Słowa kluczowe  Twierdzenie  Hipoteza  Wniosek  Definicja  Przykład  Zadanie
Rys.  Lemat  Tab.  Uwaga  Problem  Własność  Propozycja  Pytanie  Spostrzeżenie  Rozwiązanie  Teoria
```

### Czyszczenie projektu

Aby wyczyścić pliki pośrednie i PDFy, uruchom:

```shell
make clean
```

[link-download-latex]: https://github.com/marcullo/WUT-Article/releases/latest/download/Anonim_artykul_latex.pdf
[package-installation]: https://tex.stackexchange.com/questions/73016/how-do-i-install-an-individual-package-on-a-linux-system
