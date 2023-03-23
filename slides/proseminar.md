---
_class: lead
paginate: true
_paginate: false
---

# **algebraische** und <br /> **transzendente** Zahlen

Janina Wibker

---

## Algebraische Zahlen

$\alpha$ ist **algebraisch**, falls es ein Polynom $p \in \mathbb{Q}[X] \setminus \lbrace 0 \rbrace$ gibt, sodass $p(\alpha) = 0$ ist.

Menge aller algebraischen Zahlen: $\mathbb{A}$
Nicht algebraische Zahlen heißen **transzendente** Zahlen

---



## **Bemerkung**:

Sei $\alpha \in \mathbb{C}$ algebraisch, dann existiert ein **eindeutiges**, über $\mathbb{Q}$ **irreduzibles** und **normiertes** Polynom $p \in \mathbb{Q}[X] \setminus \lbrace 0 \rbrace$ mit $p(\alpha) = 0$.

---

## **Definition**: Irreduzibilität

Ein Polynom $f$ ist irreduzibel (über einem Körper), falls es nicht als $f = p \cdot q$ geschrieben werden kann, wobei

$$\text{deg}(p), \text{deg}(q) < \text{deg}(f)$$

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

## Satz von Cantor

Die Menge der algebraischen Zahlen ist abzählbar

---

## Satz von Cantor

Die Menge der algebraischen Zahlen ist abzählbar

$$N(\sum_{i=0}^{n} a_i \cdot x^i) = \vert n \vert + \sum_{i=0}^{n} \vert a_i \vert$$

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

## **Lemma**

Seien $n \in \mathbb{N}$, $a_i \in \mathbb{Z}$ für $i \in \lbrace 0, \dots, n \rbrace$ und

$$
\begin{alignedat}{3}
&f: \mathbb{C} \to \mathbb{C}, \;&f(z) &= \sum_{i=0}^n a_i \cdot z^i \\
&F: \mathbb{C} \to \mathbb{C}, \;&F(z) &= \sum_{l=0}^n f^{(l)}(z)
\end{alignedat}
$$

Dann: $\displaystyle{\vert F(0) \cdot e^z - F(z) \vert \;\le\; e^{\vert z \vert} \cdot \sum_{i=0}^{n} \vert a_i \vert \cdot {\vert z \vert}^i \qquad (\forall z \in \mathbb{C})}$

---

## **Satz**: $e$ ist transzendent

**Aufbau**:
- Annahme $e$ hat MP
- Finde für ein definiertes $\Sigma_p$ zwei Abschätzungen
- Zeige diese Abschätzungen sind widersprüchlich für groß genug gewähltes $p \in \mathbb{P}$
- $\implies$ $e$ hat doch kein MP

---

## **Satz**: $e$ ist transzendent

Angenommen $e$ hat MP:

$$g: \mathbb{C} \to \mathbb{C}, \quad g(x) = \sum_{j=0}^{m} \tfrac{b_j}{b_m} \cdot x^j$$

Für $b_j \in \mathbb{Z}$ und $b_m \in \mathbb{N}$

Es gilt $g(e) = 0$ und, dass $g$ normiert ist

---

## **Satz**: $e$ ist transzendent

Definiere für alle $p \in \mathbb{P}$

$$
\begin{alignedat}{1}
&f_p: \mathbb{C} \to \mathbb{C}, \quad f_p(x) = x^{p-1} \cdot \prod_{j=1}^{m} (j-x)^p \qquad \in \mathbb{Z}[X] \\
&n_p = (m + 1)p - 1 \\
&a_{p,p-1} = (m!)^p
\end{alignedat}
$$

---

## **Satz**: $e$ ist transzendent

Darstellungen von $f_p(x)$

- $f_p(x) = x^{p-1} \cdot \prod_{j=1}^{m} (j-x)^p$
  <br />
- $f_p(x) = a_{p,p-1} \cdot x^{p-1} + a_{p,p} \cdot x^{p} + \dots + a_{p,n_p} \cdot x^{n_p}$
  für gewisse $a_{p,n} \in \mathbb{Z}$ und $a_{p,p-1} = (m!)^p$
  ("Ausmultiplizieren")

---

## Wiederholung: **Taylorentwicklung**

$$T_{f(x; a)} = \sum_{n=0}^{\infty} \tfrac{f^{(n)}(a)}{n!} \cdot (x-a)^n = \sum_{n=0}^{\infty} t_n \cdot (x-a)^n$$

ist die Taylorentwicklung von $f$ um $a$ ausgewertet für $x$.
<br />
Inbesondere gleicht für Polynome die Taylorentwicklung dem Polynom.

---

## **Satz**: $e$ ist transzendent

Darstellungen von $f_p(x)$

- $f_p(x) = x^{p-1} \cdot \prod_{j=1}^{m} (j-x)^p$
  <br />
- $f_p(x) = a_{p,p-1} \cdot x^{p-1} + a_{p,p} \cdot x^{p} + \dots + a_{p,n_p} \cdot x^{n_p}$
  <br />
- $\displaystyle{f_p(x) = \sum_{n = p}^{n_p} a_{p,j,n} \cdot (x-j)^n}$ für alle $j \in \lbrace 1, \dots, m \rbrace$,
  gewisse $a_{p,j,n} \in \mathbb{Z}$

---

## **Satz**: $e$ ist transzendent

Definiere

$$
\begin{alignedat}{2}
  &F_p: \mathbb{C} \to \mathbb{C}, \;&F_p(x) &= \sum_{l=0}^{n_p} f_p^{(l)}(x) \\
  &G_p: \mathbb{C} \to \mathbb{C}, \;&G_p(x) &= F_p(0) \cdot e^x - F_p(x)
\end{alignedat}
$$

---

## **Satz**: $e$ ist transzendent

Sei

$$
\Sigma_p 
  := \fcolorbox{transparent}{transparent}{$\displaystyle{\sum_{j=0}^{m} b_j \cdot F_p(j)}$}
   = \fcolorbox{transparent}{transparent}{$\displaystyle{- \sum_{j=0}^{m} b_j \cdot G_p(j)}$}
$$

---

## **Satz**: $e$ ist transzendent

Betrachte

$$
\Sigma_p 
  := \fcolorbox{black}{transparent}{$\displaystyle{\sum_{j=0}^{m} b_j \cdot F_p(j)}$}
   = \fcolorbox{transparent}{transparent}{$\displaystyle{- \sum_{j=0}^{m} b_j \cdot G_p(j)}$}
$$

---

## **Satz**: $e$ ist transzendent

$$
\sum_{j=0}^{m} b_j \cdot F_p(j)
  = \fcolorbox{var(--color-highlight-secondary)}{transparent}{$\displaystyle{  b_0 \cdot \sum_{l=0}^{n_p} f^{(l)}(0)  }$}
  + \fcolorbox{var(--color-accent)}{transparent}{$\displaystyle{  \sum_{j=1}^{m} b_j \cdot \sum_{l=0}^{n_p} f^{(l)}(j)  }$}
$$

---

## **Satz**: $e$ ist transzendent

$$
\sum_{j=0}^{m} b_j \cdot F_p(j)
  = \fcolorbox{var(--color-highlight-secondary)}{transparent}{$\displaystyle{  b_0 \cdot \sum_{l=0}^{n_p} f^{(l)}(0)  }$}
  + \fcolorbox{var(--color-accent)}{transparent}{$\displaystyle{  \sum_{j=1}^{m} b_j \cdot \sum_{l=0}^{n_p} f^{(l)}(j)  }$}
$$

$$
\fcolorbox{var(--color-accent)}{transparent}{$\displaystyle{
  \sum_{j=1}^{m} b_j \cdot \sum_{l=0}^{n_p} f^{(l)}(j) = 
  \sum_{j=1}^{m} b_j \cdot \sum_{l=p}^{n_p} a_{p,j,l} \cdot l!
}$}
$$

---

## **Satz**: $e$ ist transzendent

$$
\sum_{j=0}^{m} b_j \cdot F_p(j)
  = \fcolorbox{var(--color-highlight-secondary)}{transparent}{$\displaystyle{  b_0 \cdot \sum_{l=0}^{n_p} f^{(l)}(0)  }$}
  + \fcolorbox{var(--color-accent)}{transparent}{$\displaystyle{  \sum_{j=1}^{m} b_j \cdot \sum_{l=0}^{n_p} f^{(l)}(j)  }$}
$$

$$
\fcolorbox{var(--color-highlight-secondary)}{transparent}{$\displaystyle{
  b_0 \cdot \sum_{l=0}^{n_p} f^{(l)}(0) =
  b_0 \cdot \sum_{l=p-1}^{n_p} a_{p,l} \cdot l!
}$}
$$

---

## **Satz**: $e$ ist transzendent

Somit:

$$\Sigma_p = b_0 \cdot (m!)^p \cdot (p-1)! + a_p \cdot p!$$

für ein $a_p \in \mathbb{Z}$

---

## **Satz**: $e$ ist transzendent

Somit:

$$\vert \Sigma_p \vert \ge (p-1)!$$

für $p \in \mathbb{P} > \text{max}\lbrace m, \vert b_0 \vert \rbrace$

---

## **Satz**: $e$ ist transzendent

Betrachte

$$
\Sigma_p 
  := \fcolorbox{transparent}{transparent}{$\displaystyle{\sum_{j=0}^{m} b_j \cdot F_p(j)}$}
   = \fcolorbox{black}{transparent}{$\displaystyle{- \sum_{j=0}^{m} b_j \cdot G_p(j)}$}
$$

---

## **Satz**: $e$ ist transzendent

Wir hatten

$$(p-1)! \quad\le\quad \vert \Sigma_p \vert \quad\le\quad C_g \cdot D_m^p$$

---

## **Satz**: $e$ ist transzendent

Wir hatten

$$(p-1)! \quad\le\quad \vert \Sigma_p \vert \quad\le\quad C_g \cdot D_m^p$$

Aber es gibt $N_0 \in \mathbb{N}$, sodass $\forall N \ge N_0$ gilt:

$$(N-1)! \quad\ge\quad {\Big( \dfrac{N}{3}\Big)}^{\frac{N}{2}} \quad>\quad C_g \cdot D_m^N$$

---

## **Satz**: $e$ ist transzendent

**Widerspruch** ⚡️

$\implies$ $e$ hat doch kein MP

$\implies$ $e$ ist transzendent 🎉

---

<!--
_class: lead
_paginate: false
-->

# **Vielen Dank für die<br /> Aufmerksamkeit!**

## Any questions?
