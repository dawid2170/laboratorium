# Projekt 2.1: Opis systemu plików EXT4

## Wprowadzenie
EXT4 (Fourth Extended Filesystem) jest jednym z najczęściej używanych systemów plików w systemie Linux. Wersja 2.0 dokumentacji zawiera szczegółowe informacje na temat struktury i działania systemu plików EXT4, w tym bloki, i-węzły, grupy bloków, dziennik i inne istotne elementy.

## Struktura systemu plików EXT4
### Bloki
Bloki są podstawową jednostką przechowywania danych w EXT4. Domyślnie, rozmiar bloku wynosi 4 KB, ale może być inny w zależności od konfiguracji.

### I-węzły
I-węzły (inode) są strukturami danych, które przechowują informacje o plikach i katalogach, takie jak prawa dostępu, właściciel, rozmiar i lokalizacja danych na dysku.

### Grupy bloków
Grupy bloków dzielą system plików na mniejsze sekcje, co pomaga zmniejszyć fragmentację i przyspieszyć dostęp do danych.

### Dziennik (Journaling)
EXT4 używa dziennika do śledzenia zmian w systemie plików, co pomaga zapobiegać uszkodzeniom danych w przypadku awarii systemu.

## Przykłady użycia
### Tworzenie systemu plików EXT4
```bash
mkfs.ext4 /dev/sdX1
