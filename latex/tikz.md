# Tikz

```text
\usepackage{tikz}
```

## Data from csv file

#### Package Requirement

```text
\usepackage{pgfplots}
```

I usually save my data from python using Pandas. The data are then saved into the csv format. When I plot my figure in my publication, I use `pgfplot` to construct the plot from the csv file. This allows me to complety separate data from their presentation. In this context, I can easily change the apparence of my plots in my Latex document. 

```text
\begin{figure}[!t]
\centering
\begin{tikzpicture}
    \begin{axis}[xlabel near ticks,ylabel near ticks,grid=both,legend pos=south west]
        \addplot+[thick,blue] table[x index=0, y index=1, col sep=comma] {file.csv}; 
        \addplot+[thick,red] table[x index=0, y index=1, col sep=comma] {file.csv}; 
    \legend{plot1,plot2}
    \end{axis}
\end{tikzpicture}
\caption{My caption}\label{fig:myfigure}
\end{figure}
```

## Electronic Circuits

#### Package Requirement

```text
\usepackage{tikz}
\usepackage{circuitikz}
```

### Sallen Key : Low Pass

![](../.gitbook/assets/sk_lp.svg)

```text
\begin{tikzpicture}
	\node[op amp, yscale=1] (opamp) at (6,-0.5) {};
	\draw ($(opamp.+)+(-4.5,0)$) node[left] {$V_{in}$} 
	to[R, l=$R_1$, o-*] ($(opamp.+)+(-2.5,0)$) node (nodebetween1) {}
	to[R, l=$R_2$, *-*] ($(opamp.+)+(-0.5,0)$) node (nodebetween2) {}
	to[short] (opamp.+);
	\draw (nodebetween2.center) to[C, l=$C_2$, *-] ($(nodebetween2)+(0,-1.5)$) node [ground] {};
	\draw (nodebetween1.center) to[short] ($(nodebetween1)+(0,-3)$) 
	to[C, l=$C_1$] ($(opamp.out)+(0,-3.5)$) 
	to[short] (opamp.out);
	\draw (opamp.-) to[short] ($(opamp.-)+(0,1)$) node (nodebetween3) {}
	to[R, l=$R_4$, *-]  ($(opamp.out)+(0,1.5)$) 
	to[short] ($(opamp.out)+(0,1.5)$) 
	to[short] (opamp.out);
	\draw (nodebetween3.center) to[R, l=$R_3$, *-] ($(nodebetween3)+(0,1.5)$) node [ground, yscale=-1] {};
	\draw (opamp.out) to[short, *-o]  ($(opamp.out)+(0.5,0)$) node[right] {$V_{out}$};
\end{tikzpicture}
```

### MFB : Low Pass

![](../.gitbook/assets/mfb_lp.svg)

```text
\begin{tikzpicture}
	\node[op amp, yscale=1] (opamp) at (6,-0.5) {};
	\draw ($(opamp.-)+(-5.5,0)$) node[left] {$V_{in}$} 
	to[R, l=$R_1$, o-*] ($(opamp.-)+(-2.5,0)$) node (nodebetween1) {}
	to[R, l=$R_3$, *-*] ($(opamp.-)+(-0.5,0)$) node (nodebetween2) {}
	to[short] (opamp.-);
	\draw (nodebetween1.center) to[C, l_=$C_1$, *-] ($(nodebetween1)+(0,-2)$) node [ground] {};
	\draw (nodebetween1.center) to[R, l=$R_2$, *-] ($(nodebetween1)+(0,3)$) 
	to ($(nodebetween1)+(2,3)$) node (nodebetween4) {}
	to ($(opamp.out)+(0,3.5)$) 
	to[short] (opamp.out);
	\draw (nodebetween4.center) to[C, l=$C_2$, *-] ($(nodebetween4.center)+(0,-3)$);
	\draw ($(opamp.+)$) to ($(opamp.+)+(-1,0)$) to ($(opamp.+)+(-1,-1)$) node [ground] {};
	\draw (opamp.out) to[short, *-o]  ($(opamp.out)+(0.5,0)$) node[right] {$V_{out}$};
\end{tikzpicture}
```

### Common Circuits : 

A list of common analog circuits are available here: [https://github.com/vincentchoqueuse/analog\_circuits\_tikz](https://github.com/vincentchoqueuse/analog_circuits_tikz)

