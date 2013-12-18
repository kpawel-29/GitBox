[&#8810;](../README.md) spis treści

Opis modułów: rejestracja i zalogowanie

Sekcja logowania na stonie:
Użytkownik nie zalogowany widzi na stronie przycisk „zaloguj” i „zarejestruj”. Użytkownik zalogowany widzi przycisk „wyloguj”. 
Opis rejestracji: 
Użytkownik musi podać
- nick – musi być unikatowy, składać się tylko z liter i cyfr bez polskich znaków, nie może powtarzać się w bazie danych. Jeżeli zostanie podany użyty wcześniej nick – zostanie wyświetlony komunikat „nick jest niedozwolony lub zajęty”. Jeżeli wprowadzony nick będzie dostępny – wyświetli się napis „podany nick jest dostępny”.

- adres e-mail – podany adres służy do kontaktu od strony administratora, nie jest wyświetlany publicznie innym użytkownikom.
- hasło – długość hasła od 5 do 14 cyfr, może zawierać tylko litery i cyfry.
- powtórz hasło – użytkownik podaje hasło ponownie, a funkcja sprawdza czy podane hasła są identyczne.
- odpowiedź na proste pytanie, wybierane losowo z bazy danych z tabeli pytań zabezpieczających. Są to pytania typu „ile to jest 2+2?”, „co jest stolicą Polski?” itp. Ma to na celu weryfikację czy formularz ma do czynienia z osobą czy z botem / automatem.
- akceptacja regulaminu – pod formularzem jest wyświetlany regulamin serwisu, użytkownik zakładający konto musi zaznaczyć checkbox „Oświadczam, że zapoznałem się i akceptuję treść regulaminu”.
Wszystkie pola są wymagane.

Opis logowania: 
Formularz logowania zawiera 2 pola: nick i hasło. Pod nim znajduje się przycisk powrotu do poprzedniej strony i przycisk logowania. Podawane znaki w formularzu muszą zawierać tylko litery i cyfry, podanie innych znaków spowoduje wyświetlenie odpowiedniego komunikatu „wprowadzony nick/hasło zawiera niedozwolone znaki”.
Jeżeli wprowadzone są nie poprawne, w bazie danych nie ma podanego nicku, lub hasło się nie zgadza, zostaje wyświetlony komunikat o błędzie i pozostajemy na stronie logowania. Po poprawnym zalogowaniu się użytkownik zostaje przekierowany na stronę główną. 


Tabele potrzebne w bazie danych: 
Nazwa tabeli: User
Kolumny: idUser, nick, email, hasło, idAddony

Nazwa tabeli: Addony
Kolumny: idUser, idAddony

