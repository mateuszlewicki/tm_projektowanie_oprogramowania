# Analiza Biznesowa i Zbieranie Wymagań

## Przydatne linki
- https://www.coursera.org/learn/client-needs-and-software-requirements
- https://zwinnaanaliza.pl
- https://hub.ireb.org/media/pages/resources/cpre-foundation-level-syllabus/9c084b1cfd-1787039954/cpre_foundationlevel_syllabus_en_v.3.3.0.pdf
- [https://uml.developpez.com (Strona w języku francuskim)](https://uml.developpez.com
- https://softwaremind.com/blog/the-crucial-role-of-business-analysts-in-software-development/
- https://it-consulting.pl/2012/10/01/proces-zbierania-i-analizy-wymagan-u-developera/
- https://cejsh.icm.edu.pl/cejsh/element/bwmeta1.element.desklight-c73dc1bd-151d-4c24-b8a6-1ec8223614d6/c/053_ETI_nr_Vol_8_4_Metoda_zbierania.pdf
- https://www.jellytech.com.pl/post/okiem-jellytech-analiza-wymagan-wprowadzenie
- https://zerobs.pl/zarzadzanie-projektami/zbieranie-wymagan-biznesowych/
- https://nofluffjobs.com/pl/etc/specjalizacja/wymagania-funkcjonalne-w-tworzeniu-oprogramowania/
- https://www.skmgp.com/pl/blog/software-development-process---step-by-step-tutorial


## Zrozumienie celów projektu i potrzeb klienta

Zrozumienie celów projektu i potrzeb klienta to początkowa faza cyklu życia oprogramowania (SDLC), której zadaniem jest zidentyfikować problem biznesowy zamawiającego oraz ustalić oczekiwany stan docelowy po wdrożeniu systemu

### Identyfikacja interesariuszy
Interesariuszem (ang. stakeholder) nazywamy każdą osobę, grupę lub organizację, która ma wpływ na projekt lub na którą projekt wywiera wpływ.
- Interesariusze biznesowi: Zarząd, właściciele procesu, sponsorzy projektu (definiują budżet i cele strategiczne).
- Interesariusze operacyjni: Użytkownicy końcowi, administratorzy systemu (definiują wytyczne użytkowe i operacyjne).
### Analiza dziedziny i kontekstu biznesowego
Przed przystąpieniem do definicji wymagań technicznych należy dokonać analizy środowiska, w którym aplikacja będzie funkcjonować:
- Stan obecny (As-Is): Opis istniejących procesów, procedur oraz ewentualnych systemów dziedziczonych (ang. legacy systems).
- Stan docelowy (To-Be): Wokół jakich celów ma być zaprojektowany nowy system (np. automatyzacja powtarzalnych czynności, wyeliminowanie błędów ludzkich, skrócenie czasu przetwarzania danych).

## Definiowanie wymagań funkcjonalnych i niefunkcjonalnych
Inżynieria wymagań klasyfikuje oczekiwania wobec systemu na dwie podstawowe kategorie: wymagania funkcjonalne (FR) oraz wymagania niefunkcjonalne (NFR).


### Wymagania Funkcjonalne (ang. Functional Requirements – FR)
Definiują co system ma robić. Opisują zachowanie systemu, jego funkcje, reakcje na konkretne dane wejściowe oraz zachowanie w określonych sytuacjach.
#### Zakres: 
 Użytkownicy, procedury obliczeniowe, przetwarzanie danych, walidacja, integracje z zewnętrznymi API.
#### Forma zapisu:
Historyjki użytkownika (ang. User Stories), Przypadki użycia (ang. Use Cases).
#### Przykład: 
System umożliwia edycję profilu użytkownika przez Administratora.
### Wymagania Niefunkcjonalne (ang. Non-Functional Requirements – NFR)
Definiują jak system ma realizować swoje funkcje. Określają ograniczenia, jakościowe atrybuty systemu oraz kryteria operacyjne.
#### Kategorie NFR:

- **Wydajność (Performance)**: Czas odpowiedzi interfejsu, przepustowość bazy danych.
- **Bezpieczeństwo (Security)**: Szyfrowanie połączeń (TLS), polityka haseł, autoryzacja (RBAC).
- **Niezawodność i Dostępność (Reliability & Availability)**: Wskaźnik SLA, obsługa błędów, odporność na awarie sieciowe.
- **Utrzymywalność (Maintainability)**: Zgodność z wzorcami projektowymi, poziom pokrycia kodem przez testy.
- **Przykład**: Czas wyszukiwania rekordu w bazie danych nie może przekraczać 200 ms przy obciążeniu 1000 równoległych zapytań.

## Narzędzia i techniki zbierania wymagań

### Techniki zbierania wymagań
- **Wywiady i ankiety**: Strukturyzowane rozmowy z interesariuszami w celu wydobycia jawnych oczekiwań.
- **Obserwacja (Shadowing)**: Analiza pracy użytkowników na ich stanowiskach w celu wypracowania optymalnego przepływu pracy (ang. workflow).
- **Analiza dokumentacji i inżynieria odwrotna**: Badanie dotychczasowej dokumentacji, schematów baz danych oraz kodu źródłowego istniejących aplikacji.
- **MoSCoW (Technika priorytetyzacji)**:
	- **Must have**: Wymagania krytyczne (brak oznacza porażkę projektu).
	- **Should have**: Wymagania ważne, ale niekrytyczne w pierwszej wersji (MVP).
	- **Could have**: Wymagania pożądane, realizowane w przypadku wolnych zasobów.
	- **Won't have**: Wymagania odrzucone w danym etapie realizacyjnym.
### Dokumentowanie i narzędzia
- **User Storie**s (Historyjka Użytkownika): krótki szablon opisu funkcji z perspektywy roli:
 Jako [Rola] chcę [Funkcja], aby [Korzyść] 
- **Kryteria Akceptacji** (Acceptance Criteria): Warunki, które muszą zostać spełnione, aby wymaganie uznać za zrealizowane (często zapisywane w formacie BDD: Given-When-Then).
- **Modelowanie formalne (UML)**:
	- Diagram Przypadków Użycia (Use Case Diagram): Prezentuje relacje między aktorami a funkcjonalnościami.
	- Diagram Czynności (Activity Diagram): Przedstawia przebieg procesów biznesowych i przepływ sterowania.

## Metoda MoSCoW

Metoda ustalania priorytetów dla historyjek (lub innych elementów) w podejściach przyrostowych i iteracyjnych. Metoda MoSCoW (must have, should have, could have, won’t have) pozwala wypracować wspólne zrozumienie względnej ważności dostarczenia danej historyjki lub innego elementu wartości w ramach produktu.

