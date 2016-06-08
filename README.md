# veriMotion
Jest to framework do aplikacji Javovych który testuje, a także kontroluje dwvelopera czy prawidłowo teestuje swoją aplikację. Dzięki tej bibliotece dostajemy gotowe narzędzie do testowania.

Wersja 0.1
  - Sprawdzanie zawartości projektu pod kątem używania testów z biblioteki
  - Mechanizm łaczący metodę startową testu z metodą kończącą
  - Odczytywanie "podstawowych emocji uzytkownika" 
  - Podstawowe komunikaty o błedach
  
  Jak używać veriMotion:    
    1.  Dodać do projektu plik verimotion.jar (znajdują się w nim wszystkie elementy potrzebne do testowania)
    2.  W głównym pliku uruchomieniowym (np. static main() ), musimy użyć komendy Searching.check(Main.class); (metoda ta zacznie sprawdzać nasz projekt w poszukiwaniu testów oraz uruchomi silnik odpowiedzialny za testowanie)
    3.  Aby utworzyć test czyli przetestować jakąś funkcjonalność musimy nadać adnotację @StartTest(id=1) w miejscu w którym ma zacząć się sprawdzanie (id musi być unikatowe la każdego testu), aby zakończyć test musimy w metodzie która finalizuje test dodać adnotację @StopTest(id=1).
    4.  Aby poinformować silnik testowy o tym że dana metod startuje używamy w metodzie oznaczonej adnotacją startową metody Check.start(1);
    5.  Aby poinformować silnik testowy że wykonuje się metoda kończąca test, którą oznaczyliśmy adnotacją końcową, dodajemy metodę Check.finish(1);
  
  Aktualne prace:
  Pozbycie się metod z punktu 4 oraz 5. przy wykorzystaniu silnika Adnotacyjnego.
  Dodanie adnotacji startowej i zastępując metodę z punktu 2.

  
