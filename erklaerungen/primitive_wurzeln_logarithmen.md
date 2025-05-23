# 🔁 Primitive Wurzeln und diskrete Logarithmen (mod 7)

---

## 📌 Was ist eine primitive Wurzel?

Ein Element `a` ist eine primitive Wurzel modulo `n`, wenn die Potenzen  
`a¹, a², ..., a^φ(n)` (mod n) **alle Zahlen von 1 bis n−1** abdecken.

Das heißt: `a` erzeugt die ganze multiplikative Gruppe `Zₙ*`.

---

## ❌ Beispiel 1: a = 2 in Z₇*

Berechne die Potenzen von 2 mod 7:

```

2⁰ = 1
2¹ = 2
2² = 4
2³ = 8 ≡ 1 mod 7
2⁴ = 2
2⁵ = 4
2⁶ = 1

```

Menge der Ergebnisse: {1, 2, 4}  
→ Nur 3 verschiedene Werte

**Fazit:**  
ord₇(2) = 3 < φ(7) = 6  
➡️ 2 ist **keine primitive Wurzel**

---

## ✅ Beispiel 2: a = 3 in Z₇*

Berechne die Potenzen von 3 mod 7:

```

3⁰ = 1
3¹ = 3
3² = 9 ≡ 2 mod 7
3³ = 6
3⁴ = 4
3⁵ = 5
3⁶ = 15 ≡ 1 mod 7

```

Menge der Ergebnisse: {1, 2, 3, 4, 5, 6}  
→ Alle Werte von `Z₇*`

**Fazit:**  
ord₇(3) = 6 = φ(7)  
➡️ 3 ist eine **primitive Wurzel**

---

## 🔁 Diskreter Logarithmus zur Basis 3 (mod 7)

Wenn `3ⁱ ≡ j mod 7`, dann gilt:  
`log₃(j) = i` mod 7

| i (Exponent) | 3ⁱ mod 7 |
|--------------|-----------|
| ⁰            | 1         |
| ¹            | 3         |
| ²            | 2         |
| ³            | 6         |
| ⁴            | 4         |
| ⁵            | 5         |

---

## 🔄 Umgekehrt: log₃(j) mod 7

| j ∈ Z₇* | log₃(j) |
|---------|---------|
| 1       | ⁰       |
| 2       | ²       |
| 3       | ¹       |
| 4       | ⁴       |
| 5       | ⁵       |
| 6       | ³       |

Diese Tabelle zeigt:  
→ Jede Zahl hat einen eindeutigen diskreten Logarithmus zur Basis 3

---

## 🚫 Warum geht das nicht mit a = 2?

Für `a = 2` waren die Potenzen:

```

2⁰ = 1
2¹ = 2
2² = 4
2³ = 1 ...

```

→ Es entstehen nur die Werte {1, 2, 4}  
→ Viele Zahlen (z. B. 3, 5, 6) **kann man gar nicht erreichen**

➡️ Diskrete Logarithmen **nicht eindeutig bestimmbar**  
➡️ Nur primitive Wurzeln erlauben vollständige Logarithmentabellen

---

## ✅ Zusammenfassung

| Basis a | Ordnung | Primitive Wurzel? | Vollständiger Logarithmus? |
|---------|---------|-------------------|-----------------------------|
| 2       | 3       | ❌ Nein           | ❌ Nur teilweise möglich    |
| 3       | 6       | ✅ Ja             | ✅ Für alle Werte in Z₇*    |
```
