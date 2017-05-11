# TrainCMS — system zarządzania treścią witryny internetowej

## keywords
cms, ruby on rails, calendar, comments, tags

## Autor
Kamil Pek, numer albumu 231050, [github.com/kamilpek](https://github.com/kamilpek)

## Streszczenie
W pracy przedstawiono wersję deweloperską systemu zarządzania treścią witryny internetowej „TrainCMS”. W trakcie pracy zaimplementowano publikowanie artykułów, kategoryzację, wyświetlanie listy kategorii na pasku nawigacji. Stworzono User Interface, który wyświetla wszystkie artykuły na stronie głównej, niezależnie od kategorii w kolejności malejącej od daty dodania oraz kalendarz wydarzeń. Do artykułów i wydarzeń w kalendarzu zaimplementowano możliwość załączania ilustracji oraz dodawania komentarzy.

Zaimplementowano panel administratora do zarządzania artykułami, kategoriami, komentarzami, tagami, użytkownikami i kalendarzem oraz do podglądu statystyk.

Do implementacji użyto technologie takie jak Ruby, Ruby on Rails, ZURB Foundation, jQuery Turbolinks, Plataformatec Devise, CarrierWave, RMagick, reCAPTCHA, CKEditor, Chartkick, Prawn.

Projekt wdrożono w serwisie, heroku.com i jest dostępny pod adresem: [https://traincms.herokuapp.com/](https://traincms.herokuapp.com/).

Kod źródłowy dostępny jest w serwisie github.com pod adresem: [https://github.com/kamilpek/traincms/](https://github.com/kamilpek/traincms/).

## Spis treści
1. Wprowadzenie
1. Wstęp i opis problemu
   1. Porównanie dostępnych rozwiązań z systemem TrainCMS
      1. Joomla
      1. WordPress
   1. Możliwości zastosowania praktycznego
      1. strona wizytówka
      1. internetowe portfolio
      1. serwis informacyjny
1. Projekt i analiza
   1. Diagram związków encji
   1. Diagram kontrolera danych
   1. Diagram przypadków użycia
   1. Projekt interfejsu użytkownika
      1. Panel Administratora
      1. Widok Redaktora
      1. Widok Gościa
1. Implementacja
   1. Architektura rozwiązania - Ruby on Rails
      1. Artykuły i Kategorie
      1. Komentarze
      1. Tagi
      1. Zakładki
      1. Strona Główna
      1. Kalendarz wydarzeń            
      1. Nawigacja
      1. Kanał RSS
   1. ZURB Foundation
      1. Instalacja
      1. Użycie
      1. Ikony
   1. CarrierWave, CKEditor, Cloudinary
      1. CKEditor i Cloudinary
      1. CarrierWave
   1. Prawn
   1. Chartkick
   1. reCAPTCHA
   1. deivse
   1. rQRcode i Prawn/QRCode
   1. geocoder
   1. cookies_eu
1. Bibliografia
1. Zakończenie
1. Spis rysunków
1. Spis kodów źródłowych
1. Oświadczenie

## Wstęp
Podczas kilkuletniej pracy z najpopularniejszymi aplikacjami w tej kategorii, takimi jak Joomla i WordPress nabyłem doświadczenie oraz swój pogląd na to jak ma wyglądać system zarządzania treścią (ang. __Content Managment System__, CMS). Naturalnym stało się więc stworzenie własnego systemu, przy okazji prezentując jak najszerszą część umiejętności nabytych w trakcie trwania studiów.

Istniejące systemy są często wybierane przez między innymi lokalne serwisy informacyjne, przedsiębiorstwa i instytucje, dlatego w swoim systemie zawarłem funkcjonalności, które na pewno przydadzą się różnym podmiotom w skutecznym zaistnieniu w Internecie.

Podczas tworzenia interfejsu użytkownika i administratora, kierowałem się głównie ergonomią użytkowania i przedstawieniem możliwości jakie prezentuje system w jak najbardziej przystępny sposób tak, aby początkujący użytkownik mógł poruszać się w sposób intuicyjny po aplikacji.

## Literatura
1. John Elder. Learn Ruby On Rails For Web Development: Learn Rails The Fast And Easy Way!. Codemy.com; 1 edition (January 19, 2015)
1. Dan Chak. Enterprise Rails. O’Reilly Media; 1 edition (November 3, 2008)
1. Użytkownicy Wikibooks. Ruby. Wikibooks; 1 edition (February 17, 2008)
1. Oficjalna dokumentacja frameworku Ruby on Rails. [guides.rubyonrails.org](http://guides.rubyonrails.org/)(dostęp 23.04.2017)
1. Oficjalny opis API Ruby on Rails. [api.rubyonrails.org](http://api.rubyonrails.org/)(dostęp 23.04.2017)
1. Oficjalna dokumentacja frameworku Foundation for Sites. [foundation.zurb.com/sites/docs](http://foundation.zurb.com/sites/docs/)(dostęp 23.04.2017)
1. Oficjalna dokumentacja Gemu Foundation Icon. [http://www.rubydoc.info/gems/foundation-icons-sass-rails/](http://www.rubydoc.info/gems/foundation-icons-sass-rails/)
1. Oficjalna dokumentacja Gemu CarrierWave [github.com/carrierwaveuploader/carrierwave/wiki](https://github.com/carrierwaveuploader/carrierwave/wiki)(dostęp 23.04.2017)
1. Oficjalna dokumentacja Gemu reCAPTCHA. [github.com/ambethia/recaptcha](https://github.com/ambethia/recaptcha)(dostęp 23.04.2017)
1. Oficjalna dokumentacja Gemu CKEditor for Rails. [github.com/galetahub/ckeditor](https://github.com/galetahub/ckeditor)(dostęp 23.04.2017)
1. Oficjalna dokumentacja Gemu Chartkick. [github.com/ankane/chartkick](https://github.com/ankane/chartkick)(dostęp 23.04.2017)
1. Oficjalna dokumentacja Gemu PrawnPDF. [prawnpdf.org/api-docs/2.0/](http://prawnpdf.org/api-docs/2.0/)(dostęp 23.04.2017)
1. Oficjalna dokumentacja - Gem devise. [github.com/plataformatec/devise/](https://github.com/plataformatec/devise/)(dostęp 23.04.2017)
1. Oficjalna dokumentacja - Gem rQRcode. [rubydoc.info/gems/rqrcode/](http://www.rubydoc.info/gems/rqrcode/)(dostęp 23.04.2017)
1. Oficjalna dokumentacja - Gem Prawn/QRCode. [rubydoc.info/gems/prawn-qrcode/](http://www.rubydoc.info/gems/prawn-qrcode/)(dostęp 23.04.2017)
1. Oficjalna dokumentacja - Gem Geocoder. [rubydoc.info/gems/geocoder/](http://www.rubydoc.info/gems/geocoder/)(dostęp 23.04.2017)
1. Oficjalna dokumentacja - Gem cookies_eu. [rubydoc.info/gems/cookies_eu/](http://www.rubydoc.info/gems/cookies_eu/(dostęp 23.04.2017)
