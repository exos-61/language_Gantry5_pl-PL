# Polish language for Gantry5 package and RocketTheme templates

Spolszczenie pakietu Gantry 5, darmowych szablonów Helium i Hydrogen oraz szablonów komercyjnych.

Wszystkie przetłumaczone pakiety instalacyjne są dostępne w sekcji Releases

## Zastosowana terminologia

Ponieważ nazwy cząsteczki (particles) i atomy (atoms) w języku polskim nie kojarzą się z szablonami stron, przyjąłem nazewnictwo oparte na pojęciach pochodzących z Joomla.

* Particles - Moduły-G5
* Atoms - Wtyczki-G5
* Positions - Pozycje-G5

## Co zostało spolszczone w pakiecie Gantry 5 odnośnie plików .ini?

Zostały spolszczone pliki językowe pakietu w lokalizacjach:

* Komponent

  `administrator/components/com_gantry5/language`

  * en-GB.com_gantry5.ini > pl-PL.com_gantry5.ini
  * en-GB.com_gantry5.sys.ini > pl-PL.com_gantry5.sys.ini

* Wtyczka Preset

  `plugins/gantry5/preset/language`

  * en-GB.plg_gantry5_preset.sys.ini > pl-PL.plg_gantry5_preset.sys.ini

* Wtyczka Quickicon

  `plugins/quickicon/gantry5/language`

  * en-GB.plg_quickicon_gantry5.sys.ini > pl-PL.plg_quickicon_gantry5.sys.ini

* Wtyczka systemowa

  `plugins/system/gantry5/language`

  * en-GB.plg_system_gantry5.sys.ini > pl-PL.plg_system_gantry5.sys.ini

* Moduł Particle

 `modules/mod_gantry5_particle/language`

  * en-GB.mod_gantry5_particle.ini > pl-PL.mod_gantry5_particle.ini
  * en-GB.mod_gantry5_particle.sys.ini > pl-PL.mod_gantry5_particle.sys.ini

* Wtyczka biblioteki

  `libraries/gantry5/language`

  * en-GB.lib_gantry5.sys.ini > pl-PL.lib_gantry5.sys.ini

* W site language

  `language`

  * en-GB.files_gantry5_nucleus.ini > pl-PL.files_gantry5_nucleus.ini
  * en-GB.files_gantry5_nucleus.sys.ini > pl-PL.files_gantry5_nucleus.sys.ini
  * en-GB.pkg_gantry5.sys.ini > pl-PL.pkg_gantry5.sys.ini

## Niedostępne tłumaczenia plików yaml

Niestety pliki językowe **.ini** nie zawierają wszystkich wyrażeń użytych przy konfigurowaniu elementów Gantry 5. Elementy Moduły-G5, Wtyczki-G5 i Pozycje-G5 są dostępne tylko w języku angielskim i wymagają przetłumaczenia plików konfiguracyjnych .yaml.

Zgodnie z [dokumentacją](https://docs.gantry.org/gantry5/advanced/customizing-theme-files#theme-directory-matrix) katalog **custom** w lokalizacji *templates/Twój_szablon* służy do nadpisywania wszystkich plików znajdujących się w *administrator/components/com_gantry5* w pliku **admin**, *media/gantry5/engines/nucleus* w pliku **engine** oraz pliki szablonu zgodnie z hierarchią katalogów. Aby pakiet Gantry 5 był całkowicie przetłumaczony pliki yaml muszą być zainstalowane w wymienionych lokalizacjach szablonu. Jeżeli Twój szablon nie został jeszcze przetłumaczony to pobierz jakikolwiek z dostępnych, rozpakuj na komputerze i przy pomocy FTP wrzuć katalogi **admin** i **engine** do katalogu custom Twojego szablonu co spowoduje że pakiet Gantry 5 będzie całościowo przetłumaczony. W razie problemów wystarczy pliki usunąć. Baw sie dobrze i Twórz niesamowite strony, bo teraz masz taką możliwość bez znajomości kodowania.

### Jakie pliki yaml zostały przetłumaczone?

**admin**

* administrator/components/com_gantry5/blueprints/gantry/theme
  * configuration.yaml
  * details.yaml
* administrator/components/com_gantry5/blueprints/menu
  * menu.yaml - *ustawienia menu, koło zębate na prawo.*
  * menuitem.yaml - *ustawienia elementu menu*

**engine**

* media/gantry5/engines/nucleus/admin/blueprints/layout
  * block.yaml - *Zakładka Blok (Block)*
  * container.yaml - *Zakładka Kontener (Container)*
  * offcanvas.yaml - *Zakładka Offcanvas*
  * section - *zakładka Sekcja (Section)*
* media/gantry5/engines/nucleus/admin/blueprints/layout/inheritance
  * atom.yaml - *Zakładka Dziedziczenie Wtyczka-G5*
  * offcanvas.yaml - *Zakładka Dziedziczenie sekcja Offcanvas*
  * particle.yaml - *Zakładka Dziedziczenie Moduł-G5*
  * position.yaml - *Zakładka Dziedziczenie Pozycja-G5*
  * section.yaml - *Zakładka Dziedziczenie Sekcja*
  * system.yaml - *Zakładka Dziedziczenie Komunikat systemu*
* media/gantry5/engines/nucleus/admin/blueprints/layout/inheritance/messages
  * default.yaml - *Komunikat informuje że element może być dziedziczony z szablonu bazowego*
  * empty.yaml - *Komunikat w przypadku braku podobnych elementów do dziedziczenia*
  * inherited.yaml - *Komunikat informuje które szablony dziedziczą dany element*
* media/gantry5/engines/nucleus/admin/blueprints/menu
  * block.yaml - *Zakładka Blok w menu blokowym z Modułami-G5. Układ (Layout) bloku.*
* media/gantry5/engines/nucleus/admin/blueprints/position
  * chrome.yaml
* media/gantry5/engines/nucleus/blueprints/page
  * assets.yaml - *Ustawienia strony - Assets - dodatkowe zasoby*
  * body.yaml - *Ustawienia strony - Atrybuty sekcji body*
  * fontawesome - *Ustawienia strony - Ustawienia Font Awesome*
  * head - *Ustawienia strony - Właściwości sekcji Head*
* media/gantry5/engines/nucleus/particles
  * analytics.yaml - *Wtyczka-G5 (Atom) - Konfiguracja Google Analytics.*
  * assets.yaml - *Wtyczka-G5 (Atom) - Konfiguracja niestandardowego CSS i Javascript.*
  * branding.yaml - **Moduł-G5 (Particle) - Konfiguracja informacji branżowych*
  * content.yaml - *Pozycja-G5 (Particle) - Wyświetlanie zawartości strony w określonym położeniu w układzie strony.*
  * contentarray.yaml - *Moduł-G5 (Particle) -*
  * copyright.yaml - *Moduł-G5 (Particle) - Wyświetlanie informacji o prawach autorskich.*
  * custom.yaml - *Moduł-G5 (Particle) - Wyświetla niestandardowy blok HTML.*
  * date.yaml - *Moduł-G5 (Particle) - Wyświetla datę*
  * frameworks.yaml - *Wtyczka-G5 (Atom) - Ładuje wybrane frameworki na stronę.*
  * lightcase.yaml - *Wtyczka-G5 (Atom) - Elastyczna i responsywna wtyczka Lightbox.*
  * logo.yaml - *Moduł-G5 (Particle) - Wyświetla logo strony*
  * menu.yaml - *Moduł-G5 (Particle) - Menu Gantry*
  * messages.yaml - *Pozycja-G5 (Particle) - Wyświetlanie komunikatów systemowych.*
  * mobile-menu.yaml - *Moduł-G5 (Particle) - Renderuje kontener menu mobilnego dla sekcji offcanvas. Mobile Menu*
  * module.yaml - *Pozycja-G5 (Particle) - Wyświetlanie Modułów-G5 i Joomla w określonym położeniu w układzie strony. Module Instance (Instancja modułu).*
  * position.yaml - *Pozycja-G5 (Particle) - Pozycje do umieszczania modułów w Joomla.*
  * social.yaml - *Moduł-G5 (Particle) - Wyświetla przyciski społecznościowe.*
  * spacer.yaml - *Pozycja-G5 (Particle) - Dodaje pustą kolumnę do wiersza.*
  * totop.yaml - *Moduł-G5 (Particle) - Umożliwia powrót na górę strony.*
