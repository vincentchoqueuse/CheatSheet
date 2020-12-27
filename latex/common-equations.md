# Common Equations

This Page contains several Latex code commonly used in my Latex documents. These codes are directly to my teaching courses \(signal processing, control engineering, ...\)

## Mathematics

### Euler Decomposition

* Cosine Decomposition :

$$
\cos(\theta)=\frac{1}{2}\left(e^{j\theta}+e^{-j\theta}\right)
$$

```text
\cos(\theta)=\frac{1}{2}\left(e^{j\theta}+e^{-j\theta}\right)
```

* Sine Decomposition :

$$
\sin(\theta)=\frac{1}{2j}\left(e^{j\theta}-e^{-j\theta}\right)
$$

```text
\sin(\theta)=\frac{1}{2j}\left(e^{j\theta}-e^{-j\theta}\right)
```

## Signal Processing

### Continuous Signals

* Dirac Impulse :

$$
\delta(t)=\left\{\begin{array}{cl}1 &\text{ if }t=0,\\0&\text{elsewhere}.\end{array}\right.
$$

```text
\delta(t)=\left{\begin{array}{cl}
1 &\text{ if }t=0,\\
0&\text{elsewhere}.
\end{array}\right.
```

* Step Impulse :

$$
u(t)=\left\{\begin{array}{cl}1 &\text{ if }t\ge 0,\\0&\text{elsewhere}.\end{array}\right.
$$

```text
u(t)=\left\{\begin{array}{cl}
1 &\text{ if }t\ge 0,\\
0&\text{elsewhere}.\end{array}
\right.
```

* Sine wave

$$
x(t)=a\cos(\omega_0 t+\varphi)
$$

```text
x(t)=a\cos(\omega_0 t+\varphi)
```

* Dirac Comb 

$$
\delta_{T_0}(t)=\sum_{n=-\infty}^{\infty}\delta(t-nT_0)
$$

```text
\delta_{T_0}(t)=\sum_{n=-\infty}^{\infty}\delta(t-nT_0)
```

* Periodic Signal Fourier Décomposition

$$
x(t)=\sum_{n=-\infty}^{\infty}c_n e^{2j\pi nf_0 t}dt
$$

```text
x(t)=\sum_{n=-\infty}^{\infty}c_n e^{2j\pi nf_0 t}dt
```

### Common Transforms

* Laplace Transform :

$$
X(s)=\int_{0}^{\infty}x(t)e^{-st}ds
$$

```text
X(s)=\int_{0}^{\infty}x(t)e^{-st}ds
```

* Fourier Tranform :

$$
X(f)=\int_{-\infty}^{\infty}x(t)e^{-2j\pi ft}dt
$$

```text
X(f)=\int_{-\infty}^{\infty}x(t)e^{-2j\pi ft}dt
```

* Z transform :

$$
H(z)=\sum_{n=0}^{\infty} x[n]z^{-n}
$$

```text
H(z)=\sum_{n=0}^{\infty} x[n]z^{-n}
```

### Transfer Functions

* Rational Function

$$
H(s)=\frac{b_ns^n+\cdots+b_1s+b_0}{a_ns^n+\cdots+a_1s+a_0}
$$

```text
H(s)=\frac{b_ns^n+\cdots+b_1s+b_0}{a_ns^n+\cdots+a_1s+a_0}
```

* First order Transfer function

$$
H(s)=\frac{K}{\tau s+1}
$$

```text
H(s)=\frac{K}{\tau s+1}
```

* Second order Transfer function

$$
H(s)=\frac{K}{\frac{1}{\omega_n^2}s^2+\frac{2m}{\omega_n}s+1}
$$

### Closed Loop

$$
H(s)=\frac{C(s)F(s)}{1+C(s)F(s)}
$$

```text
H(s)=\frac{C(s)F(s)}{1+C(s)F(s)}
```

