## Warum potenzieren wir beide Seiten mit e?

Gegeben ist die Gleichung:

    x⁹ ≡ 3 mod 17

Ziel: Wir wollen x bestimmen.

---

### ❌ Problem:

In der normalen Mathematik würden wir schreiben:

    x⁹ = 3  ⇒  x = ⁹√3

Aber im modularen Rechnen gibt es **keine Wurzel-Funktion**.  
Wir können **nicht einfach "durch 9 teilen"** oder eine Wurzel ziehen.

---

### ✅ Was geht stattdessen?

In der Modulo-Arithmetik können wir:

- multiplizieren  
- potenzieren  
- und: **mit inversen Potenzen** arbeiten

Wenn wir also ein e finden, sodass gilt:

    9 · e ≡ 1 mod φ(17) = 16

dann können wir beide Seiten der Gleichung mit e potenzieren, um:

    (x⁹)ᵉ ≡ 3ᵉ mod 17
⇒  x⁸¹ ≡ 3ᵉ mod 17

---

### 🧠 Warum hilft das?

Da φ(17) = 16, gilt für alle x ∈ ℤ₁₇*:

    x¹⁶ ≡ 1 mod 17

Weil:

    81 ≡ 1 mod 16  (denn 81 = 5·16 + 1)

gilt:

    x⁸¹ ≡ x mod 17

---

### 🔚 Und damit:

    x ≡ 3⁹ mod 17

---

### 📝 Fazit:

Wir potenzieren beide Seiten mit e,  
**um die ursprüngliche Potenz (⁹) auf der linken Seite aufzuheben**  
und **x direkt zu isolieren**.

Das funktioniert genau dann, wenn:

    e ≡ 9⁻¹ mod φ(17)
