# 🔍 Eigenwerte und Eigenvektoren berechnen (Beispiel)

Gegeben sei die Matrix:

```

A = [ 2  1 ]
    [ 1  2 ]

```

---

## 🧮 Schritt 1: Eigenwerte berechnen

Berechne das charakteristische Polynom:

```

det(A − λI) = 0

```

Subtrahiere λ auf der Hauptdiagonale:

```

A − λI =
    [ 2−λ  1   ]
    [ 1    2−λ ]

```

Berechne den Determinanten:

```

det(A − λI) = (2−λ)² − 1 = λ² − 4λ + 3

```

Löse:

```

λ² − 4λ + 3 = 0
⇒ λ₁ = 1, λ₂ = 3

```

---

## 🧭 Schritt 2: Eigenvektoren berechnen

### Für λ = 1:

Einsetzen in `(A − λI) ⋅ x = 0`:

```

A − I =
    [ 1  1 ]
    [ 1  1 ]

```

LGS:

```

x + y = 0 ⇒ y = −x

```

Eigenvektor:

```

v₁ = [  1 ]
     [ −1 ]

```

---

### Für λ = 3:

```

A − 3I =
    [ −1  1 ]
    [  1 −1 ]

```

LGS:

```

x − y = 0 ⇒ y = x

```

Eigenvektor:

```

v₂ = [ 1 ]
     [ 1 ]

```

---

## ✅ Ergebnisübersicht

| Eigenwert λ | Eigenvektor                 |
|-------------|-----------------------------|
| 1           | `[ 1 , −1 ]ᵀ`                |
| 3           | `[ 1 ,  1 ]ᵀ`                |

---

**Hinweis:** Jeder Eigenvektor kann beliebig skaliert werden, da die Lösung nur bis auf einen konstanten Faktor eindeutig ist.



