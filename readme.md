```math
\documentclass{article}
\usepackage{xcolor}
\usepackage{amsmath}
\usepackage{hyperref}

\begin{document}

\begin{center}
  \Huge
  \color{red} % Change text color
  \shadowbox{ % Add shadow effect
    \gradtext{ % Apply gradient
      \[
      \ce{E = mc^2}
      \]
    }
  }
\end{center}

<style>
body {
  background: url('https://github.com/passthepizza/passthepizza/blob/main/863750.png?raw=true') no-repeat center center fixed;
  background-size: cover;
  opacity: 0.74;
  animation: background-animation 10s infinite alternate;
}

@keyframes background-animation {
  0% { opacity: 0.7; }
  50% { opacity: 0.9; }
  100% { opacity: 0.7; }
}

.gradtext {
  background: -webkit-linear-gradient(45deg, #ff6b6b, #f94d6f);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.shadowbox {
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}
</style>

\end{document}
