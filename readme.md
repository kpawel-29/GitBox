osoby w zespole:
- 1) Gafka Dariusz
- 2) Józwiak Roman
- 3) Kadłubowski Paweł
- 4) Korszuń Kacper

Projekt strony mikroblogowej z addonami + aplikacja desktopowa.

Podział zadań na 1 tydzień (opisy, funkcjonalność i diagramy*): 

Jeżeli chodzi o stronę to: 
->1 - wyszukiwarka, panel administratora.
->2 - profil użytkownika (umieszczenie addonów i reszta).
->3 - rejestracja i zalogowanie (łącznie z tym jak to można zabezpieczyć).
->4 - strona główna, edycja użytkownik.

Opis modułów: 
->1 - wirtualny dysk,
->2 - youtube?
->3 - blog,
->4 - wymyśl i opisz! dobre ma być.
 
* - opcjonalne, może być demo rysunek na kartce.

Aplikacja desktopowa: 
(następny tydzień)

Opis dla Wyszukiwarki, Panelu Administratora @Darek
Moduł “Wyszukiwarki” Opis: Wyszukiwarka ma za zadania przetworzyć zapytania na jak najlepsze wyniki. Po znalezioniu rekordów, które odpowiadają zapytaniu, zwrócić top 10 najbliższych.
Funkcjonalość: Wyszukiwanie będzie odbywało się na podstawie modułów. Przy przejściu w zakładkę “Wyszukaj”, ujawnią się nam podane niżej opcje:
•	Typ [blog, wirtualny dysk, użytkownik]
•	Tekst do wyszukania Jeśli typ, będzie równy blogowi, to zostanie wyświetlone:
•	Typ Bloga: [sportowy, moda, kulinaria, zdrowie, film, muzyka, technologia] Jeśli zas, bedzie on równy wirtualnemu dyskowi, to:
•	Typ Plików: [pliki obrazkowe, pliki video, pliki tekstowe]
•	W przeciwnym wypadku, jeśli będzie to użytkownik. Nie wyświetlaj nic.
Zabezpiecznia: Przetworzenie zapytania I sprawdzenie, czy nie zawiera potencjalnego zagrożenia. Jesli tak uciec od tagów, aby uniknąć uszkodzenia systemu.
Panel Administratora: Opis: Panel administratora będzie miał za zadanie wspomóc administratora w codzienniej pracy, aby cześć problemów mogła być przetworzona za pomocą strony, bez bawienia się w zmienianie kodu źródłowego.
Funkcjonalość: Panel administratora, bedzie panelem do obługi aplikacji webowej z poziomu frontu. Panel będzie zawierał:
•	”Użytkownicy” - będzie można przejrzeć tutaj wszystkich zarejestrowanych użytkowników oraz zarządzać nimi. (Nadać/Usunąć uprawnienia, zbanować/odbanować, przejrzeć podstawowe informacje takie jak: do kiedy zbanowany, od kiedy zarejestrowany)
•	”Strona” - będzie można tutaj zmienić/dodać newsy, dla głównej strony manualnie.
•	”Blokowanie IP” - zablokowanie podanego ip, przed przeglądaniem strony
•	”Statystyki” - Statystyki strony.
Zabezpieczenia: Automatyczny redirect na stronę główną jeśli, użytkownik nie jest administratorem. Odnotowanie takiej próby zalogowania w logach.
Addon Wirtualny Dysk @Darek: Wirtualny Dysk:
Opis: Wirtualny dysk, będzie pozwałał na przechowywanie danych na swoim własnym profilu.
Funkcjonalość: Wirtualny dysk, zawierać będzie kategorie dla przetrzymywanych danych. Nie będzie możliwości przeplatania tych samych kategorii w jednym folderze. Każda kategoria będzie musiała zawierać swój folder. Kategorie:
•	Pliki obrazkowe: [.jpg, .gif, .img, .png]
•	Pliki video && muzyczne: [.avi, .mp4, .mpg, .mp3]
•	Pliki tekstowe [.doc, .txt, I inne] Autorzy serwisu nie będą odpowiadali za materiały dodawane przez użytkowników. Jeśli jednak zostanie zgłoszone naruszenie praw autorskich będą zmuszeni usunąć dany materiał z profilu użytkownika I nagrodzić go 24 godzinnym banem.
Zabezpieczenia: Przed potencjalnym wrzuceniem niewłaściwych formatów na stronę. Wyrażenia regularne przystosowane dla danych kategorii będą sprawdzać, czy dany materiał jest właściwy.

