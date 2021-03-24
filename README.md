# ZadanieTesterDelegacje
Repozytorium zawiera zgłoszenia błędów aplikacji webowej obiegu dokumentów w przedsiębiorstwie.
Screenshoty zgłoszeń zostały usunięte.

Przykładowe zgłoszenia znajdują się w zakładce "Issues" tego repozytorium. Każdy znaleziony przeze mnie błąd został odzwierciedlony w postaci osobnego ticketu.

Przykładowy scenariusz UAT dla utworzenia wniosku o delegację:

### Przypadek użycia:

**Aktor**  
Użytkownik systemu o uprawnieniach pracowniczych

**Cel**  
Utworzenie wniosku o delegację i wysłanie prośby o jego akceptację do użytkownika z uprawnieniami przełożonego

**Stan początkowy**  
Użytkownik loguje się do systemu za pomocą swojego konta

1. Użytkownik klika w przycisk oznaczony symbolem "+"
2. System wyświetla listę możliwych operacji
3. Użytkownik wybiera opcję "Wniosek o delegację"
4. System przenosi użytkownika na stronę z formularzem i prosi użytkownika o podanie danych
5. Użytkownik podaje wszystkie wymagane dane i klika przycisk "Wyślij"
   1. Użytkownik popełnia błąd i omija wymagane pole
   2. System informuje użytkownika o błędzie i blokuje opcję "Wyślij"
6. System wyświetla informację, że wniosek został utworzony i przenosi użytkownika do strony głównej

### Scenariusz testowy dla powyższego przypadku użycia:
|Numer|Wymaganie|Rezultat|Komentarz|
|---|---|---|---|
|1.|Użytkownik może odwiedzić stronę z formularzem tworzącym wniosek|   |   |
|2.|Użytkownik może podać cel, trasę, daty oraz inne wymagane dane opisujące delegacje|   |   |
|3.|Użytkownik może zapisać wrowadzone dane|   |   |
|4.|Zapisany wniosek jest widoczny na liście wysłanych wniosków|   |   |
|5.|System informuje użytkownika jeśli popełnił błąd podczas wypełniania formularza|   |   |
|6.|Wysłany wniosek jest widoczny w panelu przełożonego|   |   |
|7.|Przełożony otrzymał wiadomość e-mail z informacją o nowym wniosku do rozpatrzenia|   |   |
