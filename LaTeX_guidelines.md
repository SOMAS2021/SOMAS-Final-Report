# LaTeX Guidelines for the Final Report
Version on Dec 14, 2021.

This document is based on the guidelines proposed for the SOMAS2020 report.

Try to stick to these guidelines, and feel free to suggest other if needed. Following consistent rules will facilitate the reviewing and ensure homogeneity of the report.

1. In the report, we need to label *everything* that we refer to: figures, equations, sections, subsections, subsubsections etc. Here are some important examples:

For figures:
```tex
\label{fig:XX}
```
For equations:
```tex
\label{eq:XX}
```
For sections:
```tex
\label{sec:XX}
```
For subsections:
```tex
\label{subsec:XX}
```

To refer to these labels, just use
```tex
 \Cref{your_label}
```
`\Cref{}` automatically refers to your `your_label` by adding the corresponding label type with a capital letter, *e.g.,* Section, Figure, Table, etc. *No need to manually add "Figure" or something like that in front.*

2. Always refer to an existing figure or table at least once in the text.

3. Select the figure and table placement `[htb]` as often as possible. Avoid forcing the placement with `[H]` or `[h!]` .

4. Write *proper* captions for your images. *Finish your caption with a punctuation*.

Example:
```tex
\begin{figure}[htb]\label{sim_res_case_1}
...
\caption{Simulation results for Case 1.}
\end{figure}
```

5. Footnotes appear *before* the punctuation.

Example:
```tex
... at each turn\footnote{It is assumed that...}.
```

6. `\texttt{}` style is only for referring to something related to code.

Example:
```tex
... \texttt{a.TakeFood(foodAmount)} allows the agent to ask for food.
```

7. When referring to mathematical expression directly in the text (*e.g.,* variables, simple equations), write them in the math mode using `$ $`.

Example:
```tex
... the agent $a_1$ has taken $x$ amount of food ...
```
8.  If you want to write mathematical expressions not directly in the text, use `\begin{equation}\label{my_equation}... \end{equation}`. Avoid using `$$ ... $$`, as the equation will not be numbered.

9. Finish the itemizations/enumerations with a punctuation.

Example:
```tex
\begin{itemize}
\item The base parameters of an agent are:
    \begin{enumerate}
    \item HP
    \item Floor level.
    \end{enumerate}
\end{itemize}
```

10. Write "*i.e.,* and  *e.g.,*, in italic and followed by a comma.

11. Use comma appropriately. A common mistake is to *forget* using comma before "FANBOYS" which are:
- for
- and
- nor
- but
- or
- yet
- so.