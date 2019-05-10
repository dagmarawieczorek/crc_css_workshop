# CSS i HTML Workshop - podstawy

Zadaniem jest edycja i ostylowanie panelu studenta.
Strona jest podzielona na 4 podstrony. Wszystkie podstrony mają ten sam header i boczną nawigacje.
Globalny styl, który jest podpięty do wszystkich podstron znajduje się w pliku styles.css.
Podstrony to: 
- index.html - czyli inaczej strona główna. W kontenerze o klasie content znajduje się kalendarz. 
-  list.html, news.html, mail.html
  
Edycje i stylizowanie plików list, news i mail potraktuj jako zadanie dodatkowe. Zadanie 1 i 2 wykonuj w pliku index.html.

## Zadanie 1. Navigacja
Zmień i ostyluj :
- top-header: 
  składa się z dwóch kontenerów: uniwersity-container i user container.
  top-header jako rodzic otrzymał display: flex a jego dzieci powinny być ustawione na przez justify-content tak, żeby między nimi była odpowiednia przestrzeń
  (justify-content , https://css-tricks.com/snippets/css/a-guide-to-flexbox/).
  Obrazek użytkownika i uniwersytetu jest placeholderem, trzeba go poprawnie ostylować - aby uzyskać koło, ustawiamy border-radius: 50%;
  Należy ostylować i ustawić nazwy do tych części headera (ustawić np. przy użyciu display: flex dla kontenerów i użyć flex-direction)), dodać ikonkę strzałki w dół przy użytkowniku, zmienić kolor tła, ustawić paddingi i marginy.
  
       (Ikony są już zaimportowane jako font w sekcji html <head>. Są to ikony z material.io i ich pełna lista znajduje się pod adresem: https://material.io/tools/icons/?icon=drafts&style=baseline )
- hamburger : jest niekompletny, ma nieodpowiedni kolor, nie jest wyśrodkowany.
- left-navbar : zamiast nazw powinny być ikony. Rozmieść je przy użyciu flexboxa, zmień paddingi i kolory.


 ## Zadanie 2. Kalendarz
 Kalendarz w tym wypadku jest sztywno napisanym komponentem - wszystkie daty i wydarzenia możemy ręcznie modyfikować w pliku HTML. 
Timeline jest komponentem, który składa się z listy **(ul - unordered list)** elementów **(li - list item)** z godzinami.

**ul** w divie o klasie events składa się z pojedynczych **events-group**. 

Każdy events-group to dzień tygodnia i znajdują się w nim zajęcia **single-event**. Możesz swobodnie dodawać i modyfikować początek i koniec zajęć, a także dodawać nowe poprzez kopiowanie li i zmienianie ich położenia w tygodniu oraz tekstów, godzin i styli.

    Bloki godzinowe są ustawiane za pomocą jQuery(biblioteka do JavaScript) poprzez pobieranie atrybutów data-start i data-end z pliku HTML, który znajduje się w pliku calendar.js i jest poza zakresem tego workshopu.
    Interesuje nas to, że dzięki temu możemy ustawiać im godziny oraz przypisywać konkretne klasy dla różnego rodzaju zajęć, np: data-event="event-3". 
Klasy **event-1**, **event-2** i **event-3** są klasami, które możesz znaleźć w pliku **calendar.css**. Poprzez nadawanie eventowi jednej z nich możesz uzyskać ujednolicone style dla tego samego rodzaju elementu.

- Ostyluj, zmodyfikuj, dodaj i usuń kilka zajęć, dodaj również do nich prowadzących (zobacz klasę **lecturer** w styles.css i index.html).

- Ostyluj górną nawigację kalendarza **calendar-header** i jego dzieci, calendar-title, calendar-month i calendar-type

##  ☆ Podstrony
    
Jeśli zrobiłeś wczesniejsze zadania, możesz przejść do modyfikacji podstron. 
Nawigacja jest linkowana poprzez znacznik html <**a** href="news.html"> i po kliknięciu zostajesz przeniesiony do pliku news.html. 
Jak widzisz wszystkie zmiany w pliku styles.css są również widoczne na wszystkich podstronach, ponieważ jest podpięty ten sam plik ze stylami, a elementy mają te same klasy.
Nie są widoczne zmiany, które zostały zrobione w index.html w top-headerze, left-navbarze czy hamburgerze, ponieważ HTML w tych plikach podstron nie był modyfikowany, możesz te elementy przekopiować.
Stwórz i zmodyfikuj dowolnie zawartość podstron.
