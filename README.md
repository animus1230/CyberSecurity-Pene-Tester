# Raport Cyberbezpieczeństwa

## 1. Dane osobowe
- **Imię i nazwisko:** Kevin  
- **Wiek:** 17 lat  
- **Kierunek zainteresowań:** Penetration Testing (Pene Tester)  
- **Kontakt:** bibip0662@gmail.com  

---

## 2. Cel i motywacja
Jako pasjonat cyberbezpieczeństwa, moim głównym celem jest zdobycie praktycznego doświadczenia w dziedzinie bezpieczeństwa IT oraz nawiązanie współpracy z doświadczonymi profesjonalistami, którzy pomogą mi rozwijać umiejętności w realnych scenariuszach. Jestem gotów odbyć praktyki nawet bez wynagrodzenia, ponieważ liczy się dla mnie przede wszystkim zdobywanie wiedzy i umiejętności. Szukam mentora, który poprowadzi mnie w przyszłości, dzieląc się cennymi wskazówkami i doświadczeniem.

---

## 3. Wykształcenie i samokształcenie
- **Formalna edukacja w kierunku cyberbezpieczeństwa:**  
  - Obecnie nie uczę się w szkole o profilu związanym z bezpieczeństwem IT. W najbliższej przyszłości planuję podjąć naukę na kierunku związanym z penetration testingiem.  
- **Samokształcenie:**  
  - Całą wiedzę zdobywam samodzielnie, przede wszystkim poprzez praktykę.  
  - Studiuję materiały online: tutoriale, dokumentacje narzędzi oraz blogi ekspertów z branży.  
  - Ćwiczę w środowiskach wirtualnych, budując własne laby (VMware/VirtualBox) i testując konfiguracje, analizy podatności i proste eksploity.  

---

## 4. Umiejętności techniczne
> *Poniższy zestaw umiejętności jest przedstawiony w sposób możliwie najbardziej profesjonalny. W rzeczywistości opieram się głównie na gotowych narzędziach i skryptach, ale posiadam solidne podstawy teoretyczne i praktyczne.*

### 4.1. Systemy operacyjne
- **Linux (dystrybucje Kali, Parrot, Ubuntu):**  
  - Znajomość podstawowych komend Bash oraz zarządzania pakietami.  
  - Konfiguracja środowiska testowego (wirtualizacja, kontenery LXC/Docker).  
- **Windows:**  
  - Podstawowa administracja Windows 10/11.  
  - Znajomość PowerShell na poziomie podstawowym (tworzenie prostych skryptów).  

### 4.2. Sieci i protokoły
- **Protokoły sieciowe:**  
  - TCP/IP, UDP, HTTP, HTTPS, DNS, ARP – umiejętność analizy pakietów i ruchu sieciowego.  
  - Konfiguracja i analiza ruchu w Wireshark.  
- **Sieci bezprzewodowe:**  
  - Podstawowe zagadnienia Wi-Fi (WEP/WPA/WPA2).  
  - Techniki sniffingu i łamania zabezpieczeń w sieciach Wi-Fi.  

### 4.3. Testy penetracyjne (Penetration Testing)
- **Metodologie:**  
  - OWASP Top 10 – omówienie najważniejszych zagrożeń aplikacji webowych.  
  - OSSTMM (Open Source Security Testing Methodology Manual) – podstawy.  
- **Narzędzia:**  
  - **Hydra (THC-Hydra):** narzędzie do ataków brute-force na usługi sieciowe (SSH, FTP, HTTP, RDP itp.).  
  - **John the Ripper:** narzędzie do łamania haseł, analiza plików z haszami.  
  - **Nmap:** skanowanie portów, wykrywanie usług, skryptowanie NSE.  
  - **Metasploit Framework:** tworzenie i wykorzystywanie modułów exploitów, zarządzanie payloadami.  
  - **Burp Suite (Community Edition):** podstawowa konfiguracja proxy, analiza ruchu HTTP, testowanie luk w aplikacjach webowych.  
  - **sqlmap:** zautomatyzowane wykrywanie i eksploatacja SQL Injection.  
  - **Nikto:** skanowanie podatności serwerów WWW.  
  - **Recon-ng:** zautomatyzowane zbieranie informacji (OSINT) o domenach i infrastrukturze.  

### 4.4. Programowanie i skrypty
- **Programowanie:**  
  - Nie potrafię programować od podstaw – korzystam wyłącznie z gotowych skryptów i narzędzi przygotowanych przez społeczność lub ekspertów.  

---

## 5. Projekty i doświadczenie
### 5.1. Laboratorium testów penetracyjnych (środowisko wirtualne)
- **Opis:**  
  - Samodzielnie skonfigurowane środowisko wirtualne opierające się na VirtualBox + Kali Linux oraz Windows 10 VM.  
  - Przeprowadzenie ćwiczeń związanych ze skanowaniem portów, analizą podatności i prostą eksploatacją usług.  
- **Wykorzystane narzędzia:**  
  - Nmap, Metasploit, Hydra, John the Ripper, Burp Suite.  

### 5.2. Analiza podatności prostego serwera WWW
- **Opis:**  
  - Konfiguracja własnego serwera WWW (Apache) na Kali Linux i przeprowadzenie testów bezpieczeństwa.  
  - Wykrywanie prostych błędów w konfiguracji, np. brak aktualizacji, katalogi wystawione na publiczny dostęp.  
- **Rezultat:**  
  - Raport z rekomendacjami zabezpieczeń: konfiguracja HSTS, wymuszenie HTTPS, ograniczenie listy modułów Apache, aktualizacja systemu.  

### 5.3. Podstawowy atak typu brute-force na usługę SSH
- **Opis:**  
  - Przygotowanie skryptu w Bash, wykorzystującego narzędzie Hydra do testów siłowych na wirtualnej maszynie.  
  - Monitorowanie wydajności, analiza skuteczności ataku.  
- **Rezultat:**  
  - Dokumentacja opisująca proces: generowanie słowników, tuning parametrów Hydra, analiza szybkości łamania haseł.  

---

## 6. “Hydra John” – zestaw narzędzi do łamania haseł
Jako część mojej praktyki skonfigurowałem zestaw narzędzi “Hydra John”, który łączy w sobie możliwości:
- **Hydra (THC-Hydra):**  
  - Automatyzacja ataków brute-force na usługi sieciowe.  
  - Obsługa protokołów: SSH, FTP, Telnet, HTTP, POP3, IMAP, RDP i innych.  
  - Ustawienia zaawansowane: równoległe wątki, słowniki, ataki hybrydowe.  
- **John the Ripper:**  
  - Łamanie haseł offline (np. pliki z haszami Linux, pliki `shadow`, pliki `wp-users.sql`).  
  - Wykorzystanie modułów “single”, “wordlist+rules”, “incremental”.  
  - Integracja z narzędziami do ekstrakcji haszów (np. `hashcat-utils`).  

Podstawowe funkcjonalności zestawu “Hydra John”:
1. **Przygotowanie środowiska:**  
   - Instalacja Kali Linux, aktualizacja pakietów:  
     ```bash
     sudo apt update && sudo apt upgrade
     sudo apt install hydra john hashcat
     ```  
2. **Konfiguracja słowników:**  
   - Użycie popularnych słowników (np. `rockyou.txt`, `SecLists`).  
   - Modyfikacja i tworzenie dedykowanych słowników (np. na potrzeby specyficznych testów).  
3. **Scenariusze ataków:**  
   - Brute-force na SSH:  
     ```bash
     hydra -l root -P /usr/share/wordlists/rockyou.txt ssh://192.168.56.101
     ```  
   - Łamanie haszy offline:  
     ```bash
     john --wordlist=/usr/share/wordlists/rockyou.txt /mnt/data/hashe.shadow
     ```  

---

## 7. Umiejętności miękkie
- **Komunikacja:**  
  - Otwartość na konstruktywną krytykę i dyskusję techniczną.  
  - Umiejętność pracy w zespole (wirtualne grupy projektowe).  
- **Zarządzanie czasem:**  
  - Zdolność do samodzielnej organizacji zadań, wyznaczania priorytetów.  
  - Szybkie przyswajanie informacji i adaptacja do nowych narzędzi.  
- **Kreatywność:**  
  - Poszukiwanie niestandardowych metod testowania zabezpieczeń.  
  - Eksperymentowanie z różnymi konfiguracjami środowiska testowego.  

---

## 8. Cele zawodowe i plany rozwoju
1. **Praktyki / staż w firmie zajmującej się bezpieczeństwem IT**  
   - Jestem otwarty na praktyki nawet nieodpłatne – dla mnie kluczowa jest wiedza i doświadczenie “z pierwszej ręki”.  
2. **Znalezienie mentora / opiekuna merytorycznego**  
   - Poszukuję osoby z co najmniej kilkuletnim doświadczeniem w pentestingu lub bezpieczeństwie sieci, która pomoże rozwinąć moje umiejętności i ukierunkuje dalszą ścieżkę edukacyjną.  
3. **Rozbudowa warsztatu narzędziowego**  
   - Nauka programowania (Python, Go, C) w kontekście tworzenia własnych exploitów i narzędzi automatyzujących testy bezpieczeństwa.  
   - Poszerzenie wiedzy o inżynierię wsteczną (reverse engineering), analiza złośliwego oprogramowania.  
4. **Udział w konkursach CTF (Capture The Flag)**  
   - Regularne uczestnictwo w wydarzeniach typu CTF (TryHackMe, Hack The Box, CTFtime).  
   - Prowadzenie własnych wyzwań i dzielenie się rozwiązaniami na blogu/GitHub.  

---

## 9. Kontakt i współpraca
- **E-mail:** bibip0662@gmail.com  
- **GitHub:** [github]:https://github.com/animus1230
**Szukanie praktyk i mentora:**  
Jeśli jesteś doświadczonym specjalistą ds. bezpieczeństwa sieci lub penetracji i masz możliwość przyjęcia młodego, ambitnego adepta cyberbezpieczeństwa, proszę o kontakt – jestem otwarty na każde wyzwanie. Liczy się dla mnie jedynie możliwość nauki od ekspertów oraz realne zadania, które pozwolą mi się rozwijać.

---

## 10. Podsumowanie
Jestem młodym, pełnym zapału entuzjastą cyberbezpieczeństwa. Pomimo że na ten moment nie tworzę własnych programów od podstaw i korzystam z gotowych narzędzi, to jednak posiadam solidną podstawę teoretyczną (solinę podstawę) oraz doświadczenie w środowisku laboratoryjnym. Chcę szybko zdobywać nową wiedzę i rozwijać się pod okiem mentora. Szukam praktyk, nawet nieodpłatnych, by móc wykorzystać swoje umiejętności w realnych projektach. Wierzę, że dzięki współpracy z doświadczonymi specjalistami osiągnę poziom, który pozwoli mi w przyszłości samodzielnie prowadzić zaawansowane testy penetracyjne.

> **Hydra John** – mój zestaw narzędzi do ataków brute-force i łamania haseł, skonfigurowany do szybkich testów na środowiskach wirtualnych.  

**Zapraszam do kontaktu i współpracy!**
