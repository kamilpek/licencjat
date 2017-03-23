# TrainCMS - System zarządzania treścią witryny internetowej

## keywords
cms, ruby on rails, calendar, comments, tags

## Autor
Kamil Pek, numer albumu 231050, [github.com/kamilpek](https://github.com/kamilpek)

## Wdrożenie
[traincms.herokuapp.com](http://traincms.herokuapp.com/)

## Kod aplikacji
[github.com/kamilpek/traincms](https://github.com/kamilpek/traincms)

## Streszczenie
W pracy przedstawiono wersję beta systemu zarządzania treścią witryny internetowej „TrainCMS”. W trakcie pracy zaimplementowano publikowanie artykułów, kategoryzację, wyświetlanie listy kategorii się pasku nawigacji na szczycie strony. Zaimplementowano klasyczny User Interface, który wyświetla wszystkie artykuły na stronie głównej, nie zależnie od kategorii w ustalonym porządku czyli malejąco od daty dodania, które można również komentować. Kolejną częścią User Interface jest kalendarz wydarzeń, kótre również możena komentować. Zarówno do artykułów jak i komentarzy zaimplementowano możliwość dodania ilustracji.
Po zalogowaniu się z uprawnieniami administratora zyskujemy dostęp do panelu administratora, w którym stworzono interfejs do zarządzania artykułami, kategoriami, komentarzami, tagami, użytkwonikami i kalendarzem. Udostępniono także podgląd statystyk.
Do implementacji użyto technologie takie jak Ruby, Ruby on Rails, ZURB Foundation, jQuery Turbolinks, Plataformatec Devise, CarrierWave, RMagick, reCAPTCHA, CKEditor, Chartkick, Prawn.

## Spis treści
1. Wstęp i opis problemu   
   - Porównanie dostępnych rozwiązań,
      - Joomla,
      - WordPress,
   - Możliwości zastosowania praktycznego,
      - strona wizytówka,
      - internetowe portfolio,
      - serwis informacyjny,
1. Projekt i analiza
   - Diagram klas,
   - Diagram modelu danych,
   - Projekt interfejsu użytkownika,
1. Implementacja
   - Architektura rozwiązania - Ruby on Rails
   - ZURB Foundation
   - CarrierWave
   - Prawn
1. Bibliografia
    - ksiązki,
    - artykuły w Internecie,
    - GitHub,

## Wstęp
Motywacją do napisania własnego systemu zarządzania treścią (ang. _Content Managment System_, CMS) było zaprezentowanie jak obszerniejszej części nabytych umiejętności podczas trwania studiów. Innym ważnym aspektem, który skłonił mnie do stworzenia akurat CMS’a jest wieloletnia praca na systemie Joomla. Takie systemy są często wybierane przez między innymi lokalne serwisy informacyjne, bądź różnego rodzaju firmy, dlatego w swoim systemie zawarłem wiele funkcjonalności, które na pewno przydadzą się różnym podmiotom i instytucjom w skutecznym zaistnieniu w Internecie. Korzystając już z utartych schematów, pojedynczy artykuł posiada dwa dodatkowe atrybuty takie jak aktywny i wyróżniony, które odpowiednio pozwalają na jego wyświetlanie i wyświetlanie w karuzeli obrazków na szczycie pod paskiem nawigacji. Do każdego artykułu możemy dodać tagi, które umożliwiają dodatkowe kategoryzowanie jak i łatwe wyszukiwanie interesujących nas treści.

## Literatura
1. [guides.rubyonrails.org](http://guides.rubyonrails.org/)
1. [api.rubyonrails.org](http://api.rubyonrails.org/)
1. [rubygems.org](https://rubygems.org/)
1. [foundation.zurb.com/sites/docs](http://foundation.zurb.com/sites/docs/)
1. [github.com/plataformatec/devise/wiki](https://github.com/plataformatec/devise/wiki)
1. [github.com/mislav/will_paginate](https://github.com/mislav/will_paginate)
1. [github.com/carrierwaveuploader/carrierwave/wiki](https://github.com/carrierwaveuploader/carrierwave/wiki)
1. [github.com/rmagick/rmagick](https://github.com/rmagick/rmagick)
1. [github.com/ambethia/recaptcha](https://github.com/ambethia/recaptcha)
1. [github.com/galetahub/ckeditor](https://github.com/galetahub/ckeditor)
1. [github.com/ankane/chartkick](https://github.com/ankane/chartkick)
1. [prawnpdf.org/api-docs/2.0/](http://prawnpdf.org/api-docs/2.0/)
