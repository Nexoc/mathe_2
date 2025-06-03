## Chinesischer Restsatz

### Problemstellung

Gegeben ist ein System von Kongruenzen:

```text
x ≡ a₁ mod m₁
x ≡ a₂ mod m₂
...
x ≡ aₖ mod mₖ
```

**Voraussetzung:**
Die Moduli `m₁, m₂, ..., mₖ` sind **paarweise teilerfremd**, also `ggT(mᵢ, mⱼ) = 1` für alle `i ≠ j`.

Dann existiert genau **eine Lösung modulo M**, wobei:

```text
M = m₁ × m₂ × ... × mₖ
```

## Beispiel

Finde `x` mit:

```text
x ≡ 2 mod 3
x ≡ 3 mod 4
x ≡ 2 mod 5
```

---

###  Rechenschritte

| Bezeichnung | Rechnung  | Ergebnis |
| ----------- | --------- | -------- |
| M           | 3 × 4 × 5 | 60       |
| M₁          | 60 ÷ 3    | 20       |
| M₂          | 60 ÷ 4    | 15       |
| M₃          | 60 ÷ 5    | 12       |

Finde nun das **modulare Inverse** `yᵢ`, sodass:

```text
Mᵢ × yᵢ ≡ 1 mod mᵢ
```

| Gleichung         | Lösung |
| ----------------- | ------ |
| 20 × y₁ ≡ 1 mod 3 | y₁ = 2 |
| 15 × y₂ ≡ 1 mod 4 | y₂ = 3 |
| 12 × y₃ ≡ 1 mod 5 | y₃ = 3 |

---

### Endformel:

```text
x ≡ a₁·M₁·y₁ + a₂·M₂·y₂ + a₃·M₃·y₃ mod M
x ≡ 2·20·2 + 3·15·3 + 2·12·3
x ≡ 80 + 135 + 72 = 287
x ≡ 287 mod 60 = 47
```

---

### Ergebnis

```text
x ≡ 47 mod 60
```

---

### 🛠 Anwendungsbereiche

* Zahlentheorie
* Kryptographie (z. B. RSA)
* Gleichungen mit mehreren Moduli
* Uhrzeit-/Kalenderprobleme
* Parallele Rechenprozesse
