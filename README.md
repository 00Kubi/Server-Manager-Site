## Server Manager Site

### Opis projektu

**Server Manager Site** to aplikacja webowa umożliwiająca przeglądanie, edytowanie i zarządzanie plikami bezpośrednio z przeglądarki. Oferuje dostęp do plików serwerowych, ich modyfikacji oraz uruchamiania komend terminala na serwerze za pomocą wbudowanej konsoli. Projekt jest idealnym rozwiązaniem dla developerów potrzebujących zdalnego zarządzania serwerem z poziomu przeglądarki.

### Funkcje
- **Przeglądarka plików**: Przeglądaj strukturę katalogów i plików na serwerze.
- **Edytor plików**: Edytuj pliki tekstowe bezpośrednio w przeglądarce.
- **Terminal**: Uruchamiaj komendy systemowe za pomocą wbudowanej konsoli terminala.
- **Zarządzanie plikami**: Twórz, usuwaj, przenoś i zmieniaj nazwy plików i folderów.

### Technologie
- **Frontend**: HTML, CSS, JavaScript (możesz wykorzystać React.js)
- **Backend**: Node.js, Express.js, WebSocket, File System (fs)
- **Terminal**: node-pty, xterm.js

---

### To-Do List

#### Faza 1: Planowanie i inicjalizacja projektu
- [x] Stworzenie repozytorium na GitHubie
- [x] Inicjalizacja projektu z użyciem `npm init`
- [ ] Zainstalowanie podstawowych zależności:
  - `express` (serwer backendowy)
  - `ws` (WebSocket do komunikacji terminala)
  - `node-pty` (do emulacji terminala)
  - `fs` (system plików w Node.js)

#### Faza 2: Frontend (Interfejs użytkownika)
- [ ] Stworzenie podstawowej struktury strony (HTML + CSS + JavaScript)
- [ ] Zaimplementowanie przeglądarki plików (wyświetlanie struktury katalogów)
- [ ] Zaimplementowanie funkcji tworzenia i usuwania plików oraz folderów
- [ ] Dodanie edytora plików do edycji plików tekstowych (np. Monaco Editor)
- [ ] Stylizacja interfejsu użytkownika

#### Faza 3: Backend (Serwer)
- [x] Utworzenie serwera Express.js
- [x] Zainstalowanie i skonfigurowanie WebSocket do komunikacji z terminalem
- [ ] Zaimplementowanie logiki przeglądania plików przy użyciu `fs`
- [ ] Utworzenie endpointów API do zarządzania plikami (tworzenie, usuwanie, edycja)

#### Faza 4: Integracja terminala
- [ ] Konfiguracja **node-pty** do obsługi komend terminala
- [ ] Połączenie terminala z interfejsem za pomocą WebSocket (xterm.js)
- [ ] Testowanie terminala (wywoływanie komend np. `ls`, `mkdir`, `rm`)

#### Faza 5: Testowanie i finalizacja
- [ ] Testowanie aplikacji pod kątem funkcjonalności przeglądarki plików
- [ ] Testowanie edytora plików
- [ ] Testowanie terminala i komunikacji w czasie rzeczywistym
- [ ] Usunięcie błędów i optymalizacja kodu

#### Faza 6: Dokumentacja i wdrożenie
- [ ] Utworzenie pełnej dokumentacji (opis API, konfiguracja, uruchomienie)
- [ ] Przygotowanie aplikacji do wdrożenia na serwerze (np. Heroku, VPS)
- [ ] Finalne wdrożenie

---

### Uruchomienie projektu

Aby uruchomić projekt lokalnie, wykonaj następujące kroki:

1. Sklonuj repozytorium:
   ```bash
   git clone https://github.com/yourusername/WebFileManager.git
   ```

2. Zainstaluj zależności:
   ```bash
   npm install
   ```

3. Uruchom serwer:
   ```bash
   node server.js
   ```

4. Otwórz przeglądarkę i przejdź na adres:
   ```
   http://localhost:3000
   ```

---

### Contributing

Wszelkie sugestie i pull requesty są mile widziane. Aby uzyskać więcej informacji na temat wprowadzania zmian, zapoznaj się z plikiem [CONTRIBUTING.md](CONTRIBUTING.md).

---

Czy potrzebujesz dodatkowych instrukcji lub zmian w tej strukturze?
