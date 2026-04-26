# Wiki – aplikacja encyklopedii

Aplikacja webowa inspirowana Wikipedią, umożliwiająca tworzenie, edycję oraz przeglądanie wpisów encyklopedycznych zapisanych w formacie Markdown.

Każdy wpis jest przechowywany jako plik Markdown i dynamicznie konwertowany do HTML podczas wyświetlania.

---

## 📌 Funkcjonalności

- Przeglądanie wpisów encyklopedii pod adresem `/wiki/TITLE`
- Tworzenie nowych stron encyklopedii
- Edycja istniejących wpisów
- Wyszukiwanie:
  - dokładne dopasowanie tytułu (przekierowanie na stronę)
  - częściowe dopasowanie (lista wyników)
- Losowa strona encyklopedii
- Konwersja Markdown → HTML
- Strona błędu dla nieistniejących wpisów

---

## 🧩 Jak działa aplikacja

- Wpisy są zapisywane jako pliki Markdown na dysku
- Treść jest dynamicznie ładowana przez Django
- Wyszukiwanie obsługuje zarówno dopasowanie pełne, jak i fragmentaryczne
- Edycja wpisów odbywa się poprzez formularz z prewypełnioną treścią
- Każdy wpis może być wyświetlony jako strona HTML

---

## 🛠️ Technologie

- Python
- Django
- HTML / CSS
- Markdown

---

## 📁 Struktura projektu

- `encyclopedia/` – logika aplikacji (widoki, routing)
- `entries/` – pliki Markdown z wpisami
- `templates/` – szablony HTML
- `util.py` – funkcje pomocnicze (odczyt i zapis wpisów)
