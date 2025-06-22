# Konfiguracja i wdrożenie Jira

Poniżej znajdziesz szczegółową instrukcję krok po kroku, jak skonfigurować i wdrożyć Jira w Twoim zespole, wraz z podstawową integracją z GitHub oraz wskazówkami dotyczącymi zarządzania projektami i workflow.

---

## 1. Rejestracja konta

1. Przejdź na stronę: [https://www.atlassian.com/software/jira](https://www.atlassian.com/software/jira)
2. Załóż nowe konto lub zaloguj się, jeśli już posiadasz.
3. Wybierz odpowiedni plan (darmowy lub płatny, w zależności od potrzeb zespołu).

---

## 2. Utwórz pierwszy projekt

- Po zalogowaniu kliknij **Create project**.
- Wybierz typ projektu:
  - **Software project** – do zarządzania zespołami programistycznymi.
  - Typ metodyki: **Scrum** (jeśli pracujesz sprintami) lub **Kanban** (praca ciągła).
- Nadaj nazwę projektu, np. „Zespół IT”.
- Opcjonalnie ustaw klucz projektu (skrót, np. IT).

---

## 3. Dodaj członków zespołu

- Przejdź do **Settings** → **People**.
- Kliknij **Invite users**.
- Wpisz adresy email członków zespołu i wybierz ich role (np. Developer, Administrator, Viewer).

---

## 4. Konfiguracja workflow

Workflow to schemat statusów, przez które przechodzi ticket (zgłoszenie).

- Przejdź do **Settings** → **Issues** → **Workflows**.
- Wybierz istniejący workflow lub utwórz nowy klikając **Add workflow**.
- Dodaj statusy, np.:
  - To Do (Do zrobienia)
  - In Progress (W trakcie)
  - Review (Weryfikacja)
  - Done (Zakończone)
- Ustaw przejścia między statusami (np. z To Do do In Progress, z In Progress do Review).
- Zapisz workflow i przypisz go do odpowiednich typów ticketów.

---

## 5. Zarządzanie backlogiem i sprintami (dla Scrum)

- W panelu projektu przejdź do zakładki **Backlog**.
- Dodaj nowe zadania/tickety do backlogu.
- Twórz sprinty, przeciągając zadania do planowanego sprintu.
- Uruchom sprint, klikając **Start sprint** i zarządzaj postępem na tablicy Scrum.

---

## 6. Ustawienia ról i uprawnień

- W **Project settings** → **Permissions** możesz ustawić, kto co może robić (np. tworzyć tickety, zmieniać statusy).
- Możesz tworzyć niestandardowe role i przypisywać je użytkownikom.

---

## 7. Integracja z GitHub

Integracja pozwala automatycznie powiązać zmiany w repozytorium z ticketami Jira.

- Przejdź do **Apps** w Jira → wyszukaj i zainstaluj aplikację **GitHub for Jira**.
- Po instalacji połącz konto GitHub, autoryzując dostęp.
- Skonfiguruj repozytoria, które mają być monitorowane.
- Dodaj w commit message ID ticketu, np. `PROJECT-123`, aby automatycznie powiązać commit z ticketem.
- Możesz ustawić automatyczne przejścia ticketów po pushu (np. po mergu ticket zostaje zamknięty).

---

## 8. Powiadomienia i automatyzacje

- W **Project settings** → **Notifications** możesz ustawić, kto i kiedy otrzymuje powiadomienia o zmianach.
- Użyj **Automation rules**, by automatycznie wykonywać akcje, np. przypisywać tickety, zmieniać statusy, wysyłać powiadomienia.

---

## 9. Raportowanie i analiza

- Jira oferuje gotowe raporty (burndown, velocity, raporty o błędach).
- Możesz generować wykresy na podstawie danych z projektu, co pomaga w planowaniu i ocenie postępów.

---

# Podsumowanie

Prawidłowa konfiguracja Jira pozwala na pełne wykorzystanie potencjału systemu w zarządzaniu projektem. Dzięki powyższym krokom ustawisz środowisko dostosowane do potrzeb zespołu, usprawnisz komunikację oraz monitoring pracy.


