\section*{RR\_MPCC\_output --- Repository Guide}

This repository contains numerical results for MPCC/CC2 scans across multiple basis sets and molecules.  
The directory structure is organized to ensure clarity, consistency, and ease of navigation.

\subsection*{Repository Structure}

At the top level, the repository contains four basis-set directories:

\begin{verbatim}
cc-pvdz/
cc-pvtz/
aug-cc-pvdz/
aug-cc-pvtz/
\end{verbatim}

Each basis directory contains folders corresponding to the molecules studied, for example:

\begin{verbatim}
cc-pvdz/
    TIP4P-6/
    C6H14/
    ...
\end{verbatim}

\subsection*{Contents of Each Molecule Folder}

Within each molecule directory, results are organized by \textbf{scan type}.  
The four scan types included are:

\begin{itemize}
    \item \texttt{Lov}
    \item \texttt{Lvv}
    \item \texttt{Lov\_Lvv\_fix\_Loo\_1}
    \item \texttt{Lvv\_fix\_Loo\_1}
\end{itemize}

For each scan, the following folders are present:

\subsubsection*{\texttt{energies\_folder\_\{scan\}}}
\begin{itemize}
    \item CC2 energy convergence plots
    \item Iteration-wise energy behavior
\end{itemize}

\subsubsection*{\texttt{Y\_amp\_\{scan\}}}
\begin{itemize}
    \item \( L_2 \) error of Y amplitudes
    \item Histogram of Y amplitude distribution
\end{itemize}

\subsubsection*{\texttt{Omega\_\{scan\}}}
\begin{itemize}
    \item \( L_2 \) error of \( \Omega \)
    \item Histogram of \( \Omega \)
\end{itemize}

\subsubsection*{\texttt{Foo\_\{scan\}}}
\begin{itemize}
    \item \( L_2 \) error of \( F_{oo} \)
    \item Histogram of \( F_{oo} \)
\end{itemize}

\subsubsection*{\texttt{Fov\_\{scan\}}}
\begin{itemize}
    \item \( L_2 \) error of \( F_{ov} \)
    \item Histogram of \( F_{ov} \)
\end{itemize}

\subsubsection*{\texttt{Fvv\_\{scan\}}}
\begin{itemize}
    \item \( L_2 \) error of \( F_{vv} \)
    \item Histogram of \( F_{vv} \)
\end{itemize}

\subsection*{Combined 2$\times$2 Plots}

For convenience, combined plots (CC2 convergence, \(L_2\) error of Y, and \(L_2\) error of \(\Omega\))  
are stored in the directory:

\begin{verbatim}
RR_MPCC_output/
\end{verbatim}

These summary plots are intended for quick comparison, while individual plots are used in the paper.

\subsection*{Notes}

\begin{itemize}
    \item All results currently use tolerance \( \text{tol} = 10^{-4} \), unless stated otherwise.
    \item The folder structure is standardized across all basis sets and molecules.
\end{itemize}

