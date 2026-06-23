# Changelog

Wszystkie zmiany w projekcie **DTexturePack** są dokumentowane w tym pliku.

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
