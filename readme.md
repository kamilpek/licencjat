# TrainCMS — System zarządzania treścią witryny internetowej

## keywords
cms, ruby on rails, calendar, comments, tags

## Autor
Kamil Pek, numer albumu 231050, [github.com/kamilpek](https://github.com/kamilpek)

## Wdrożenie
[traincms.herokuapp.com](http://traincms.herokuapp.com/)

## Kod aplikacji
[github.com/kamilpek/traincms](https://github.com/kamilpek/traincms)

## Streszczenie
W pracy przedstawiono wersję beta systemu zarządzania treścią witryny internetowej „TrainCMS”. W trakcie pracy zaimplementowano publikowanie artykułów, kategoryzację, wyświetlanie listy kategorii na pasku nawigacji. Stworzono User Interface, który wyświetla wszystkie artykuły na stronie głównej, niezależnie od kategorii w kolejności malejącej od daty dodania oraz kalendarz wydarzeń. Do artykułów i wydarzeń w kalendarzu zaimplementowano możliwość załączania ilustracji oraz dodawania komentarzy.

Zaimplementowano panel administratora do zarządzania artykułami, kategoriami, komentarzami, tagami, użytkownikami i kalendarzem oraz do podglądu statystyk.

Do implementacji użyto technologie takie jak Ruby, Ruby on Rails, ZURB Foundation, jQuery Turbolinks, Plataformatec Devise, CarrierWave, RMagick, reCAPTCHA, CKEditor, Chartkick, Prawn.

## Spis treści
1. Wstęp i opis problemu   
   1. Porównanie dostępnych rozwiązań,
      1. Joomla,
      1. WordPress,
   1. Możliwości zastosowania praktycznego,
      1. strona wizytówka,
      1. internetowe portfolio,
      1. serwis informacyjny,
1. Projekt i analiza
   1. Diagram klas,
   1. Diagram modelu danych,
   1. Projekt interfejsu użytkownika,
1. Implementacja
   1. Architektura rozwiązania - Ruby on Rails
   1. ZURB Foundation
   1. CarrierWave
   1. Prawn
1. Bibliografia
    1. książki
    1. artykuły w Internecie
    1. materiały dostępne na GitHub.com

## Wstęp
Podczas kilkuletniej pracy z najpopularniejszymi aplikacjami w tej kategorii, takimi jak Joomla i WordPress nabyłem doświadczenie oraz swój pogląd na to jak ma wyglądać system zarządzania treścią (ang. _Content Managment System_, CMS). Naturalnym stało się więc stworzenie własnego systemu, przy okazji prezentując jak najszerszą część umiejętności nabytych w trakcie trwania studiów.

Istniejące systemy są często wybierane przez między innymi lokalne serwisy informacyjne, przedsiębiorstwa i instytucje, dlatego w swoim systemie zawarłem funkcjonalności, które na pewno przydadzą się różnym podmiotom w skutecznym zaistnieniu w Internecie.

Podczas tworzenia interfejsu użytkownika i administratora, kierowałem się głównie ergonomią użytkowania i przedstawieniem możliwości jakie prezentuje system w jak najbardziej przystępny sposób tak, aby początkujący użytkownik mógł poruszać się w sposób intuicyjny po aplikacji.

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
