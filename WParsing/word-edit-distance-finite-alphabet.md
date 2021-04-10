# Word edit distance 
$\Sigma$ is a finite alphabet

we consider extension to infinite alphabet in [[word-edit-distance-infinite-alphabet]].


distance $d$:
- defined over $\Sigma^*$ 
- into a semiring  $S = ( K, \oplus, \otimes, 0, 1)$

**Levenstein E.D.** 
based on a cost function $\delta$:
$$\delta: (\Sigma \cup \{ \epsilon \}) \times (\Sigma \cup \{ \epsilon \}) 
          \setminus \{ (\epsilon, \epsilon) \} \to S$$

Complexity for $d(w_1, w_2)$ computation:
  - classical : $O(|w_1| . |w_2|)$ [Wagner, Fisher 1974]
    assuming $\Sigma$ fixed and finite.
  - improved $O(|w_1| + |w_2| + d^2)$ [Ukonnen 1985]
  - subquadratic 

