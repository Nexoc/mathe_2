### Definition der Eulerschen φ-Funktion

Die **Eulersche φ-Funktion**  ist **die Anzahl der natürlichen Zahlen von 1 bis \( m - 1 \)**,  
die **zu \( m \) teilerfremd** sind – also solcher Zahlen \( a \), für die gilt:

    ggT(a, m) = 1

---

### Berechnung von φ(m)

Wenn m eine Primfaktorzerlegung der Form  
m = p₁ᵏ¹ · p₂ᵏ² · ... · pₙᵏⁿ  
hat, dann gilt:

    φ(m) = m · (1 − 1/p₁) · (1 − 1/p₂) · ... · (1 − 1/pₙ)

---

### Beispiel:

m = 12 = 2² · 3

Dann:

    φ(12) = 12 · (1 − 1/2) · (1 − 1/3)  
          = 12 · 1/2 · 2/3  
          = 4

Es gibt also **4 Zahlen zwischen 1 und 11**, die zu 12 teilerfremd sind.

✅ Ergebnis: φ(12) = 4
