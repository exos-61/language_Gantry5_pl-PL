# Polish language for package Gantry5

Spolszczenie pakietu Gantry 5, wraz z darmowymi szablonami Helium i Hydrogen.

Aby zainstalować polski pakiet językowy dla pakietu Gantry 5 zastosuj instalator Joomla z opcją **Instaluj z URL** i wklej poniższy adres URL:

`http://upgrade.dziadek.guide/upgrade/gantry-5-lang/lang_joomla_gantry5_pl-PL.zip`

## Zastosowana terminologia

Ponieważ nazwy cząsteczki (particles) i atomy (atoms) w języku polskim nie kojarzą się z szablonami stron, przyjąłem nazewnictwo oparte na pojęciach pochodzących z Joomla.

* Particles - Moduły-G5
* Atoms - Wtyczki-G5
* Positions - Pozycje-G5

## Co zostało spolszczone?

Zostały spolszczone pliki językowe pakietu w lokalizacjach:

* Komponent
  `administrator/components/com_gantry5/language`

  * en-GB.com_gantry5.ini > pl-PL.com_gantry5.ini
  * en-GB.com_gantry5.sys.ini > pl-PL.com_gantry5.sys.ini

* Moduł Particle
 `modules/mod_gantry5_particle/language`

  * en-GB.mod_gantry5_particle.ini > pl-PL.mod_gantry5_particle.ini
  * en-GB.mod_gantry5_particle.sys.ini > pl-PL.mod_gantry5_particle.sys.ini

* Wtyczka Preset
  `plugins/gantry5/preset/language`

  * en-GB.plg_gantry5_preset.sys.ini > pl-PL.plg_gantry5_preset.sys.ini

* Wtyczka Quickicon
  `plugins/quickicon/gantry5/language`

  * en-GB.plg_quickicon_gantry5.sys.ini > pl-PL.plg_quickicon_gantry5.sys.ini

* Wtyczka systemowa
  `plugins/system/gantry5/language`

  * en-GB.plg_system_gantry5.sys.ini > pl-PL.plg_system_gantry5.sys.ini

* Wtyczka biblioteki
  `libraries/gantry5/language`

  * en-GB.lib_gantry5.sys.ini > pl-PL.lib_gantry5.sys.ini

* W site language
  `language`

  * en-GB.files_gantry5_nucleus.ini > pl-PL.files_gantry5_nucleus.ini
  * en-GB.files_gantry5_nucleus.sys.ini > pl-PL.files_gantry5_nucleus.sys.ini
  * en-GB.pkg_gantry5.sys.ini > pl-PL.pkg_gantry5.sys.ini

Niestety pliki językowe nie zawierają wszystkich wyrażeń użytych do konfiguracji elementów Gantry 5. Elementy Moduły-G5, Wtyczki-G5 i Pozycje-G5 są dostępne tylko w języku angielskim. Aby je spolszczyć na chwilę obecną należałoby ingerować w pliki YAML i tłumaczyć każdą pozycję osobno. Programiści RocketTheme zachęcają użytkowników do samodzielnego podjęcia się rozwiązania problemu. Chętnie podjąłbym się tego, ale nie będąc programistą nie wiem jak się do tego zabrać. Zacząłem tłumaczyć elementy gantry oparte na plikach YAML i stworzyłem sygnatury dla wyrażeń, może jakieś rozwiązanie znajdę.
