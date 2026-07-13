# Changelog / Rejestr zmian

**PL:** Wszystkie zmiany w projekcie **DTexturePack** są dokumentowane w tym pliku.
**EN:** *All changes made to the **DTexturePack** project are documented in this file.*

---

## [v0.1.5] - 2026-07-12

### Dodano / Added

* **PL:** Wprowadzono **Pack Presser** — system walidacji projektu przed eksportem paczki.
  **EN:** *Introduced **Pack Presser** — a project validation system that runs before a pack can be exported.*

  * **PL:** Wykrywanie błędów i ostrzeżeń w poszczególnych kategoriach: ustawienia, przedmioty, bloki, zbroja, symbole, łuk i kusza.
    **EN:** *Detection of errors and warnings across individual categories: settings, items, blocks, armor, symbols, bows, and crossbows.*

  * **PL:** Automatyczne naprawy duplikatów `CustomModelData`, konfliktów slotów tekstury, brakującej domyślnej nazwy i wersji paczki oraz niepoprawnego pliku `.mcmeta`.
    **EN:** *Automatic fixes for duplicate `CustomModelData` values, texture slot conflicts, missing default pack names and versions, and invalid `.mcmeta` files.*

  * **PL:** Nawigacja z raportu walidacji bezpośrednio do edytowanego zasobu.
    **EN:** *Navigation directly from the validation report to the affected resource.*

  * **PL:** Blokada generowania paczki do momentu pomyślnego przejścia walidacji.
    **EN:** *Pack generation is blocked until validation is completed successfully.*

* **PL:** Dodano **interaktywne podglądy 3D** oparte na Three.js.
  **EN:** *Added **interactive 3D previews** powered by Three.js.*

  * **PL:** Obracane podglądy modeli 3D przedmiotów, między innymi modeli utworzonych w Blockbench.
    **EN:** *Rotatable previews of 3D item models, including models created in Blockbench.*

  * **PL:** Podgląd bloków jako sześcianów 3D w siatce oraz edytorze.
    **EN:** *Block previews displayed as 3D cubes in both the asset grid and editor.*

  * **PL:** Edytor transformacji modelu dla ustawień `display`: `thirdperson`, `firstperson`, `gui`, `ground` i `fixed`.
    **EN:** *A model transformation editor for `display` settings: `thirdperson`, `firstperson`, `gui`, `ground`, and `fixed`.*

  * **PL:** Generowanie miniatur oraz preload podglądów znajdujących się poza widocznym obszarem.
    **EN:** *Thumbnail snapshot generation and preloading of previews outside the visible viewport.*

* **PL:** Dodano **pełną obsługę języków polskiego i angielskiego**.
  **EN:** *Added **full Polish and English language support**.*

  * **PL:** Tłumaczenie interfejsu edytora, strony głównej oraz Pack Presser.
    **EN:** *Translations for the editor interface, landing page, and Pack Presser.*

  * **PL:** Przełącznik języka z zapisem preferencji w pliku cookie.
    **EN:** *A language switcher that stores the selected preference in a cookie.*

  * **PL:** Automatyczne wykrywanie języka na podstawie nagłówka `Accept-Language`.
    **EN:** *Automatic language detection based on the `Accept-Language` header.*

* **PL:** Dodano **stronę dokumentacji `/docs`**.
  **EN:** *Added a dedicated **`/docs` documentation page**.*

  * **PL:** Przewodnik w języku polskim i angielskim obejmujący między innymi pierwsze kroki, `CustomModelData`, opisy z kodami §, format `.dtpack`, strukturę paczki oraz FAQ.
    **EN:** *A Polish and English guide covering topics such as getting started, `CustomModelData`, descriptions with § formatting codes, the `.dtpack` format, pack structure, and frequently asked questions.*

  * **PL:** Wyszukiwarka treści dokumentacji.
    **EN:** *A documentation content search feature.*

* **PL:** Przebudowano **stronę marketingową — Landing Page**.
  **EN:** *Rebuilt the **marketing landing page**.*

  * **PL:** Dodano sekcje: hero, funkcje, edytor, platformy, workflow i CTA.
    **EN:** *Added hero, features, editor, platforms, workflow, and CTA sections.*

  * **PL:** Dodano **aktualizowane na żywo statystyki serwisu**, obejmujące liczbę wygenerowanych paczek Java, Bedrock i Geyser.
    **EN:** *Added **live service statistics**, including the number of generated Java, Bedrock, and Geyser packs.*

  * **PL:** Dodano odznaki wsparcia platform dla poszczególnych funkcji: Java, Bedrock, obie platformy, częściowe wsparcie i WIP.
    **EN:** *Added platform support badges for individual features: Java, Bedrock, both platforms, partial support, and WIP.*

* **PL:** Dodano **autosave sesji w przeglądarce** — stan projektu jest automatycznie zapisywany w `localStorage` i może zostać przywrócony po powrocie na stronę.
  **EN:** *Added **browser session autosave** — the project state is automatically stored in `localStorage` and can be restored after returning to the page.*

* **PL:** Dodano **overlay generowania paczki** z wielofazowym wskaźnikiem postępu: przygotowanie → wysyłanie → budowa na serwerze → pobieranie.
  **EN:** *Added a **pack generation overlay** with multi-stage progress: preparation → upload → server-side build → download.*

* **PL:** Rozbudowano moduł **symboli i czcionek — Fonts**.
  **EN:** *Expanded the **symbols and fonts module — Fonts**.*

  * **PL:** Automatyczne wyliczanie metryk glifu `ascent` i `height` na podstawie pliku PNG.
    **EN:** *Automatic calculation of the `ascent` and `height` glyph metrics from a PNG file.*

  * **PL:** Podgląd symbolu w kontekście linii tekstu Minecraft.
    **EN:** *Symbol previews displayed within a Minecraft-style text line.*

  * **PL:** Eksport dla Java Edition oraz eksperymentalny eksport dla Bedrock Edition.
    **EN:** *Export support for Java Edition and experimental export support for Bedrock Edition.*

* **PL:** Dodano nowe elementy interfejsu edytora.
  **EN:** *Added new editor interface components.*

  * **PL:** Siatka zasobów z paginacją, filtrowaniem i możliwością konfiguracji liczby kolumn.
    **EN:** *An asset grid with pagination, filtering, and configurable column density.*

  * **PL:** Filtry przedmiotów: simple, animacja, 3D, CMD i mcmeta.
    **EN:** *Item filters: simple, animation, 3D, CMD, and mcmeta.*

  * **PL:** Pobieranie pojedynczych plików lub archiwum ZIP bezpośrednio z karty zasobu.
    **EN:** *Downloading individual files or ZIP archives directly from an asset card.*

  * **PL:** Edytor opisu paczki z kodami formatowania Minecraft § i podglądem kolorów.
    **EN:** *A pack description editor with Minecraft § formatting codes and color previews.*

  * **PL:** Przeszukiwany wybór wersji Minecraft i wartości `pack_format`.
    **EN:** *A searchable Minecraft version and `pack_format` selector.*

  * **PL:** Odznaki wsparcia platform przy poszczególnych zakładkach.
    **EN:** *Platform support badges displayed next to individual tabs.*

### Zmieniono / Changed

* **PL:** Zaktualizowano identyfikację wizualną projektu.
  **EN:** *Updated the project's visual identity.*

  * **PL:** Zmieniono branding z **NiceCode** na **TexturePack**.
    **EN:** *Changed the branding from **NiceCode** to **TexturePack**.*

  * **PL:** Odświeżono logo, nazwę i opis aplikacji.
    **EN:** *Refreshed the application's logo, name, and description.*

* **PL:** Przebudowano architekturę frontendu.
  **EN:** *Reworked the frontend architecture.*

* **PL:** Zmieniono proces generowania paczek — eksport wymaga teraz przejścia walidacji **Pack Presser**. Wcześniej generowanie rozpoczynało się od razu.
  **EN:** *Changed the pack generation process — exporting now requires successful **Pack Presser** validation. Previously, generation started immediately.*

* **PL:** Zastąpiono własny system powiadomień biblioteką **Sonner** z obsługą tłumaczeń.
  **EN:** *Replaced the custom notification system with the **Sonner** library, including localization support.*

* **PL:** Rozbudowano istniejące zakładki edytora.
  **EN:** *Expanded the existing editor tabs.*

  * **PL:** **Bloki** — siatka z podglądem 3D, paginacja i integracja z walidacją.
    **EN:** ***Blocks** — a grid with 3D previews, pagination, and validation integration.*

  * **PL:** **Zbroja** — siatka, podpowiedzi dotyczące platform oraz interfejs `CustomModelData`.
    **EN:** ***Armor** — a grid, platform-related hints, and a `CustomModelData` interface.*

  * **PL:** **Przedmioty** — siatka z podglądem 3D, filtry tagów i wbudowany edytor modelu.
    **EN:** ***Items** — a grid with 3D previews, tag filters, and an inline model editor.*

  * **PL:** **Symbole** — siatka z automatycznym wyliczaniem metryk i podglądem glifu.
    **EN:** ***Symbols** — a grid with automatic metric calculation and glyph previews.*

* **PL:** Ujednolicono opis platformy **Geyser** w interfejsie jako rozwiązania hybrydowego łączącego Java i Bedrock, z wyraźnym oznaczeniem obsługiwanych funkcji.
  **EN:** *Standardized the description of the **Geyser** platform in the interface as a hybrid Java and Bedrock solution, with clearly marked supported features.*

### Ulepszono / Improved

* **PL:** Usprawniono wydajność podglądów 3D dzięki cache'owaniu tekstur, geometrii i snapshotów miniatur.
  **EN:** *Improved 3D preview performance by caching textures, geometry, and thumbnail snapshots.*

* **PL:** Zwiększono wygodę korzystania z edytora.
  **EN:** *Improved the editor's usability.*

  * **PL:** Dodano responsywny sidebar na urządzeniach mobilnych.
    **EN:** *Added a responsive sidebar for mobile devices.*

  * **PL:** Dodano wspólny panel zarządzania zasobami `ManagerPanel` we wszystkich zakładkach.
    **EN:** *Added a shared `ManagerPanel` resource management panel across all tabs.*

  * **PL:** Ujednolicono dialog edycji zasobu, dodając Drag & Drop oraz podgląd tekstur.
    **EN:** *Standardized the resource editing dialog and added Drag & Drop with texture previews.*

  * **PL:** Dodano dialog „Nowa sesja” z potwierdzeniem przed wyczyszczeniem bieżącej pracy.
    **EN:** *Added a “New Session” dialog requiring confirmation before clearing the current work.*

* **PL:** Rozszerzono obsługę przesyłania plików przez Drag & Drop oraz Clipboard Paste na wszystkie typy zasobów w edytorze.
  **EN:** *Extended Drag & Drop and Clipboard Paste file uploads to all resource types available in the editor.*

### Naprawiono / Fixed

* **PL:** Dodano walidację po stronie serwera przed rozpoczęciem budowy paczki za pomocą `GenerateRequestValidator`. Generowanie jest blokowane w przypadku brakujących pól lub niepoprawnego formatu animacji.
  **EN:** *Added server-side validation before starting the pack build using `GenerateRequestValidator`. Generation is blocked when required fields are missing or the animation format is invalid.*

* **PL:** Naprawiono obsługę duplikatów `CustomModelData` oraz konfliktów slotów tekstury poprzez automatyczne naprawy Pack Presser.
  **EN:** *Fixed duplicate `CustomModelData` values and texture slot conflicts through Pack Presser automatic fixes.*

* **PL:** Wprowadzono ustrukturyzowane odpowiedzi błędów HTTP zamiast ogólnych kodów 500.
  **EN:** *Introduced structured HTTP error responses instead of generic 500 status codes.*

* **PL:** Dodano ostrzeżenie wyświetlane po przekroczeniu limitu `localStorage` podczas automatycznego zapisywania sesji.
  **EN:** *Added a warning displayed when the `localStorage` limit is exceeded during session autosave.*

* **PL:** Poprawiono komunikaty wyświetlane podczas importowania archiwum ZIP bez osadzonego pliku `data.dtpack`.
  **EN:** *Improved messages displayed when importing a ZIP archive that does not contain an embedded `data.dtpack` file.*

---

## [v0.1.4] - 2026-06-22

### Dodano / Added

* **PL:** Dodano możliwość tworzenia **własnych łuków — Bows — oraz kusz — Crossbows**.
  **EN:** *Added support for creating **custom bows and crossbows**.*

  * **PL:** Własne modele 3D.
    **EN:** *Custom 3D models.*

  * **PL:** Wartości `CustomModelData`.
    **EN:** *`CustomModelData` values.*

  * **PL:** Niestandardowe tekstury.
    **EN:** *Custom textures.*

* **PL:** Dodano funkcję **automatycznej podmiany tekstury przedmiotu** dla wszystkich dodawanych modeli 3D, co znacząco upraszcza proces konfiguracji zasobów.
  **EN:** *Added **automatic item texture replacement** for all imported 3D models, significantly simplifying resource configuration.*

* **PL:** Dodano możliwość **przeciągania i upuszczania — Drag & Drop** obrazów bezpośrednio na stronę w celu szybszego przesyłania plików.
  **EN:** *Added support for **dragging and dropping images — Drag & Drop** directly onto the page for faster file uploads.*

* **PL:** Dodano obsługę **wklejania skopiowanych grafik i modeli 3D** bezpośrednio do aplikacji za pomocą skrótów systemowych, takich jak Ctrl+V.
  **EN:** *Added support for **pasting copied images and 3D models** directly into the application using system shortcuts such as Ctrl+V.*

### Zmieniono / Changed

* **PL:** Zaktualizowano identyfikację wizualną projektu.
  **EN:** *Updated the project's visual identity.*

  * **PL:** Zmieniono logo projektu na **NiceCode**.
    **EN:** *Changed the project logo to **NiceCode**.*

  * **PL:** Odświeżono branding aplikacji.
    **EN:** *Refreshed the application's branding.*

* **PL:** Zmieniono domyślną kolorystykę interfejsu z **Dark Black** na **Dark Aqua**, poprawiając czytelność i estetykę strony.
  **EN:** *Changed the default interface color scheme from **Dark Black** to **Dark Aqua**, improving readability and visual appearance.*

* **PL:** Przebudowano proces generowania paczek.
  **EN:** *Reworked the pack generation process.*

  * **PL:** Domyślnie wybraną opcją generowania jest teraz **Java Edition**.
    **EN:** ***Java Edition** is now selected as the default generation option.*

  * **PL:** Opcja **Geyser** nie jest już wybierana automatycznie podczas pierwszego uruchomienia.
    **EN:** *The **Geyser** option is no longer selected automatically on the first launch.*

### Ulepszono / Improved

* **PL:** Usprawniono proces dodawania modeli 3D i tekstur poprzez automatyzację konfiguracji zasobów.
  **EN:** *Improved the process of adding 3D models and textures by automating resource configuration.*

* **PL:** Zwiększono wygodę korzystania z aplikacji dzięki nowym metodom przesyłania plików: Drag & Drop oraz Clipboard Paste.
  **EN:** *Improved application usability with new file upload methods: Drag & Drop and Clipboard Paste.*

---

## [v0.1.3] - 2026-01-30

### Zmieniono / Changed

* **PL:** Całkowicie przebudowano interfejs użytkownika strony.
  **EN:** *Completely rebuilt the website's user interface.*

* **PL:** Zoptymalizowano pomniejsze elementy wizualne i funkcjonalne.
  **EN:** *Optimized various minor visual and functional elements.*

---

## [v0.1.2] - 2026-01-30

### Dodano / Added

* **PL:** Zaimplementowano animacje interfejsu użytkownika.
  **EN:** *Implemented user interface animations.*

* **PL:** Dodano wskaźnik statusu informujący o postępie procesu generowania paczki.
  **EN:** *Added a status indicator showing the progress of the pack generation process.*

* **PL:** Wprowadzono mechanizm automatycznego pobierania tekstur dla przedmiotów, których modele w nowszych wersjach gry nie wyświetlały się poprawnie — auto-fix.
  **EN:** *Introduced an automatic texture downloading mechanism for items whose models were not displayed correctly in newer game versions — auto-fix.*

* **PL:** Dodano bezpośredni odnośnik do repozytorium projektu w serwisie GitHub.
  **EN:** *Added a direct link to the project's GitHub repository.*

### Zmieniono / Changed

* **PL:** Zaktualizowano styl wizualny powiadomień systemowych.
  **EN:** *Updated the visual style of system notifications.*

* **PL:** Zmodyfikowano strukturę katalogów modeli wewnątrz generowanej paczki, aby zwiększyć kompatybilność.
  **EN:** *Modified the model directory structure inside generated packs to improve compatibility.*

### Naprawiono / Fixed

* **PL:** Naprawiono błąd uniemożliwiający poprawne generowanie paczek dla platformy Geyser.
  **EN:** *Fixed an issue that prevented packs from being generated correctly for the Geyser platform.*

---

## [v0.1.1] - 2026-01-22

### Dodano / Added

* **PL:** Dodano pełną obsługę tekstur bloków — Blocks — dla Minecraft Bedrock Edition.
  **EN:** *Added full support for block textures in Minecraft Bedrock Edition.*

* **PL:** Zaimplementowano obsługę pancerzy — Armor — dla Minecraft Bedrock Edition.
  **EN:** *Implemented armor support for Minecraft Bedrock Edition.*

* **PL:** Opracowano generator struktury plików `.json` oraz manifestów przeznaczonych dla wersji Bedrock.
  **EN:** *Developed a generator for `.json` file structures and manifests specific to Bedrock Edition.*

---

## [v0.1.0] - 2026-01-20

### Dodano / Added

* **PL:** **Pierwsze wydanie publiczne.**
  **EN:** ***Initial public release.***

* **PL:** Udostępniono konfigurator metadanych paczki, obejmujący nazwę, opis i ikonę.
  **EN:** *Introduced a pack metadata configurator covering the pack name, description, and icon.*

* **PL:** Zaimplementowano generowanie paczek dla następujących platform:
  **EN:** *Implemented pack generation for the following platforms:*

  * **PL:** Minecraft Java Edition.
    **EN:** *Minecraft Java Edition.*

  * **PL:** Minecraft Bedrock Edition.
    **EN:** *Minecraft Bedrock Edition.*

* **PL:** Dodano funkcję importowania tekstur przedmiotów — Items.
  **EN:** *Added support for importing item textures.*

* **PL:** Umożliwiono eksport gotowego projektu do pliku `.zip`.
  **EN:** *Added support for exporting a completed project as a `.zip` file.*

---

> **PL — Nota:** Projekt znajduje się w fazie **BETA**. Funkcjonalności mogą ulegać znaczącym zmianom w kolejnych wersjach bez zachowania kompatybilności wstecznej.
>
> **EN — Note:** *The project is currently in **BETA**. Features may change significantly in future releases without maintaining backward compatibility.*
