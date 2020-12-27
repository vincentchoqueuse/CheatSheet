# Introduction

## Why Latex

![](../.gitbook/assets/latex.png)

Latex is a software system for document preparation. It can be used to create long document \(such as PhD Thesis, report, and article\) and provides tools for the management of tables of contents, table of figure, bibliography, and more. Latex also provide a wonderful syntax for equation writing.

### How to Install Latex

* [Install Latex](https://www.latex-project.org/get/)

### How to Use Latex

* [The not so short introduction to Latex](https://tex.loria.fr/general/lshort2e.pdf). The not so short introduction is a good ressource to start with. Section 3.9 contains the list of available mathematical symbols.

## Code Snippets

### Create a document

```text
\documentclass{article}

\begin{document}
First document.
\end{document}
```

For french documents, I need to import specifc packages to deal with particular characters.

```text
\documentclass[french]{article}
\usepackage{lmodern}
\usepackage[T1]{fontenc}
\usepackage{babel}

\begin{document}
First document.
\end{document}
```

### Figures

* Packages to include : 

```text
\usepackage{caption}
\usepackage{subcaption}
```

* Side by Side figures

```text
\begin{subfigure}{.5\textwidth}
  \centering
  \includegraphics[width=.4\linewidth]{image1}
  \caption{A subfigure}
  \label{fig:sub1}
\end{subfigure}%
\begin{subfigure}{.5\textwidth}
  \centering
  \includegraphics[width=.4\linewidth]{image1}
  \caption{A subfigure}
  \label{fig:sub2}
\end{subfigure}
\caption{A figure with two subfigures}
\label{fig:test}
\end{figure}
```

### Tables

```text
\begin{table}{cccc}
\hline
 & & & \\
\hline
 & & & \\
 & & & \\
\hline
\end{table}
```

