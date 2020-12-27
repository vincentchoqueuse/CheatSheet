# Tikz

```text
\usepackage{tikz}
```

## Data from csv file

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



