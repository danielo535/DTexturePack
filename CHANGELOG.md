# Changelog

Wszystkie zmiany w projekcie **DTexturePack** są dokumentowane w tym pliku.

---

## [v0.1.5] - 2026-07-12

### Added

* Wprowadzono **Pack Presser** — system walidacji projektu przed eksportem paczki:

  * wykrywanie błędów i ostrzeżeń w poszczególnych kategoriach (ustawienia, przedmioty, bloki, zbroja, symbole, łuk, kusza),
  * automatyczne naprawy (duplikaty `CustomModelData`, konflikty slotów tekstury, domyślna nazwa i wersja paczki, reset niepoprawnego `.mcmeta`),
  * nawigacja z raportu walidacji bezpośrednio do edytowanego zasobu,
  * blokada generowania paczki do momentu pomyślnego przejścia walidacji.
* Dodano **interaktywne podglądy 3D** oparte na Three.js:

  * obracane podglądy modeli 3D przedmiotów (Blockbench),
  * podgląd bloków jako sześcian 3D w siatce i edytorze,
  * edytor transformacji modelu (`display`: thirdperson, firstperson, gui, ground, fixed),
  * generowanie miniatur (snapshotów) oraz preload podglądów poza widocznym obszarem.
* Dodano **pełną obsługę języków polskiego i angielskiego**:

  * tłumaczenie interfejsu edytora, landingu i Pack Presser,
  * przełącznik języka z zapisem preferencji w cookie,
  * automatyczne wykrywanie języka z nagłówka `Accept-Language`.
* Dodano **stronę dokumentacji `/docs`**:

  * przewodnik PL/EN obejmujący m.in. pierwsze kroki, `CustomModelData`, opisy z kodami §, format `.dtpack`, strukturę paczki i FAQ,
  * wyszukiwarka treści dokumentacji.
* Przebudowano **stronę marketingową (Landing Page)**:

  * sekcje: hero, funkcje, edytor, platformy, workflow i CTA,
  * **na żywo aktualizowane statystyki serwisu** (liczba wygenerowanych paczek Java / Bedrock / Geyser),
  * odznaki wsparcia platform per funkcja (Java / Bedrock / both / partial / WIP).
* Dodano **autosave sesji w przeglądarce** — automatyczny zapis stanu projektu w `localStorage` z możliwością przywrócenia po powrocie na stronę.
* Dodano **overlay generowania paczki** z wielofazowym postępem (przygotowanie → wysyłanie → budowa na serwerze → pobieranie).
* Rozbudowano moduł **symboli / czcionek (Fonts)**:

  * automatyczne wyliczanie metryk glifu (`ascent`, `height`) z pliku PNG,
  * podgląd symbolu w kontekście linii tekstu Minecraft,
  * eksport dla Java Edition oraz eksperymentalny eksport dla Bedrock Edition.
* Dodano nowe elementy interfejsu edytora:

  * siatka assetów z paginacją, filtrowaniem i konfiguracją gęstości kolumn,
  * filtry przedmiotów (simple / animacja / 3D / CMD / mcmeta),
  * pobieranie pojedynczych plików lub archiwum ZIP z karty zasobu,
  * edytor opisu paczki z kodami formatowania Minecraft (§) i podglądem kolorów,
  * wyszukiwany wybór wersji Minecraft (`pack_format`),
  * odznaki wsparcia platform przy poszczególnych zakładkach.

### Changed

* Zaktualizowano identyfikację wizualną projektu:

  * zmieniono branding z **NiceCode** na **TexturePack**,
  * odświeżono logo, nazwę i opis aplikacji.
* Przebudowano architekturę frontendu:

* Zmieniono proces generowania paczek — eksport wymaga teraz przejścia walidacji **Pack Presser** (wcześniej generowanie uruchamiało się od razu).
* Zastąpiono własne powiadomienia systemowe biblioteką **Sonner** z obsługą tłumaczeń.
* Rozbudowano istniejące zakładki edytora:

  * **Bloki** — siatka z podglądem 3D, paginacja i integracja z walidacją,
  * **Zbroja** — siatka, podpowiedzi platform i UI `CustomModelData`,
  * **Przedmioty** — siatka z podglądem 3D, filtry tagów i edytor modelu inline,
  * **Symbole** — siatka z auto-metriki i podglądem glifu.
* Ujednolicono opis platformy **Geyser** w interfejsie jako hybrydę Java + Bedrock z wyraźnym oznaczeniem obsługiwanych funkcji.

### Improved

* Usprawniono wydajność podglądów 3D dzięki cache'owaniu tekstur, geometrii i snapshotów miniatur.
* Zwiększono wygodę korzystania z edytora:

  * responsywny sidebar na urządzeniach mobilnych,
  * wspólny panel zarządzania zasobami (`ManagerPanel`) we wszystkich zakładkach,
  * ujednolicony dialog edycji zasobu z Drag & Drop i podglądem tekstur,
  * dialog „Nowa sesja” z potwierdzeniem przed wyczyszczeniem pracy.
* Rozszerzono metody przesyłania plików (Drag & Drop oraz Clipboard Paste) na wszystkie typy zasobów w edytorze.

### Fixed

* Dodano walidację po stronie serwera przed budową paczki (`GenerateRequestValidator`) — blokada generowania przy brakujących polach lub niepoprawnym formacie animacji.
* Naprawiono obsługę duplikatów `CustomModelData` oraz konfliktów slotów tekstury poprzez auto-naprawy Pack Presser.
* Wprowadzono ustrukturyzowane odpowiedzi błędów HTTP zamiast generycznych kodów 500.
* Dodano ostrzeżenie przy przepełnieniu limitu `localStorage` podczas autosave sesji.
* Poprawiono komunikaty przy imporcie archiwum ZIP bez osadzonego pliku `data.dtpack`.

---

## [v0.1.4] - 2026-06-22

### Added

* Dodano możliwość tworzenia **własnych łuków (Bows) oraz kusz (Crossbows)** wraz z obsługą:

  * własnych modeli 3D,
  * wartości `CustomModelData`,
  * niestandardowych tekstur.
* Dodano funkcję **automatycznej podmiany tekstury przedmiotu** dla wszystkich dodawanych modeli 3D, co znacząco upraszcza proces konfiguracji zasobów.
* Dodano możliwość **przeciągania i upuszczania (Drag & Drop)** obrazów bezpośrednio na stronę w celu szybszego przesyłania plików.
* Dodano obsługę **wklejania skopiowanych grafik oraz modeli 3D** bezpośrednio do aplikacji za pomocą skrótów systemowych (Ctrl+V).

### Changed

* Zaktualizowano identyfikację wizualną projektu:

  * zmieniono logo projektu na **NiceCode**,
  * odświeżono branding aplikacji.
* Zmieniono domyślną kolorystykę interfejsu z **Dark Black** na **Dark Aqua**, poprawiając czytelność oraz estetykę strony.
* Przebudowano proces generowania paczek:

  * domyślnie wybraną opcją generowania jest teraz **Java Edition**,
  * opcja **Geyser** nie jest już wybierana automatycznie przy pierwszym uruchomieniu.

### Improved

* Usprawniono proces dodawania modeli 3D i tekstur poprzez automatyzację konfiguracji zasobów.
* Zwiększono wygodę korzystania z aplikacji dzięki nowym metodom przesyłania plików (Drag & Drop oraz Clipboard Paste).

---

## [v0.1.3] - 2026-01-30

### Changed

* Całkowicie przebudowano interfejs użytkownika (UI) strony.
* Zoptymalizowano pomniejsze elementy wizualne oraz funkcjonalne.

---

## [v0.1.2] - 2026-01-30

### Added

* Zaimplementowano animacje interfejsu użytkownika.
* Dodano wskaźnik statusu informujący o postępie procesu generowania paczki.
* Wprowadzono mechanizm automatycznego pobierania tekstur dla przedmiotów, których modele w nowszych wersjach gry nie wyświetlały się poprawnie (auto-fix).
* Dodano bezpośredni odnośnik do repozytorium projektu na GitHubie.

### Changed

* Zaktualizowano styl wizualny powiadomień systemowych.
* Zmodyfikowano strukturę katalogów modeli wewnątrz generowanej paczki dla lepszej kompatybilności.

### Fixed

* Naprawiono błąd uniemożliwiający poprawne generowanie paczek dla platformy Geyser.

---

## [v0.1.1] - 2026-01-22

### Added

* Dodano pełną obsługę tekstur bloków (Blocks) dla Minecraft Bedrock Edition.
* Zaimplementowano obsługę pancerzy (Armor) dla Minecraft Bedrock Edition.
* Opracowano generator struktury plików `.json` oraz manifestów specyficznych dla wersji Bedrock.

---

## [v0.1.0] - 2026-01-20

### Added

* **Pierwsze wydanie publiczne (Initial Release).**
* Udostępniono konfigurator metadanych paczki (nazwa, opis, ikona).
* Zaimplementowano generowanie paczek dla platform:

  * Minecraft Java Edition
  * Minecraft Bedrock Edition
* Dodano funkcję importu tekstur przedmiotów (Items).
* Umożliwiono eksport gotowego projektu do pliku `.zip`.

---

> **Nota:** Projekt znajduje się w fazie **BETA**. Funkcjonalności mogą ulegać znaczącym zmianom w kolejnych wersjach bez zachowania wstecznej kompatybilności.
