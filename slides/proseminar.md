---
_class: lead
paginate: true
_paginate: false
---

# **algebraische** und <br /> **transzendente** Zahlen

Jannik Wibker

---

## Wiederholung: **Monoid**

$(M, +)$ ist ein Monoid:

- Assoziativ: $a + (b + c) = (a + b) + c$
- neutrales Element $0$

---

## Wiederholung: **Gruppe**

$(G, +)$ ist eine Gruppe:

- Assoziativ: $a + (b + c) = (a + b) + c$
- neutrales Element $0$
- Inverses Element $-x$ für jedes $x$
<br />

**abelsch**, falls kommutativ: $a + b = b + a$

---

## Wiederholung: **Ring**

$(R, +, \cdot)$ ist ein Ring:

- $(R, +)$ abelsche Gruppe
- $(R, \cdot)$ Monoid
- Distributiv: $a \cdot (b + c) = a \cdot b + a \cdot c$
<br />

**Nullteilerfrei**, falls $a \cdot b = 0 \implies a = 0 \lor b = 0$
**Einheiten** $R^{\times}$ sind die invertierbaren Elemente von $R$

---

## Wiederholung: **Körper**

$(K, +, \cdot)$ ist ein Körper:

- $(K, +)$ abelsche Gruppe
- $(K, \cdot)$ abelsche Gruppe
- Distributiv: $a \cdot (b + c) = a \cdot b + a \cdot c$
<br />

**Körper** sind **nullteilerfrei** und $K^{\times} = K \setminus \lbrace 0 \rbrace$

---

## Polynomring

Für Ring $R$ ist $R[X]$ der **Polynomring** über $R$:
alle Polynome die Koeffizienten $a_i$ aus $R$ haben

---

## Polynomring

Für Ring $R$ ist $R[X]$ der **Polynomring** über $R$:
alle Polynome die Koeffizienten $a_i$ aus $R$ haben

$$\sum_{i=0}^{n} a_i \cdot X^i\qquad (a_i \in R)$$

---

## Polynomring

Für Ring $R$ ist $R[X]$ der **Polynomring** über $R$:
alle Polynome die Koeffizienten $a_i$ aus $R$ haben

$$\sum_{i=0}^{n} a_i \cdot X^i\qquad (a_i \in R)$$
<br />

Polynom **normiert**, falls $a_n = 1$
$R$ nullteilerfrei $\implies$ $R[X]$ nullteilerfrei

---

## Algebraische Zahlen

$\alpha$ ist **algebraisch**, falls es ein Polynom $p \in \mathbb{Q}[X] \setminus \lbrace 0 \rbrace$ gibt, sodass $p(\alpha) = 0$ ist.

Menge aller algebraischen Zahlen: $\mathbb{A}$
Nicht algebraische Zahlen heißen **transzendente** Zahlen

---

## **Bemerkung**:

$R$ Körper $\implies$ alle $f \in R[X] \setminus \lbrace 0 \rbrace$ können normiert werden.

---

## **Bemerkung**:

Sei $\alpha \in \mathbb{C}$ algebraisch, dann existiert ein **eindeutiges**, über $\mathbb{Q}$ **irreduzibles** und **normiertes** Polynom $p \in \mathbb{Q}[X] \setminus \lbrace 0 \rbrace$ mit $p(\alpha) = 0$.

---

## **Bemerkung**:

Sei $\alpha \in \mathbb{C}$ algebraisch, dann existiert ein **eindeutiges**, über $\mathbb{Q}$ **irreduzibles** und **normiertes** Polynom $p \in \mathbb{Q}[X] \setminus \lbrace 0 \rbrace$ mit $p(\alpha) = 0$.

## **Beweis**:

1. **Existenz** und **Irreduzibilität**
2. **Normiertheit**
3. **Eindeutigkeit**

---

## Minimalpolynom

Für $\alpha \in \mathbb{C}$ heißt $p \in \mathbb{Q}[X]$ **Minimalpolynom** (von $\alpha$), falls

- $p(\alpha) = 0$
- $p$ irreduzibel
- $p$ normiert

---

## Minimalpolynom

Für $\alpha \in \mathbb{C}$ heißt $p \in \mathbb{Q}[X]$ **Minimalpolynom** (von $\alpha$), falls

- $p(\alpha) = 0$
- $p$ irreduzibel
- $p$ normiert

Für $\alpha \in \mathbb{C}$ sagt man, dass es **algebraisch vom Grad n** ist, falls $\text{deg}(p) = n$.
Falls Minimalpolynom $p \in \mathbb{Z}[X]$ ist, sagt man $\alpha \in \mathbb{C}$ ist **ganz-algebraisch**.

---

## Beispiele:

- $\tfrac{a}{b} \in \mathbb{Q}$
- $\sqrt{n}$ für $n \in \mathbb{N}$

---

## **Bemerkung**:

Zu jedem $\alpha \in \mathbb{C}$ algebraisch kann man $d \in \mathbb{N}$ finden, sodass $d \cdot \alpha$ ganz-algebraisch.

---

## Konjugierte von algebraischen Zahlen

Falls das MP $p$ für ein $\alpha \in \mathbb{C}$ zerfällt in:

$$p(X) = (X-\alpha_1) \cdot \dots \cdot (X-\alpha_n)$$

für $n = \text{deg}(p), \alpha_i \in \mathbb{C}, \alpha_1 = \alpha$ dann nennt man $\lbrace \alpha_1, \dots, \alpha_n \rbrace$ die **Konjugierten** von $\alpha$.

---

## **Bemerkung**:

Die Konjugierten von $\alpha$ sind paarweise disjunkt

---

## **Bemerkung**:

Algebraische Zahlen bilden einen Körper (mit gewöhnlicher Addition und Multiplikation)

---

## Satz von Cantor

Die Menge der algebraischen Zahlen ist abzählbar

---

## Satz von Liouville

Sei $\alpha$ algebraisch vom Grad $n > 1$ und $\alpha \notin \mathbb{Q}$.

Dann existiert $c \in \mathbb{R}^{+}$ mit:

$$\vert \alpha - \tfrac{p}{q} \vert > \tfrac{c}{q^n}$$

für alle $\tfrac{p}{q} \in \mathbb{Q}$

---

## Wiederholung: **Mittelwertsatz**

![bg right:45% fit](./assets/mittelwertsatz.svg)

Seien $a < b$,
$f: [a, b] \to \mathbb{R}$ stetig,
$f$ differenzierbar auf $(a, b)$

Dann existiert ein $\xi \in (a, b)$ mit $f'(\xi) = \tfrac{f(b) - f(a)}{b - a}$

---
