# Python Hacking - flask

Projekt tworzony podczas spotkań hs3city *Python Hacking* w [Hacker:Space](http://hs3.pl/) trójmiasto.

## Przygotowanie środowiska:

### Linux / MacOS
_(ToDo: dla Windows)_

```bash
python3 -m venv ~/projekty/venv/pythonhacking-flask
```

Ewentualnie z kopiowaniem całego interpretera:
```bash
python3 -m venv --copies ~/projekty/venv/pythonhacking-flask
```

Aktywowanie środowiska:
```bash
source ~/projekty/venv/pythonhacking-flask/bin/activate
```

## Pobranie i uruchomienie projektu

Pobranie źródeł:
```bash
cd ~/projekty/
git clone https://github.com/hs3city/pythonhacking-flask.git
```

### Instalacja zależności
Pamiętaj, aby środowisko było aktywne:
```bash
cd ~/projekty/flask_hs/
pip install --upgrade -r requirements.txt
```

### Uruchomienie aplikacji

```bash
python manage.py runserver
```

### Inicjalizacja bazy danych

```bash
python manage.py init_db
```

### Czyszczenie bazy danych

```bash
python manage.py drop_db
```

### Wymagania

Aplikacja ToDo - wymagania:
 - [x] Menu do nawigacji u góry strony
 - [x] Główna strona z możliwością rejestracji i zalogowania
 - [x] Wszystkie pozostałe funkcjonalności dostępne są po zalogowaniu
 - [x] Lista ToDo danego użytkownika po zalogowaniu
 - [ ] Możliwość tworzenia kategorii list ToDo
 - [ ] Wyświetlanie ToDo dla wybranych kategorii
 - [ ] Możliwość oznaczania ToDo jako "skończone" -> przestają być
 widoczne na liście ToDo
 - [ ] Odzielna strona na przeglądanie zamkniętych ToDo
 - [ ] Strony ze statystykami dotyczącymi ToDo -> ile zakończonych,
 ile trwały (avg/min/max)
 - [ ] Możliwość wyświetlania/wyszukiwania zamkniętych ToDo

Wymagania niefunkcjonalne:
 - [x] Makefile lub inny mechanizm to automatyzacji wykonywania różnych operacji
 - [ ] testy funkcjonalne
 - [ ] unit testy
 - [x] Budowanie dockera w którym uruchamiana będzie aplikacja
 - [ ] docker-compose do uruchomienia aplikacji z bazą danych PostgreSQL
