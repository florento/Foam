# Word Edit Distance Infinite Alphabet

$\Omega$ is an infinite alphabet

[[word-language-edit-distance-infinite-alphabet]]

## Alphabet
infinite set of symbols $\Omega$

**ex.**  [alphabet]
timestamped events (onsets, offsets), 
The date of $a \in \Omega$ is denoted $t_a$.
$\Omega$ finite but huge for sampled dates (or IOI values), or infinite (rational values).

**ex.** [sequences]
- a music performance is a sequence of timestamped events ~ unquantified MIDI
- a score (music sheet) is also a sequence of timestamped events (with quantified timestamped)
  - quantified ("score") MIDI
  - structured with additional markups (parentheses): XML (MEI etc)

## Distance between words

**DTW** (for temporal sequences)
  based on $\delta(a, b) = |t_a - t_b|$ for $a, b \in \Omega$

complexity DTW: 
  - TIME $O(|w_1| . |w_2|)$
  - subquadratic TIME and SPACE $O(\frac{|w_1|^2}{\log \log|w_1|})$, with $|w_1| \geq |w_2|$ [Gold and Sharir 2018 JACM]
    https://doi.org/10.1145/3230734
  -  SPACE $O(|w_1| + |w_2|)$ [Tralie and Dempsey 2020 ISMIR]
     https://arxiv.org/abs/2008.02734


**ex.** distance between a performance and a score, using the above representations.
with the possibility of missing notes (?)
If the score contains markups, it is possible to ignore them in the computation, with appropriate deletion primitive values.

**ex.** semiring containing as components:
- cumulated time-shifts
- a tempo curve
