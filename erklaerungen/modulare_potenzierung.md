# 🔢 Beispiel: Berechne 3^57 mod 11 (mit Binärzerlegung und Mod-Potenzierung)

---

## Schritt 1: Zerlege 57 in Binärform

57 = 1 1 1 0 0 1

Tabelle:

```

64  32  16  8   4   2   1
0   1   1  1   0   0   1

```

Also:  
57 = 32 + 16 + 8 + 1 = 2^5 + 2^4 + 2^3 + 2^0

---

## Schritt 2: Baue Tabelle für Potenzen von 3 mod 11

| k | 2^k | 3^(2^k)         | Ergebnis mod 11 |
|---|-----|------------------|-----------------|
| 0 | 1   | 3                | 3               |
| 1 | 2   | 3^2 = 9          | 9               |
| 2 | 4   | 9^2 = 81         | 81 mod 11 = 4   |
| 3 | 8   | 4^2 = 16         | 16 mod 11 = 5   |
| 4 | 16  | 5^2 = 25         | 25 mod 11 = 3   |
| 5 | 32  | 3^2 = 9          | 9               |

---

## Schritt 3: Wähle nur die Potenzen, die in 57 vorkommen

57 = 2^5 + 2^4 + 2^3 + 2^0  
→ also brauchen wir:

3^32, 3^16, 3^8, 3^1

Diese Werte aus der Tabelle:

- 3^32 mod 11 = 9  
- 3^16 mod 11 = 3  
- 3^8  mod 11 = 5  
- 3^1  mod 11 = 3

---

## Schritt 4: Multipliziere alle relevanten Werte

```

3^57 mod 11 =
\= 9 \* 3 \* 5 \* 3 mod 11
\= 27 \* 15 mod 11

```

Jetzt Schritt für Schritt:

- 27 mod 11 = 5  
- 15 mod 11 = 4  
- 5 * 4 = 20  
- 20 mod 11 = 9 ✅

---

## Ergebnis:

**3^57 mod 11 = 9**

Funktioniert ✔



![alt text](./img/pot.png)