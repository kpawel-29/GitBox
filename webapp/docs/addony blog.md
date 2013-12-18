[&#8810;](../README.md) spis treści

Opis addonu – blog

Jest to jeden z głównych addonów, ustawiany domyślnie jako włączony. Użytkownik posiadający ten addon będzie miał możliwość dodawania, edycji, komentowania i usuwania swoich notatek. Notatki mogą być prywatne (wyświetlane tylko dla właściciela) lub publiczne (pokazywane wszystkim). 
Blog wyświetlany jest w formie postów ułożonych chronologicznie zgodnie z datami dodania wiadomości. Wyświetlane będą informacje o nicku właściciela notatki, dacie dodania, treść wiadomości i komentarze. Nie ma ograniczenia na długość notatki, ani na długość komentarza. 
Komentować mogą tylko zalogowani użytkownicy, treści notatek są dostępne publicznie wszystkim.

Tabele potrzebne w bazie danych:
nazwa tabeli: Blog
Kolumny: idNotatka, idAutor, prywatna, dataDodania, treść, idKomentarz

nazwa tabeli: Komentarz 
Kolumny: idKomentarz, idAutor, dataDodania, treść 
