# Word Language Edit Distance Infinite Alphabet


languages defined by Symbolic Automata Framework

Questions:

- $d(L_1, L_2)$ computable for $L_1, L_2$ Symbolic Automata (SA) languages?
  (ref.?)
    

- and for Symbolic Visibly Pushdown Automata ?
  
> Loris D’Antoni and Rajeev Alur 
> Symbolic visibly pushdown automata
> International Conference on Computer Aided Verification. Springer, 2014.  
https://doi.org/10.1007/978-3-319-08867-9_14

definition of $L(A_1, A_2)$ must take care of relationship between the label theory (Boolean closed) for SA and the cost function for E.D. / DTW ?


**ex.** 
- $A_1$ is an automaton for prior score language. 
  The value in $S$ returned by is a measure of notational complexity of a score.
  Note that for markups, the language is not regular ($A_1$ is a VPA then).
- $A_2$ is a singleton automaton for a performance given $w_2$.
- the distance is then $\bigoplus_{w_1 \in \Omega^*} A_1(w_1) \otimes d(w_1, w_2)$, i.e. the combination of 2 criteria to optimise. 
  The best $w_1$ is a music score infered for $w_2$ (transcription of $w_2$).

