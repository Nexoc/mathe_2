# 📊 Übersicht: Graphentheorie kompakt erklärt (zweisprachig)

---

## 🔹 Was ist ein Graph?

Ein Graph **G = (V, E)** besteht aus:
- einer Menge von Knoten **V** („vertices“),
- einer Menge von Kanten **E**, die Knoten verbinden.

---

## 🔹 Graphtypen

- **Einfacher Graph**: keine Schleifen, keine Mehrfachkanten  
  \( E ⊆ \{ \{u, v\} | u ≠ v ∈ V \} \)

- **Multigraph**: erlaubt Mehrfachkanten, auch Schleifen möglich

- **Gerichteter Graph** (Digraph): Kanten haben Richtung  
  \( E ⊆ \{ (u, v) | u, v ∈ V \} \)

- **Ungerichteter Graph**: Kanten sind ungerichtet  
  \( \{u, v\} = \{v, u\} \)

---

## 🔹 Teilgraph

Ein **Teilgraph** \( G' = (V', E') \) ist ein Subset von \( G = (V, E) \),  
d. h. \( V' ⊆ V, E' ⊆ E \)

---

## 🔹 Knotengrad (deg)

- Im **ungerichteten Graphen**:  
  deg(u) = Anzahl der inzidenten Kanten  
  Schleifen zählen doppelt

- Im **gerichteten Graphen**:  
  - Eingangsgrad: Anzahl eingehender Kanten  
  - Ausgangsgrad: Anzahl ausgehender Kanten

---

## 🔹 Nachbarschaft

Zwei Knoten \( u, v \) sind **adjazent**, wenn \( \{u, v\} ∈ E \)  
Nachbarschaft von \( u \):  
\( N(u) = \{ v ∈ V | \{u, v\} ∈ E \} \)

---

## 🔹 Händedruck-Lemma

\[
sum {v∈V} deg(v) = 2m
\]

Die Summe aller Knotengrade = 2× Anzahl der Kanten.

---

## 🔹 Pfade, Wege, Kreise

- **Pfad**: Folge von Kanten, um von \( u \) nach \( v \) zu gelangen  
- **Einfacher Pfad**: keine Kante doppelt  
- **Kreis**: Pfad, bei dem Start- und Endknoten gleich sind  
- **Einfacher Kreis**: keine Kante doppelt

⚠ Begriffe sind in Literatur uneinheitlich

---

## 🔹 Zusammenhang

- **Zusammenhängender ungerichteter Graph**:  
  Für alle \( u, v ∈ V \) existiert ein Pfad zwischen ihnen
  

- **Zusammenhangskomponente**: maximaler zusammenhängender Teilgraph

- **Gerichteter Graph**:
    - stark zusammenhängend, wenn es für jedes Paar u,v einen gerichteten Pfad von u nach v und zurück gibt.
    - schwach zusammenhängend, wenn man alle Kanten als ungerichtet betrachtet und der resultierende Graph zusammenhängend ist.
---

## 🌲 Bäume (ungerichtet & gerichtet)

- **Baum**: zusammenhängender, kreisfreier, einfacher ungerichteter Graph  
- Eigenschaften:
  - genau ein einfacher Pfad zwischen zwei Knoten
  - bei \( n \) Knoten: genau \( n - 1 \) Kanten

- **Gerichteter Baum**:
  - hat einen Wurzelknoten (keine eingehenden Kanten)
  - alle anderen sind von der Wurzel erreichbar

---

✅ Fertig. Diese Datei deckt die wichtigsten Grundlagen der Graphentheorie ab – perfekt für Übersicht & Wiederholung.


