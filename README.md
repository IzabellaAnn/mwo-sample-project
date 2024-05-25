

# mwo-sample-project

- Aplikacjia konsolowa, która wczytuje dane statystyczne z pliku
  JSON a następnie wyświetli podstawowe statystyki dotyczące 
  przetwarzanych danych.




## Authors
- Izabella Łecka
- Anna Grygierczyk
- Paweł Kawalec


## 🔗 Link
[![GitHub Project](https://github.com/users/IzabellaAnn/projects/2/views/1)](https://github.com/users/IzabellaAnn/projects/2/views/1)

-------------------------------------------

# Dane wejściowe
Przedmiotem analizy będzie plik zawierający informacje o czasie trwania pit stopów
poszczególnych zawodników, pobrane z serwisu https://openf1.org. Przykładowe zapytanie
zwracające dane z wyścigu na torze Imola z 2024 roku wygląda następująco:
https://api.openf1.org/v1/pit?session_key=9515. Sformatowany plik z pobranymi danymi został
dołączony na Moodle'a.
A oto wycinek danych z informacją o dwóch pit stopach:
Do naszego programu potrzebne są następujące informacje:
Wymagania funkcjonalne
Aplikacja powinna wczytać dane z przykładowego pliku oraz umożliwić policzenie (i wypisanie
na terminal) następujących wartości:

```bash
[
{
"session_key": 9515,
"meeting_key": 1235,
"date": "2024-05-19T13:13:40.698000+00:00",
"driver_number": 14,
"pit_duration": 31.3,
"lap_number": 7
},
{
"session_key": 9515,
"meeting_key": 1235,
"date": "2024-05-19T13:14:55.977000+00:00",
"driver_number": 23,
"pit_duration": 30.0,
"lap_number": 8
}
]
```

# Do naszego programu potrzebne są następujące informacje:

- długość trwania pit stopu pit_duration
- numer okrążenia lap_number
- numer kierowcy driver_number

# Wymagania funkcjonalne

Aplikacja powinna wczytać dane z przykładowego pliku oraz umożliwić policzenie (i wypisanie
na terminal) następujących wartości:

- liczbę pit stopów w wyścigu
- czas trwania najdłuższego pit stopu wraz z numerem kierowcy
- średni czas trwania pit stopów w całym wyścigu
- numer pierwszego i ostatniego zjazdu na pit stop