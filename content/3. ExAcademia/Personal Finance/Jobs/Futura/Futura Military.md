---
draft: false
---
On this page, I provide both the lesson materials I have produced and briefly present my work with [[Futura]] regarding public competition preparation. Since September 2024, I have been a teacher of mathematics, logic, and physics, delivering a 90-minute lesson each week. The page dedicated to students is [[ADT Forze Armate]].
### Materials List
In this section, I divide the [relevant topics](https://docs.google.com/spreadsheets/d/1eMpxxHZ-sKFeJQUStWW4EmgYVRKeH61FAxySaHhZHes/read) for different competitions and include the slides I have prepared for each of these lessons.
##### Mathematics
- [Overleaf: Trigonometry](https://www.overleaf.com/read/nwgnjmprzjpj#e27ac6)
- 
##### Logic
##### Physics

#### $\LaTeX$ Code
I suggest to compile this code using [Overleaf](https://www.overleaf.com/), the following passages are crucial for the proper compilation of the code:
1. Download these images, and upload them (left column)
	- [[slide1.jpeg]]
	- [[slide2.jpeg]]
	- [[lastslide.jpeg]]
2. Set LuaTeX instead of LaTeXpdf compiler from the menu.

```LaTeX
% Compilare con XeLaTeX o LuaLaTeX

\documentclass{beamer}
\usepackage[absolute,overlay]{textpos}
% Pacchetti necessari per il font Open Sans e la gestione dei colori
\usepackage{fontspec}   % Funziona con XeLaTeX o LuaLaTeX
\usepackage{xcolor}     % Per definire colori personalizzati
\usepackage{graphicx}   % Per includere immagini
\usepackage{enumitem}   % Per personalizzare gli elementi delle liste
\usepackage{adjustbox}  % Per adattare dimensioni di immagini e altri elementi
\usepackage{amsmath}    % Per le equazioni matematiche
\usepackage{pgfplots}   % Per i grafici

% Impostare il font Open Sans (è necessario avere Open Sans installato sul sistema)
\setsansfont{Open Sans}

% Definire i colori personalizzati ADT
\definecolor{ADTBlue}{RGB}{26, 46, 73}   % Colore blu (#1A2E49)
\definecolor{ADTRed}{RGB}{235, 77, 61}   % Colore rosso (#EB4D3D)

% Impostare il tema Beamer su default e modificare le impostazioni di colore
\setbeamercolor{normal text}{fg=ADTBlue}
\setbeamercolor{frametitle}{fg=ADTBlue}

% Definire i colori per i simboli delle liste
\setbeamercolor{item}{fg=ADTBlue}

% Definire il simbolo del trattino usando ADTRed
\newcommand{\reddash}{{\color{ADTRed}\textbf{\textemdash}}}

% Comando per i titoli delle diapositive: trattino + titolo in grassetto
\newcommand{\titledash}[1]{\frametitle{\reddash\ \textbf{#1}}}

% Personalizzare i simboli delle liste: usare pallini invece di triangoli
\setlist[itemize,1]{label=\textbullet, labelsep=1em, left=1em, itemsep=0.5em, font=\color{ADTBlue}}

\begin{document}

\begin{frame}[plain]
    \begin{textblock}{10}(-1,1) % Regola (x,y) come necessario
        \includegraphics[width=14cm,keepaspectratio]{slide1.jpeg}
    \end{textblock}
\end{frame}

\begin{frame}[plain]
    \begin{textblock}{10}(-1,1) % Regola (x,y) come necessario
        \includegraphics[width=14cm,keepaspectratio]{slide2.jpeg}
    \end{textblock}
\end{frame}


% Ultima Diapositiva: Immagine a tutto schermo
\begin{frame}[plain]
    \begin{textblock}{10}(-1,1) % Regola (x,y) come necessario
        \includegraphics[width=14cm,keepaspectratio]{lastslide.jpeg}
    \end{textblock}
\end{frame}

\end{document}
```