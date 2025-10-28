\pagebreak

# Análisis en $\mathbb{R}$

Los números reales forman una estructura algebraica con operaciones de suma y producto, y una relación de orden que cumple ciertas propiedades fundamentales. A continuación se presentan los axiomas y teoremas más importantes que caracterizan a $\mathbb{R}$.

## Construcción Axiomática

\begin{axiom}[Conmutatividad de la suma]
Para todo $a,b \in \mathbb{R}$: $a + b = b + a$
\end{axiom}

\begin{axiom}[Asociatividad de la suma]
Para todo $a,b,c \in \mathbb{R}$: $(a + b) + c = a + (b + c)$
\end{axiom}

\begin{axiom}[Elemento neutro de la suma]
Existe $0 \in \mathbb{R}$ tal que para todo $a \in \mathbb{R}$: $a + 0 = 0 + a = a$
\end{axiom}

\begin{axiom}[Elemento opuesto de la suma]
Para todo $a \in \mathbb{R}$ existe $(-a) \in \mathbb{R}$ tal que: $a + (-a) = 0$
\end{axiom}

\begin{axiom}[Conmutatividad del producto]
Para todo $a,b \in \mathbb{R}$: $a \cdot b = b \cdot a$
\end{axiom}

\begin{axiom}[Asociatividad del producto]
Para todo $a,b,c \in \mathbb{R}$: $(a \cdot b) \cdot c = a \cdot (b \cdot c)$
\end{axiom}

\begin{axiom}[Elemento neutro del producto]
Existe $1 \in \mathbb{R}$ tal que para todo $a \in \mathbb{R}$: $a \cdot 1 = 1 \cdot a = a$
\end{axiom}

\begin{axiom}[Elemento inverso del producto]
Para todo $a \neq 0$ existe $a^{-1} \in \mathbb{R}$ tal que: $a \cdot a^{-1} = 1$
\end{axiom}

\begin{axiom}[Distributividad]
Para todo $a,b,c \in \mathbb{R}$: $a(b + c) = ab + ac$
\end{axiom}

\begin{axiom}[Reflexividad del orden]
Para todo $a \in \mathbb{R}$: $a \leq a$
\end{axiom}

\begin{axiom}[Antisimetría del orden]
Para todo $a,b \in \mathbb{R}$: $a \leq b \land b \leq a \Rightarrow a = b$
\end{axiom}

\begin{axiom}[Transitividad del orden]
Para todo $a,b,c \in \mathbb{R}$: $a \leq b \land b \leq c \Rightarrow a \leq c$
\end{axiom}

\begin{axiom}[Compatibilidad del orden con la suma]
Para todo $a,b,c \in \mathbb{R}$: $a \leq b \Rightarrow a + c \leq b + c$
\end{axiom}

\begin{axiom}[Compatibilidad del orden con el producto]
Para todo $a,b,c \in \mathbb{R}$: $a \leq b \land c \geq 0 \Rightarrow ac \leq bc$
\end{axiom}

\begin{axiom}[Completitud]
Todo conjunto no vacío de números reales que está acotado superiormente tiene un supremo en $\mathbb{R}$.
\end{axiom}

## Valor Absoluto

\begin{theorem}[Definición de Valor Absoluto]
El valor absoluto de un número real $a$ se define como:

$$|a| = \begin{cases} a, & a \ge 0 \\ -a, & a < 0 \end{cases}$$

\end{theorem}

\begin{theorem}[Caracterización del Valor Absoluto]
Para $a \in \mathbb{R}$ y $b \ge 0$,
$|a| \le b \Leftrightarrow -b \le a \le b$.
\end{theorem}

\begin{theorem}[Multiplicatividad del Valor Absoluto]
Para todo $a,b \in \mathbb{R}$,
$|ab| = |a| \cdot |b|$.
\end{theorem}

\begin{theorem}[Cociente del Valor Absoluto]
Para todo $a, b \in \mathbb{R}$ con $b \neq 0$,
$\left|\frac{a}{b}\right| = \frac{|a|}{|b|}$.
\end{theorem}

\begin{theorem}[Cota Inferior del Valor Absoluto]
Para todo $a \in \mathbb{R}$, $a \le |a|$.
\end{theorem}

\begin{theorem}[Desigualdad del triángulo invertida]
Para todo $a, b \in \mathbb{R}$,
$||a| - |b|| \le |a - b|$.
\end{theorem}

\begin{theorem}[Desigualdad triangular]
Para todo $a, b \in \mathbb{R}$,
$|a + b| \le |a| + |b|$.
\end{theorem}

## Sucesiones

\begin{definition}[Sucesión]
Una sucesión $(a_n)$ es una función $a:\mathbb{N}_0 \to \mathbb{R}$.
\end{definition}

\begin{definition}[Límite de sucesión]
$\displaystyle \lim_{n \to \infty} a_n = l$ si $\forall \varepsilon > 0, \exists n_0 \in \mathbb{N}$ tal que $n \ge n_0 \Rightarrow |a_n - l| < \varepsilon$.
\end{definition}

\begin{theorem}[Unicidad del límite]
Si una sucesión tiene límite, este es único.
\end{theorem}

\begin{definition}[Sucesión acotada]
Una sucesión $(a_n)$ es acotada si $\exists M > 0$ tal que $|a_n| < M$ para todo $n \in \mathbb{N}$.
\end{definition}

\begin{theorem}[Condición necesaria de convergencia]
Si una sucesión $(a_n)$ converge, entonces es acotada.
\end{theorem}

\begin{theorem}[Teorema del Sandwich para sucesiones]
Si $(a_n)$, $(b_n)$, $(c_n)$ son sucesiones tales que $\displaystyle \lim_{n \to \infty} a_n = \lim_{n \to \infty} c_n = l$ y $a_n \le b_n \le c_n$, entonces $\displaystyle \lim_{n \to \infty} b_n = l$.
\end{theorem}

\begin{theorem}[Álgebra de límites de sucesiones]
Sean $(a_n)$, $(b_n)$ sucesiones convergentes con límites $l_1, l_2$:
\begin{enumerate}
\item $\lim(a_n + b_n) = l_1 + l_2$
\item $\lim(a_n b_n) = l_1 l_2$
\item $\lim(k a_n) = k l_1$
\item $\lim\left(\frac{a_n}{b_n}\right) = \frac{l_1}{l_2}$, si $l_2 \neq 0$
\item $\lim |a_n| = |l_1|$
\end{enumerate}
\end{theorem}

\begin{definition}[Sucesión monótona]
Una sucesión es monótona si es creciente ($a_n \le a_{n+1}$) o decreciente ($a_n \ge a_{n+1}$).
\end{definition}

\begin{theorem}[Convergencia de sucesiones monótonas]
Si una sucesión es monótona y acotada, entonces converge.
\end{theorem}

\begin{theorem}[Teorema de Bolzano-Weierstrass]
Toda sucesión acotada en $\mathbb{R}$ tiene una subsucesión convergente.
\end{theorem}

\begin{theorem}[Criterio de Cauchy]
Una sucesión $(a_n)$ es convergente si y solo si es de Cauchy, es decir:
$$\forall \varepsilon > 0, \exists N \in \mathbb{N} : \forall n,m \geq N, |a_n - a_m| < \varepsilon$$
\end{theorem}

\begin{theorem}[Teorema de Heine-Borel]
Un subconjunto de $\mathbb{R}$ es compacto si y solo si es cerrado y acotado.
\end{theorem}

## Límites y Continuidad

\begin{definition}[Límite de una función]
Sea $f:(a,b)\to\mathbb{R}$, se dice que $\displaystyle \lim_{x \to a} f(x) = l$ si 
$\forall \varepsilon > 0, \exists \delta > 0$ tal que 
$0 < |x - a| < \delta \Rightarrow |f(x) - l| < \varepsilon$.
\end{definition}

\begin{theorem}[Unicidad del límite funcional]
Si una función tiene límite en un punto, este es único.
\end{theorem}

\begin{theorem}[Álgebra de límites funcionales]
Sean $f, g$ funciones tales que $\lim_{x \to a} f(x) = l_1$ y $\lim_{x \to a} g(x) = l_2$. Entonces:
\begin{enumerate}
\item $\lim_{x \to a} (f(x) + g(x)) = l_1 + l_2$
\item $\lim_{x \to a} (f(x) g(x)) = l_1 l_2$
\item Si $l_2 \ne 0$, entonces $\lim_{x \to a} \frac{f(x)}{g(x)} = \frac{l_1}{l_2}$
\end{enumerate}
\end{theorem}

\begin{definition}[Continuidad]
Sea $f:(a,b)\to\mathbb{R}$ y $x_0\in(a,b)$, se dice que $f$ es continua en $x_0$ si $\lim_{x \to x_0} f(x) = f(x_0)$.
\end{definition}

\begin{theorem}[Composición de funciones continuas]
Si $g$ es continua en $x_0$ y $f$ es continua en $g(x_0)$, entonces $f \circ g$ es continua en $x_0$.
\end{theorem}

\begin{theorem}[Teorema del Valor Intermedio]
Sea $f:[a,b] \to \mathbb{R}$ una función continua. Si $f(a) \neq f(b)$ y $k$ es un número entre $f(a)$ y $f(b)$, entonces existe $c \in (a,b)$ tal que $f(c) = k$.

\begin{proof}
Sin pérdida de generalidad, supongamos que $f(a) < k < f(b)$. Definimos el conjunto:

$$A = \{x \in [a,b] : f(x) \leq k\}$$

1) $A$ es no vacío pues $a \in A$ ya que $f(a) < k$.

2) $A$ está acotado superiormente por $b$ pues $f(b) > k$.

3) Por el axioma de completitud, existe $c = \sup A$.

4) Veamos que $f(c) = k$:

   Supongamos que $f(c) < k$. Por la continuidad de $f$ en $c$, existe $\delta > 0$ tal que:
   $$|x-c| < \delta \Rightarrow |f(x) - f(c)| < k - f(c)$$
   
   En particular, para $x = c + \frac{\delta}{2}$:
   $$f(x) < f(c) + (k - f(c)) = k$$
   
   Por lo tanto $x \in A$, pero $x > c$, contradiciendo que $c$ es el supremo de $A$.

   De manera similar, si $f(c) > k$, por continuidad existiría un punto antes de $c$ donde $f$ tomaría valores mayores que $k$, contradiciendo la definición de $A$.

Por lo tanto, necesariamente $f(c) = k$.
\end{proof}\end{theorem}

\begin{theorem}[Teorema de Weierstrass]
Toda función continua en un intervalo cerrado y acotado $[a,b]$ alcanza su máximo y su mínimo en ese intervalo.
\end{theorem}

\begin{theorem}[Teorema del Valor Medio]
Sea $f:[a,b] \to \mathbb{R}$ una función continua en $[a,b]$ y derivable en $(a,b)$. Entonces existe $c \in (a,b)$ tal que:
$$f'(c) = \frac{f(b) - f(a)}{b - a}$$
\end{theorem}

\begin{theorem}[Teorema Fundamental del Cálculo]
Sea $f:[a,b] \to \mathbb{R}$ una función continua. Entonces:
\begin{enumerate}
\item La función $F(x) = \int_a^x f(t) \, dt$ es derivable en $[a,b]$ y $F'(x) = f(x)$ para todo $x \in [a,b]$.
\item Si $G$ es una primitiva de $f$ en $[a,b]$, entonces:
$$\int_a^b f(x) \, dx = G(b) - G(a)$$
\end{enumerate}
\end{theorem}

## Exponenciales y Logaritmos

\begin{definition}[Exponencial - definición inductiva]
Para $a \in \mathbb{R}$ y $n \in \mathbb{N}$:
\begin{enumerate}
\item $a^0 = 1$
\item $a^{n+1} = a^n \cdot a$, $n \ge 0$
\item $a^{-n} = 1 / a^n$
\end{enumerate}
\end{definition}

\begin{definition}[Exponencial - extensión a racionales]
Para $a > 0$ y $m,n \in \mathbb{Z}, n \neq 0$:
$$a^{m/n} = \sqrt[n]{a^m}$$
\end{definition}

\begin{theorem}[Propiedades del exponente racional]
Para $a,b > 0$ y $r,s \in \mathbb{Q}$:
\begin{enumerate}
\item $a^r a^s = a^{r+s}$
\item $(a^r)^s = a^{rs}$
\item $a^r / a^s = a^{r-s}$
\item $(ab)^r = a^r b^r$
\item $a^1 = a$, $a^0 = 1$
\end{enumerate}
\end{theorem}

\begin{definition}[Exponencial - exponente real]
Para $a > 0$ y $r \in \mathbb{R}$:
$$a^r = \sup\{a^q : q \in \mathbb{Q}, q < r\} = \inf\{a^q : q \in \mathbb{Q}, q > r\}$$
\end{definition}

\begin{definition}[El número e]
$$e = \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n$$
donde $2 < e < 3$
\end{definition}

\begin{definition}[Logaritmo natural]
Para $y > 0$:
$$\log(y) = \sup\{x \in \mathbb{R} : e^x < y\}$$
Es la función inversa de $e^x$.
\end{definition}

\begin{theorem}[Propiedades del logaritmo]
Para $a,b > 0$:
\begin{enumerate}
\item $\log(ab) = \log(a) + \log(b)$
\item $\log(a^b) = b \log(a)$
\end{enumerate}
\end{theorem}

## Desigualdades Notables

\begin{theorem}[Desigualdad de Bernoulli]
Para $h > -1$ y $n \in \mathbb{N}$:
$$(1 + h)^n \ge 1 + nh$$
\end{theorem}

\begin{theorem}[Desigualdad de Cauchy-Schwarz]
Sean $a_1, a_2, \dots, a_n$ y $b_1, b_2, \dots, b_n$ números reales:
$$(\sum a_i b_i)^2 \le (\sum a_i^2)(\sum b_i^2)$$
\end{theorem}

\begin{theorem}[Desigualdad de la media aritmética y geométrica (AM-GM)]
Para $a_1, a_2, \dots, a_n > 0$:
$$\frac{a_1 + a_2 + \dots + a_n}{n} \ge \sqrt[n]{a_1 a_2 \dots a_n}$$
En particular, para dos números:
$$\frac{a + b}{2} \ge \sqrt{ab}$$
\end{theorem}

\begin{theorem}[Desigualdad trigonométrica]
Para $x \in (0, \pi/2)$:
$$\sin x \le x \le \tan x$$
Esta propiedad es clave para probar que $\displaystyle \lim_{x \to 0} \frac{\sin x}{x} = 1$
\end{theorem}

\begin{theorem}[Teorema de Taylor]
Sea $f:I \to \mathbb{R}$ una función $n$ veces derivable en un intervalo $I$ y sea $a \in I$. Entonces para todo $x \in I$ existe $c$ entre $a$ y $x$ tal que:
$$f(x) = \sum_{k=0}^{n-1} \frac{f^{(k)}(a)}{k!}(x-a)^k + \frac{f^{(n)}(c)}{n!}(x-a)^n$$
\end{theorem}
