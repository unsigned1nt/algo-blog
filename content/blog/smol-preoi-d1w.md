---
date: '2025-12-15T22:17:00+01:00'
draft: false
title: 'Smol PREOI 2025 D1W'
---

<!--more-->

{{% include "note-zadanie-preoi.md" %}}

## Treść

Dany jest \( N \)-elementowy ciąg \( a(n) \). Potrzebujemy obsłużyć \( Q \) 
zapytań (typu \( 1 \)) o ilość spójnych podciągów niemalejących na przedziale 
\( a[L, R] \). Są też zapytania (typ \( 2 \)) o zmianę wartości \( a[i] \) na \( x \).


## Założenia

- \( 1 \leq N \leq 2 \cdot 10^5 \)
- \( 1 \leq Q \leq 2 \cdot 10^5 \)
- \( 1 \leq a[i], x \leq 10^9 \)


## Rozwiązanie

Na bazie ciągu \( a(n) \) konstruujemy ciąg \( b(n-1) \). 
Niech \( b[i]=(a[i] \leq a[i+1]) \). Wtedy postępujemy podobnie
do rozwiązania przedstawionego na omówieniu po konteście - budujemy drzewo 
przedziałowe, na którym robimy \( dp \), w którym łączymy ciągi \(11 \dots 1\).

TODO: opowiedz o metodzie dp na drzewie przedziałowym
