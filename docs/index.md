<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Dokumentacja Jira</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 0;
    }
    nav {
      background: #333;
      padding: 10px 20px;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 100;
    }
    nav ul {
      list-style: none;
      margin: 0;
      padding: 0;
      display: flex;
      gap: 20px;
    }
    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    nav ul li a:hover {
      text-decoration: underline;
    }
    section {
      padding: 100px 20px 40px; /* padding-top uwzględnia wysokość nav */
      max-width: 900px;
      margin: auto;
    }
    hr {
      border: none;
      border-top: 1px solid #ccc;
      margin: 20px 0;
    }
    h1, h2 {
      color: #333;
    }
  </style>
</head>
<body>

<nav>
  <ul>
    <li><a href="#home">Witaj</a></li>
    <li><a href="#teoria">Teoria działania Jira</a></li>
    <li><a href="#konfiguracja">Konfiguracja i wdrożenie</a></li>
    <li><a href="#przyklady">Przykłady ticketów</a></li>
    <li><a href="#autorzy">Informacje o autorach</a></li>
  </ul>
</nav>

<section id="home">
  <h1>Witaj w dokumentacji projektu <strong>Jira</strong></h1>
  <p>
    Witamy w naszym przewodniku po systemie <strong>Jira</strong> – jednym z najczęściej wykorzystywanych narzędzi do zarządzania projektami, zadaniami i zgłoszeniami w zespołach IT.
  </p>
  <hr />
</section>

<section id="teoria">
  <h2>Co znajdziesz w dokumentacji?</h2>
  <ul>
    <li>🔹 <strong>Teoria działania Jira</strong><br>Zrozumiesz podstawy działania systemu, jego zastosowania i najważniejsze funkcjonalności.</li>
    <li>🔹 <strong>Konfiguracja i wdrożenie</strong><br>Krok po kroku pokażemy Ci, jak rozpocząć pracę z Jira – od rejestracji konta po integrację z GitHubem.</li>
    <li>🔹 <strong>Przykłady wykorzystania ticketów</strong><br>Zobaczysz, jak tworzyć zgłoszenia (ticket’y), jak je organizować i przypisywać w praktyce.</li>
    <li>🔹 <strong>Informacje o autorach</strong><br>Poznasz osoby odpowiedzialne za przygotowanie projektu.</li>
  </ul>
  <hr />
</section>

<section id="konfiguracja">
  <h2>Konfiguracja i wdrożenie</h2>
  <p>Krok po kroku pokażemy Ci, jak rozpocząć pracę z Jira – od rejestracji konta po integrację z GitHubem.</p>
  <hr />
</section>

<section id="przyklady">
  <h2>Przykłady wykorzystania ticketów</h2>
  <p>Zobaczysz, jak tworzyć zgłoszenia (ticket’y), jak je organizować i przypisywać w praktyce.</p>
  <hr />
</section>

<section id="autorzy">
  <h2>Informacje o autorach</h2>
  <p>Poznasz osoby odpowiedzialne za przygotowanie projektu.</p>
  <hr />
</section>

<script>
  // Płynne przewijanie do sekcji po kliknięciu w link w menu
  document.querySelectorAll('nav a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
      e.preventDefault();
      const target = document.querySelector(this.getAttribute('href'));
      if (target) {
        target.scrollIntoView({
          behavior: 'smooth'
        });
      }
    });
  });
</script>

</body>
</html>
