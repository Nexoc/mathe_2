# 🔐 RSA – Komplettes Beispiel (Schritt für Schritt, GitHub-tauglich)

Dieses Beispiel zeigt, wie das RSA-Verschlüsselungsverfahren funktioniert – mit kleinen Zahlen und klaren Schritten.

---

## ✅ Schritt 1: Zwei Primzahlen wählen

Wir wählen:

- p = 5  
- q = 11

---

## ✅ Schritt 2: Modulus berechnen

k = p × q = 5 × 11 = 55

---

## ✅ Schritt 3: Eulersche Funktion berechnen

m = (p - 1) × (q - 1) = 4 × 10 = 40

---

## ✅ Schritt 4: Öffentlichen Exponenten wählen

Wir wählen e = 3, weil 3 und 40 teilerfremd sind (ggT = 1)

---

## ✅ Schritt 5: Privaten Schlüssel berechnen

Wir suchen d so, dass:

3 × d mod 40 = 1

Lösung: d = 27  
(denn 3 × 27 = 81 → 81 mod 40 = 1)

---

## ✅ Schritt 6: Schlüsselpaare

- Öffentlicher Schlüssel: (e = 3, k = 55)  
- Privater Schlüssel: (d = 27, k = 55)

---

## ✅ Schritt 7: Verschlüsselung

Klartext T = 9  
Verschlüsseln mit:

T⁽ᵉ⁾ mod k = 9³ mod 55

Berechnung:

9 × 9 = 81  
81 × 9 = 729  
729 mod 55 = 14

**Geheimtext = 14**

---

## ✅ Schritt 8: Entschlüsselung

Wir entschlüsseln G = 14 mit d = 27 und k = 55

Berechnung:

T = 14⁽²⁷⁾ mod 55

Da 14⁽²⁷⁾ zu groß ist, nutzen wir modulare Potenzierung in Schritten:

- 14² mod 55 = 196 mod 55 = 31  
- 14⁴ = 31² = 961 → mod 55 = 26  
- 14⁸ = 26² = 676 → mod 55 = 16  
- 14¹⁶ = 16² = 256 → mod 55 = 36

Jetzt kombinieren wir die Faktoren, die 14⁽²⁷⁾ ergeben:

14⁽²⁷⁾ = 14¹ × 14² × 14⁸ × 14¹⁶  
entspricht: 14 × 31 × 16 × 36

Berechnung:

- 36 × 16 = 576 → mod 55 = 26  
- 26 × 31 = 806 → mod 55 = 36  
- 36 × 14 = 504 → mod 55 = 9

**Ergebnis: T = 9**

---

## ✅ Zusammenfassung

| Bezeichnung       | Wert         |
|------------------|--------------|
| Primzahlen       | p = 5, q = 11 |
| Modulus          | 55           |
| Phi (m)          | 40           |
| Öffentlicher Exponent | 3       |
| Privater Exponent     | 27      |
| Klartext         | 9            |
| Geheimtext       | 14           |
| Entschlüsselung  | 9 ✅          |

RSA hat korrekt funktioniert ✔
