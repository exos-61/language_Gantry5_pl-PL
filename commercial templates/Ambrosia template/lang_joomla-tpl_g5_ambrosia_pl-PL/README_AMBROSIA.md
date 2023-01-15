# Polish language for Ambrosia templates

Spolszczenie komercyjnego szablonu Ambrosia dla Gantry 5.

Wszystkie przetłumaczone pakiety instalacyjne są dostępne w sekcji Releases

## Zastosowana terminologia

Ponieważ nazwy cząsteczki (particles) i atomy (atoms) w języku polskim nie kojarzą się z szablonami stron, przyjąłem nazewnictwo oparte na pojęciach pochodzących z Joomla.

* Particles - Moduły-G5
* Atoms - Wtyczki-G5
* Positions - Pozycje-G5

## Co zostało spolszczone w szablonie odnośnie plików .ini?

Zostały spolszczone pliki językowe pakietu w lokalizacjach:

* Templates

  `templates/rt_ambrosia/language`

  * en-GB.tpl_rt_ambrosia.ini > pl-PL.tpl_rt_ambrosia.ini
  * en-GB.tpl_rt_ambrosia.sys.ini > pl-PL.tpl_rt_ambrosia.sys.ini

## Niedostępne tłumaczenia plików yaml

Niestety pliki językowe **.ini** nie zawierają wszystkich wyrażeń użytych przy konfigurowaniu elementów szablonu i Gantry 5. Elementy Moduły-G5, Wtyczki-G5 i Pozycje-G5 są dostępne tylko w języku angielskim i wymagają przetłumaczenia plików konfiguracyjnych .yaml.

Zgodnie z [dokumentacją](https://docs.gantry.org/gantry5/advanced/customizing-theme-files#theme-directory-matrix) katalog **custom** w lokalizacji *templates/Twój_szablon* służy do nadpisywania wszystkich plików znajdujących się w *administrator/components/com_gantry5* w katalogu **admin**, *media/gantry5/engines/nucleus* w katalogu **engine** oraz pliki szablonu zgodnie z nazwą i hierarchią katalogów. Aby pakiet Gantry 5 był całkowicie przetłumaczony pliki yaml muszą być zainstalowane lub wklejone do katalogu custom szablonu w wymienionych katalogach.

Ten pakiet językowy zainstaluje pliki językowe .ini, przetłumaczone pliki yaml i twig, szablonu Ambrosia oraz pakietu Gantry 5.

### Jakie pliki yaml i twig szablonu zostały przetłumaczone i dorzucone?

**templates**

* templates/rt_ambrosia/admin/templates/pages
  * about.html.twig - *Opis szablonu w oknie otwieranym przyciskiem About*

**blueprints**

* templates/rt_ambrosia/blueprints/styles
  * above.yaml - *Style dla prawej kolumny*
  * accent.yaml - *Style kolorów akcentujących.*
  * base.yaml - *Style kolorów podstawowych*
  * bottom.yaml - *Style sekcji Bottom*
  * breakpoints.yaml - *Ustawienia przerwań dla urządzeń wyświetlających*
  * copyright.yaml - *Style sekcji Copyright*
  * extension.yaml - *Style sekcji Extension*
  * feature.yaml - *Style sekcji Feature*
  * font.yaml - *Ustawianie czcionek*
  * footer.yaml - *Style sekcji Footer*
  * header.yaml - *Style sekcji Header*
  * main.yaml - *Style sekcji Main*
  * menu.yaml - *Style menu*
  * navigation.yaml - *Style sekcji Navigation*
  * offcanvas.yaml - *Style sekcji Offcanvas*
  * slideshow.yaml - *Style sekcji Slideshow*
  * top.yaml - *Style sekcji Top*

* templates/rt_ambrosia/gantry
  * theme_modyfikuj.yaml - *Wzór instalacji dodatkowej czcionki Lato*

* templates/rt_ambrosia/layouts
  * _error.yaml - *Układ strony błędów z skonfigurowanymi elementami*
  * _offline.yaml - *Układ strony informacyjnej dla wyłączonej witryny*
  * coming_son.yaml - *Wzór strony zapowiedzi*
  * home.yaml - *Układ strony frontowej z skonfigurowanymi elementami*

* templates/rt_ambrosia/particles
  * aos.yaml - *Wtyczka-G5 (Atom) - Dodaje animacje podczas przewijania*
  * audioplayer.yaml - *Moduł-G5 (Particle) - Odtwarzanie muzyki poprzez interfejs odtwarzacza audio.*
  * blockcontent.yaml - *Moduł-G5 (Particle) - Wyświetla zawartość bloku*
  * calendar.yaml - *Moduł-G5 (Particle) - Kalendarz do wyświetlania dat.*
  * cookie-consent.yaml - *Wtyczka-G5 (Atom) - Wyświetla komunikat zgody na stosowanie cookies.*
  * cookie-consent.html.twig - *Wtyczka darmowa z [Inspire Theme](https://www.inspiretheme.com/documentation/gantry5-particles/cookie-consent)*
  * contact.yaml - *Moduł-G5 (Particle) - Wyświetla kontakt.*
  * contentlist.yaml - *Moduł-G5 (Particle) - Wyświetla listę zawartości.*
  * contenttabs.yaml - *Moduł-G5 (Particle) - Wyświetla karty treści.*
  * featuresslider.yaml - *Moduł-G5 (Particle) - Wyświetlanie suwaka z funkcjami.*
  * fixedheader.yaml - *Wtyczka-G5 (Atom) - Dodaje stały nagłówek do swojej strony.*
  * googlemap.yaml - *Moduł-G5 (Particle) - umożliwia wstawianie na stronę bloku z lokalizacją np. Twojej firmy w mapach Google*
  * googlemap.html.twig - *Wtyczka darmowa z [Inspire Theme](https://www.inspiretheme.com/documentation/gantry5-particles/google-maps)*
  * headlines.yaml - *Moduł-G5 (Particle) - Wyświetla nagłówki.*
  * horizontalmenu.yaml - *Moduł-G5 (Particle) - Wyświetlanie menu poziomego.*
  * imagegrid.yaml - *Moduł-G5 (Particle) - Wyświetlanie siatki zdjęć.*
  * infolist.yaml - *Moduł-G5 (Particle) - Wyświetla listę informacji*
  * lists.yaml - *Moduł-G5 (Particle) - Wyświetlanie list.*
  * logo.yaml - *Moduł-G5 (Particle) - Wyświetlanie logo.*
  * newsletter.yaml - *Moduł-G5 (Particle) - Wyświetla formularz newslettera.*
  * promoimage.yaml - *Moduł-G5 (Particle) - Wyświetla obrazek promocyjny.*
  * simplecounter.yaml - *Moduł-G5 (Particle) - Wyświetla prosty licznik.*
  * social.yaml - *Moduł-G5 (Particle) - Wyświetla przyciski społecznościowe.*
  * stripsslider.yaml - *Moduł-G5 (Particle) - Suwak do wyświetlania pasków.*
  * swiper.yaml - *Moduł-G5 (Particle) - Karuzela JS*
  * tabimage.yaml - *Moduł-G5 (Particle) - Wyświetlanie obrazów w kartach.*
  * video.yaml - *Moduł-G5 (Particle) - Osadza filmy z serwisów YouTube, Vimeo, lokalnych lub zewnętrznych adresów URL.*

* templates/rt_ambrosia/scss
  * custom.scss - *Doinstalowanie czcionek*
    * Allura - 	*Kaligraficzna , ekspozycyjna , elegancka, formalna , zaproszenia*
    * Italiano - *Kaligraficzna , Kursywa , Wyświetlaczowa , Elegancka , Formalna*
    * Lato - *Współczesna, Nagłówki, Akapity, Groteska, Humanista, Kursywa, Bolt, Heavy, Light, Sans, Ultra Light*
    * Promocyjna - *Kaligraficzna , Swobodna , Kręcona , Ekspozycyjna , Elegancka , Ślubna , Szeroka*
    * Rubik Moonrock - *Ozdobna, Okazjonalna*

### Dodatkowa treść poza projektem

Dla przetłumaczonych plików konfiguracyjnych .yaml dodałem sygnatury językowe dla których treść znajduje się w głównym pliku językowym  **pl-PL.com_gantry5.ini** na końcu arkusza. Sygnatury umieściłem w **_info** i **_alert** plików yaml.

Dodatkowe darmowe Wtyczki-G i Moduły-G5

* Cookie Consent - *Zgoda na ciasteczka* [Inspire Theme](https://www.inspiretheme.com/downloads/freebies/cookie-consent-atom)

