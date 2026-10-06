# Ryczałtomat

Wewnętrzne narzędzie sklepu **EveryShop4You** na Allegro — przygotowuje ewidencję sprzedaży
dla biura rachunkowego (jednoosobowa działalność na ryczałcie).

## Co robi aplikacja

- pobiera z Allegro REST API **wyłącznie dane własnego konta sprzedawcy**: zamówienia,
  operacje billingowe (opłaty i prowizje), zwroty klientów i historię operacji płatniczych,
- korzysta **tylko z uprawnień do odczytu** — niczego nie wystawia, nie zmienia ofert ani zamówień,
- działa lokalnie na komputerze właściciela; dane nie są nikomu udostępniane ani przesyłane dalej,
- zapytania wysyła rzadko — kilka razy w miesiącu, przy zamknięciu miesiąca.

Na podstawie pobranych danych powstaje rejestr sprzedaży, rejestr zwrotów i zestawienie marży.

## Dane techniczne

- typ aplikacji: device flow (OAuth 2.0), jedno konto sprzedawcy,
- nagłówek User-Agent: `Ryczałtomat/<wersja> (+https://github.com/Buczuuu/Ryczaltomat-info)`, np. `Ryczałtomat/1.0.0 (+https://github.com/Buczuuu/Ryczaltomat-info)`.

## Kontakt

Przez profil GitHub [@Buczuuu](https://github.com/Buczuuu).
