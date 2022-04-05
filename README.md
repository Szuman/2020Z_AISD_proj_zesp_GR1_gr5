# 2020Z_AISD_proj_zesp_GR1_gr5
## Sytuacja geopolityczna
Polska, rok 2033. Kraj po wykonaniu serii ćwiczeń gimnastycznych (wstaniu z kolan, przewróceniu się o własne nogi, podniesieniu się i dumnym spojrzeniu w górę) ponownie został dotknięty pandemią. Po zmianach politycznych na samym szczycie współczesnej drabiny feudalnej, po ustąpieniu z tronu miłościwie panującego naczelnika i króla w jednej osobie, ludzie już zaczęli przyzwyczajać się do myśli, że ta zaraza nie wróci (tzn. pandemia nie wróci).
Rzeczywistość, w roli szulera, ponownie zagrała w karty z ludzkością, zachowując przy sobie wszystkie asy.
Kraj jest sparaliżowany wizją zamrożeniem całej gospodarki wywołanej strachem przed powtórzeniem doświadczeń z nieodległej przeszłości. Jednak na froncie walki ponownie, jak zwykle w trudnych momentach, postawiona została Służba Ochrony Zdrowia ze swoimi Ośrodkami Medycznymi (szpitalami) OM oraz ratownikami w Karetkach Pogotowia (KP).

KP realizują kursy do pacjentów (P) potrzebujących pomocy. Pacjenci mogą znajdować się w dowolnym miejscu na terenie kraju, a znalezionego pacjenta (P) należy przetransportować do najbliższego ośrodka medycznego (OM).
Znane są odległości pomiędzy poszczególnymi OM. Choć w niektórych miejscach kraju może nie występować bezpośrednia droga łącząca ze sobą OM.
Znany jest również fakt, że OM mają ograniczoną liczbę łóżek (LŁ) dla pacjentów.

## Opis zadania
Pomóż zespołom ratowników z Karetek Pogotowia (KP) przewozić pacjentów (P) do Ośrodków Medycznych (OM). Do tego celu możesz wykorzystać informacje, które otrzymujesz od Dyspozytora Pogotowia (DP).

```
# Szpitale (id | nazwa | wsp. x | wsp. y | Liczba łóżek | Liczba wolnych łóżek)
1 | Szpital Wojewódzki nr 997 | 10 | 10 | 1000 | 100
2 | Krakowski Szpital Kliniczny | 100 | 120 | 999 | 99
3 | Pierwszy Szpital im. Prezesa RP | 120 | 130 | 99 | 0
4 | Drugi Szpital im. Naczelnika RP | 10 | 140 | 70 | 1
5 | Trzeci Szpital im. Króla RP | 140 | 10 | 996 | 0

# Obiekty (id | nazwa | wsp. x | wsp. y)
1 | Pomnik Wikipedii | -1 | 50
2 | Pomnik Fryderyka Chopina | 110 | 55
3 | Pomnik Anonimowego Przechodnia | 40 | 70

# Drogi (id | id_szpitala | id_szpitala | odległość)
1 | 1 | 2 | 700
2 | 1 | 4 | 550
3 | 1 | 5 | 800
4 | 2 | 3 | 300
5 | 2 | 4 | 550
6 | 3 | 5 | 600
7 | 4 | 5 | 750

```
Do programu może zostać przekazana lista zawierająca wspołrzędne pacjentów. Należy umożliwić przeprowadzenie symulacji "obsługi" pacjentów (z poziomu graficznego interfejsu użytkownika).

```
# Pacjenci (id | wsp. x | wsp.y)
1 | 20 | 20
2 | 99 | 105
3 | 23 | 40
```
## Ważne
* Jeżeli drogi przecinają się, to można przyjąć, że w miejscu przecięcia jest skrzyżowanie;
* współrzędne pacjenta (punkt początkowy) może być dowolnym miejscem w obszarze ograniczonym przez współrzędne pozostałych punktów na mapie;
* obszar / mapa jest ograniczony przez najbardziej oddalone punkty (jest to najmniejszy zbiór wypukły zawierający w sobie wszystkie punkty);
* nie opiekujemy się pacjentami poza granicami kraju.
