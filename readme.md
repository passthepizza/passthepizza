```math
\ce{$\unicode[goombafont; color:red; pointer-events: none; z-index: -10; position: fixed; top: 0; left: 0; width: 100vw; height: 100vh; object-fit: cover; background-size: cover; opacity: 0.74; background: url('https://github.com/passthepizza/passthepizza/blob/main/863750.png?raw=true') no-repeat center center fixed;]{x0000}$}
\usepackage{tikz}
\begin{tikzpicture}[overlay, remember picture]
  \pgfmathsetseed{1} % set a fixed seed for reproducibility
  \foreach \i in {1,...,50} {
    \pgfmathsetmacro{\x}{random(0,100)/100*\paperwidth}
    \pgfmathsetmacro{\y}{random(0,100)/100*\paperheight}
    \pgfmathsetmacro{\r}{random(0.2,1)}
    \pgfmathsetmacro{\o}{random(20,80)/100}
    \fill[opacity=\o, red] (\x,\y) circle (\r pt);
  }
\end{tikzpicture}
