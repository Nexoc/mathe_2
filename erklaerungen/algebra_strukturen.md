# ⚙️ Algebraische Strukturen und Eigenschaften von Operationen

## 📌 Eigenschaften von Operationen

**1. Assoziativität**  
- Beschreibung: Klammerreihenfolge ändert das Ergebnis nicht  
- Beispiel: (a + b) + c = a + (b + c)

**2. Kommutativität**  
- Beschreibung: Reihenfolge der Operanden ist egal  
- Beispiel: a * b = b * a

**3. Distributivität**  
- Beschreibung: Verknüpft zwei Operationen  
- Beispiel: 2 * (3 + 4) = 2 * 3 + 2 * 4

**4. Neutrales Element**  
- Beschreibung: Element, das den Wert nicht verändert  
- Beispiel: a + 0 = a, a * 1 = a

**5. Inverses Element**  
- Beschreibung: Element, das die Wirkung der Operation "aufhebt"  
- Beispiel:  
  - a + (−a) = 0  
  - a * (1/a) = 1

---

## 🧩 Algebraische Strukturen

### 🔹 Halbgruppe (Halbgruppe)  
- Bedingung: Assoziativität  
- Beispiel: (N, ·)

### 🔹 Monoid  
- Bedingung: Halbgruppe + neutrales Element  
- Beispiel: (N, ·, 1)

### 🔹 Gruppe  
- Bedingung: Monoid + inverse Elemente  
- Beispiel: (Z, +, 0, -x)

### 🔹 Kommutative Gruppe  
- Bedingung: Gruppe mit kommutativer Operation  
- Beispiel: (Z, +)

---

## 🧩 Weitere Strukturen

### 🔹 Ring  
- Bedingung: Kommutative Gruppe (Addition) + Halbgruppe (Multiplikation) + Distributivität  
- Beispiel: (Z, +, *)

### 🔹 Kommutativer Ring  
- Bedingung: Ring mit kommutativer Multiplikation  
- Beispiel: Z, Q, R

### 🔹 Ring mit Einselement  
- Bedingung: Ring mit multiplikativem Einselement (1)  
- Beispiel: (Z, +, *, 1)

### 🔹 Integritätsbereich  
- Bedingung: Kommutativer Ring mit 1 ohne Nullteiler  
- Beispiel: Z

### 🔹 Körper (Feld)  
- Bedingung: Kommutativer Ring mit 1, alle ≠ 0 Elemente sind invertierbar  
- Beispiel: Q, R, C

---

## 🔗 Struktur-Einschlusskette

```

Halbgruppe ⊂ Monoid ⊂ Gruppe ⊂ Kommutative Gruppe

Ring ⊂ Kommutativer Ring ⊂ Ring mit Einselement ⊂ Integritätsbereich ⊂ Körper

```

