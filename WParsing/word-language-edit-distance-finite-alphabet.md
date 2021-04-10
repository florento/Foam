# Word language edit distance 
finite alphabet

for $L_1, L_2 \subseteq \Sigma^*$, 
$$ d(L_1, L_2) = \bigoplus_{w_1 \in L_1, w_2 \in L_2} d(w_1, w_2) $$ 

rem: we need to define infinite sums with $\oplus$.

Results:
- $d(L_1, L_2)$ computable in TIME $O(| A_1| . | A_2 |)$ (resp. sizes of automata) for $L_1, L_2$ regular

> Mohri, Mehryar, Fernando Pereira, and Michael Riley
> The design principles of a weighted finite-state transducer library
> Theoretical Computer Science 231.1 (2000): 17-32
https://www.sciencedirect.com/science/article/pii/S0304397599000146

> Allauzen, Cyril, Michael Riley, Johan Schalkwyk, Wojciech Skut, and Mehryar Mohri
> OpenFst: A general and efficient weighted finite-state transducer library
> In International Conference on Implementation and Application of Automata, pp. 11-23, 2007.
https://doi.org/10.1007/978-3-540-76336-9_3


- $d(L_1, L_2)$ not computable for $L_1, L_2$ CF

reduction of non-emptiness of the intersection of 2 CF languages.

- $d(L_1, L_2)$ computable for $L_1$ regular and $L_2$ CF
  - PTIME algorithm based on unary homomorphisms
  - optimal alignment in worst case exponential in size of grammar automaton

> Han, Yo-Sub, Sang-Ki Ko, and Kai Salomaa
> The edit-distance between a regular language and a context-free language
> International Journal of Foundations of Computer Science 24.07 (2013): 1067-1082.
https://doi.org/10.1142/S0129054113400315

- $d(L_1, L_2)$ computable for $L_1, L_2$ VPA ?
  (ref. ?) 
