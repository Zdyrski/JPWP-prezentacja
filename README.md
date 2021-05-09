# JPWP-prezentacja

Zadanie 1. Server-Client
W metodach main() klienta i serwera użyć odpowiednich gotowych metod tak, aby:
-nawiązać połączenie
-klient wysłał wiadomość message i odczytał wiadomość od serwera
-serwer odebrał wiadomość i wysłał swoją 

W Zadaniach 2 i 3 w klasy Message muszą coś zaimplementować, aby móc przesyłać ich obiekty.

Zadanie 2. Przesyłanie obiektów.
Tak samo jak w zadaniu 1, tylko teraz zamiast String’a przesyłamy obiekt klasy Message2.

Zadanie 3. Wielowątkowość. 
Server3 dla każdego połączonego klienta startuje wątek ClientHandler do obsługi tego klienta i dodaje go do array listy clientHandlers. ClientHandler cały czas nasłuchuje na wiadomość od swojego klienta i jeśli jakąś dostanie rozsyłą ją do pozostałych klientów.
W klasie ClientHandler uzupełnić metodę sendToAll() tak, aby każdy element(oprócz tego elementu, który odebrał wiadomość) array listy clientHandlers wysłał podany jako argument obiekt message.
