# JPWP-prezentacja

## Zadanie 1. Server-Client
W metodach main() klienta i serwera użyć odpowiednich gotowych metod tak, aby:
* nawiązać połączenie
* klient wysłał wiadomość message i odczytał wiadomość od serwera
* serwer odebrał wiadomość i wysłał swoją 


### W Zadaniach 2 i 3 klasa Message musi coś zaimplementować, aby móc przesyłać obiekty.


## Zadanie 2. Przesyłanie obiektów.

Podobnie jak w zadaniu 1, tylko tym razem zamiast String’a przesyłamy obiekt klasy Message2.

## Zadanie 3. Wielowątkowość. 

Server3 dla każdego połączonego klienta startuje wątek ClientHandler do obsługi tego klienta i dodaje go do arrayListy clientHandlers. ClientHandler ciągle nasłuchuje na wiadomość od swojego klienta i jeśli jakąś dostanie rozsyła ją do pozostałych klientów.

W klasie ClientHandler uzupełnić metodę sendToAll() tak, aby każdy element arrayListy clientHandlers wysłał podany jako argument obiekt message. Zwróć uwagę, że element, który odebrał wiadomość nie powinien tego robić.
