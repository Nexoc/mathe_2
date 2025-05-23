# 🔁 Permutationsmatrizen – Definition, Eigenschaften und Beispiel

---

## 🔷 Was ist eine Permutationsmatrix?

Eine **Permutationsmatrix** ist eine spezielle quadratische Matrix, bei der in **jeder Zeile und jeder Spalte genau eine Eins** steht – alle anderen Einträge sind Null.

Man erhält sie durch Vertauschung der Zeilen (oder Spalten) der Einheitsmatrix.

---

## 🧩 Eigenschaften

- Genau **eine 1 pro Zeile und Spalte**
- Alle anderen Einträge sind **0**
- **Orthogonalität**:  
  \( Pᵀ = P⁻¹ \)
- Produkt mit Transponierter ergibt die Einheitsmatrix:  
  \( P ⋅ Pᵀ = I \)
- **Determinante**:  
  \( \det(P) = ±1 \)
- **Links-Multiplikation**: vertauscht **Zeilen**
- **Rechts-Multiplikation**: vertauscht **Spalten**

---

## 📘 Beispiel: Vertauschen eines Vektors

Gegeben sei der Vektor:

```

x = (a, b, c)ᵀ

```

und die Permutationsmatrix:

```

P =
0 0 1
1 0 0
0 1 0

```

Berechne:

```

P ⋅ x =
(0 0 1)   (a)    = (c)
(1 0 0) \* (b)  = (a)
(0 1 0)   (c)    = (b)

```

**Ergebnis:**

```

P ⋅ x = (c, a, b)ᵀ

```

→ Die Einträge wurden zyklisch vertauscht: Position 1 → 3, 2 → 1, 3 → 2

---

## 🔁 Transponierte und Inverse

Die Transponierte \( Pᵀ \) ist auch die Inverse:  
```

Pᵀ = P⁻¹

```

Wenn \( P \) Zeilen vertauscht, dann vertauscht \( Pᵀ \) die gleichen Spalten.

---

## 🔄 Matrixmultiplikation

Sei \( A \) eine Matrix, dann gilt:

- \( P ⋅ A \): vertauscht **Zeilen** von \( A \)
- \( A ⋅ Pᵀ \): vertauscht **Spalten** von \( A \)

Aus der Transpositionsregel:

```

(P ⋅ Aᵀ)ᵀ = A ⋅ Pᵀ

```

---

✅ Jetzt ist die Permutationsmatrix formal definiert, mit allen relevanten Eigenschaften und einem anschaulichen Beispiel – perfekt geeignet für Lernunterlagen oder GitHub-Dokumentation.


