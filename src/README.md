Aplikacja Spring Boot z Thymeleaf
Opis działania
Aplikacja wykorzystuje Spring Boot do obsługi żądań HTTP oraz Thymeleaf jako silnika szablonów HTML. Główne funkcjonalności aplikacji obejmują:

Endpoint /: Wyświetla powitanie w formie tekstowej.
Endpoint /greeting: Przyjmuje parametr name i wyświetla personalizowaną wiadomość, np. "Hello, Visula!", wraz z obrazkiem załadowanym z zasobów statycznych.
Case study
Problem 1: Jak obsługiwać dynamiczne widoki w aplikacji internetowej?

Rozwiązanie: Zastosowano Spring Boot w połączeniu z Thymeleaf. Endpoint /greeting przekazuje parametr name do widoku, który wyświetla go w wiadomości przy użyciu zmiennej Thymeleaf ${name}.
Rezultat: Personalizowane powitanie w przeglądarce.
Problem 2: Jak dodawać zasoby statyczne, takie jak obrazki?

Rozwiązanie: Obrazek został umieszczony w katalogu static/images (Spring automatycznie udostępnia zasoby z tego folderu).
Rezultat: Obrazek został poprawnie załadowany i wyświetlony na stronie.
Przykłady działania
Uruchomienie strony głównej:

Adres: http://localhost:8080
Wyświetla prosty komunikat:
perl
Skopiuj kod
Hello Vistula, in my first Spring controller.
Uruchomienie strony powitalnej:

Adres: http://localhost:8080/greeting?name=Visula
Wyświetla:
Skopiuj kod
Hello, Visula!
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Oraz obrazek vistula.png z folderu statycznego.
