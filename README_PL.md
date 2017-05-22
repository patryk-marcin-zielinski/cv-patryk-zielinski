# gulp-starter

Prosty starter gulpa dla projektów front-endowych.

## Podstawowe elementy

- Kompilator SASS (używaj rozszerzenia `.scss` lub zmień je w `gulpfile.js`)
- Minimalizacja CSS
- Łączenie (concat) plików JS
- JSHint (dla ES6)
- Optymalizacja obrazów

## Wymagania

- Node.JS &ge; 6.1
- npm &ge; 4.6

## Instrukcja

1. Zrób fork tego repo. Sprawdź [GitHub Help](https://help.github.com/articles/fork-a-repo/) jeśli potrzebujesz pomocy.
2. Zainstaluj pakiety npm: `npm install`.
3. Umieść pliki w folderach wewnątrz katalogu `src`.
4. Uruchom gulpa: `gulp`.

## Q&A

### Dlaczego uglify() jest w komentarzu?

Podczas testowania [gulpfile.js](gulpfile.js), `gulp-uglify` wyrzucał błąd (sprawdź więcej szczegółów [tutaj](https://gist.github.com/WojtekWernicki/5bb1a1722ad94ff7c2cbd1f32169188d)). Zdecydowałem, że zdezaktywuję go, tak samo jak `gulp-rename` linię wyżej. Pliki JS-a będą łączone w jeden, ale nie będą minimalizowane. Podejrzewam, że jest to wina mojego komputera (Windows 10), dlatego jeśli chcesz zobaczyć czy Twój Node i gulp są w stanie minimalizować JS-a, po prostu odkomentuj te dwie linie i uruchom `gulp`. Jeśli wiesz jak rozwiązać ten problem, wykonaj proszę pull request.

### Dlaczego `gulp-watch` nie uruchamia się przy nowych zdjęciach?

Nie mam pojęcia ¯ \\\_(ツ)_/¯  Zrestartuj gulpa, wtedy `gulp-watch` zoptymalizuje Twoje zdjęcia. Jeśli wiesz jak rozwiązać ten problem, wykonaj proszę pull request.

### Co oznaczają te pliki `.keep`?

Nic. Stworzyłem je wewnątrz folderów, ponieważ Git nie śledzi pustych katalogów (zobacz ten [wątek](http://stackoverflow.com/questions/115983/how-can-i-add-an-empty-directory-to-a-git-repository) na Stack Overflow). Możesz je usunąć, gdy umieścisz swoje pliki w tych folderach.

## Licencja

[MIT License](LICENSE)