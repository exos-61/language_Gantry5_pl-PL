# Polish language for package Gantry5, Helium and Hydrogen templates

Spolszczenie pakietu Gantry 5, oraz darmowych szablonów Helium i Hydrogen.

Aby zainstalować polski pakiet językowy dla pakietu Gantry 5 zastosuj instalator Joomla z opcją **Instaluj z URL** i wklej poniższy adres URL:

`http://upgrade.dziadek.guide/gantry-5-lang/lang_joomla_gantry5_pl-PL.zip`

## Zastosowana terminologia

Ponieważ nazwy cząsteczki (particles) i atomy (atoms) w języku polskim nie kojarzą się z szablonami stron, przyjąłem nazewnictwo oparte na pojęciach pochodzących z Joomla.

* Particles - Moduły-G5
* Atoms - Wtyczki-G5
* Positions - Pozycje-G5

## Co zostało spolszczone?

Zostały spolszczone pliki językowe pakietu w lokalizacjach:

### Back-End

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

### Front-End

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

## Niedostępne pliki językowe .ini

Niestety pliki językowe **.ini** nie zawierają wszystkich wyrażeń użytych przy konfigurowaniu elementów Gantry 5. Elementy Moduły-G5, Wtyczki-G5 i Pozycje-G5 są dostępne tylko w języku angielskim. Aby je spolszczyć na chwilę obecną należałoby ingerować w pliki YAML i tłumaczyć każde pole osobno. Programiści RocketTheme zachęcają użytkowników do samodzielnego podjęcia się rozwiązania problemu. Chętnie podjąłbym się tego, ale nie będąc programistą nie wiem jak się do tego zabrać. Zacząłem tłumaczyć elementy gantry oparte na plikach YAML i stworzyłem sygnatury dla wyrażeń.

Bardzo dobrym przykładem jest rozwiązanie zastosowane przez programistów RocketTheme w kilku miejscach elementów pakietu. Moduł-G5 (Particle) składa się z dwóch plików: YAML i TWIG i w przypadku pliku menu.yaml (media/gantry5/engines/nucleus/particles) w sekcji **_info** i polu **content** zastosowano sygnaturę językową **GANTRY5_PARTICLE_MENU_INFO**, która pobiera zawartość wpisaną w pliku językowym **.ini**, a zastosowanie takich sygnatur w innych polach nie działa. Tu jest potrzebna wiedza programistyczna.

## Rozwiązanie tymczasowe

Na chwilę obecną postanowiłem tłumaczyć komendy i opisy w plikach YAML i instalować poprzez podmianę plików en-GB.yaml na pl-PL.yaml.

### Jakie pliki będą przetłumaczone?

Pliki YAML pakietu Gantry 5 znajdują się w katalogu Joomla **media/gantry5/engines/nucleus/** katalogach: **admin**, **blueprints** i **particles**.

#### Pliki yaml konfiguracji szablonu (blueprints)

Lokalizacja plików core:

`media/gantry5/engines/nucleus/admin`\
`media/gantry5/engines/nucleus/blueprints`

* media/gantry5/engines/nucleus/admin/blueprints/layout/inheritance/messages
  * default.yaml
  * empty.yaml
  * inherited
* media/gantry5/engines/nucleus/admin/blueprints/layout/inheritance
  * atom.yaml
  * offcanvas.yaml
  * particle.yaml
  * position.yaml
  * section.yaml
  * system.yaml
* media/gantry5/engines/nucleus/admin/blueprints/layout
  * block.yaml
  * container.yaml
  * offcanvas.yaml
  * section.yaml
* media/gantry5/engines/nucleus/admin/menu
  * block.yaml
* media/gantry5/engines/nucleus/admin/position
  * chrome
* media/gantry5/engines/nucleus/blueprints/page
  * assets.yaml
  * body.yaml
  * fontawesome.yaml
  * head.yaml


#### Pliki yaml konfiguracji Modułów-G5 (Particles), Wtyczek-G5 (Atoms) i Pozycji-g5 (Positions)

Lokalizacja plików core:

`media/gantry5/engines/nucleus/particles`

* analytics.yaml
* assets.yaml
* branding.yaml
* content.yaml
* contentarray.yaml
* copyright.yaml
* custom.yaml
* date.yaml
* frameworks.yaml
* lightcase.yaml
* logo.yaml
* menu.yaml
* messages.yaml
* mobile-menu.yaml
* module.yaml
* position.yaml
* social.yaml
* spacer.yaml
* totop.yaml


