# Polish language for Hydrogen templates

Spolszczenie darmowego szablonu Hydrogen dla Gantry 5.

Wszystkie przetłumaczone pakiety instalacyjne są dostępne w sekcji Releases

## Zastosowana terminologia

Ponieważ nazwy cząsteczki (particles) i atomy (atoms) w języku polskim nie kojarzą się z szablonami stron, przyjąłem nazewnictwo oparte na pojęciach pochodzących z Joomla.

* Particles - Moduły-G5
* Atoms - Wtyczki-G5
* Positions - Pozycje-G5

## Co zostało spolszczone w szablonie odnośnie plików .ini?

Zostały spolszczone pliki językowe pakietu w lokalizacjach:

* Templates

  `templates/g5_hydrogen/language`

  * en-GB.tpl_g5_hydrogen.ini > pl-PL.tpl_g5_hydrogen.ini
  * en-GB.tpl_g5_hydrogen.sys.ini > pl-PL.tpl_g5_hydrogen.sys.ini

## Niedostępne tłumaczenia plików yaml

Niestety pliki językowe **.ini** nie zawierają wszystkich wyrażeń użytych przy konfigurowaniu elementów szablonu i Gantry 5. Elementy Moduły-G5, Wtyczki-G5 i Pozycje-G5 są dostępne tylko w języku angielskim i wymagają przetłumaczenia plików konfiguracyjnych .yaml.

Zgodnie z [dokumentacją](https://docs.gantry.org/gantry5/advanced/customizing-theme-files#theme-directory-matrix) katalog **custom** w lokalizacji *templates/Twój_szablon* służy do nadpisywania wszystkich plików znajdujących się w *administrator/components/com_gantry5* w katalogu **admin**, *media/gantry5/engines/nucleus* w katalogu **engine** oraz pliki szablonu zgodnie z nazwą i hierarchią katalogów. Aby pakiet Gantry 5 był całkowicie przetłumaczony pliki yaml muszą być zainstalowane lub wklejone do katalogu custom szablonu w wymienionych katalogach.

Ten pakiet językowy zainstaluje pliki językowe .ini, przetłumaczone pliki yaml szablonu Hydrogen i pakietu Gantry 5.

### Jakie pliki yaml szablonu zostały przetłumaczone?

**templates**

* templates/g5_hydrogen/admin/templates/ajax
  * icons.html.twig - *Komunikat w oknie dodawania czcionki awesome*
  * outline-new.html.twig - *Okno tworzenia nowego szablonu*
* admin/templates/pages
  * about.html.twig - *Opis szablonu w oknie otwieranym przyciskiem About*

**blueprints**

* templates/g5_hydrogen/blueprints
  * page.yaml - *Zakładka Blok (Block).*
* templates/g5_hydrogen/blueprints/style
  * accent.yaml - *Style kolorów akcentujących.*
  * base.yaml - *Style kolorów podstawowych*
  * breakpoints.yaml - *Ustawienia przerwań dla urządzeń wyświetlających*
  * feature.yaml - *Style sekcji Feature*
  * footer.yaml - *Style sekcji Footer*
  * header.yaml - *Style sekcji Header*
  * main.yaml - *Style sekcji Main*
  * menu.yaml - *Style menu*
  * navigation.yaml - *Style sekcji Navigation*
  * offcanvas.yaml - *Style sekcji Offcanvas*
  * showcase.yaml - *Style sekcji Showcase*
  * subfeature.yaml - *Style sekcji Subfeature*

* templates/g5_hydrogen/layouts
  * home.yaml - *Układ strony frontowej z skonfigurowanymi elementami*

* media/gantry5/engines/nucleus/particles
  * sample.yaml - *Przykładowa treść umieszczona w Module-G5 umożliwiającym prezentację kontentu strony*

### Dodatkowa treść poza projektem

Do przetłumaczonych plików konfiguracyjnych .yaml dodałem sygnatury językowe dla których treść znajduje się w głównym pliku językowym  **pl-PL.com_gantry5.ini** na końcu arkusza. Sygnatury umieściłem w **_info** i **_alert** plików yaml.
