# Quantum-differences

This Mathematica notebook is an efficient (O[N]) implementation of an algorithm finding  differences of two lists of equal lengths along with the corresponding parity sign
Notes:
- Each lists must contain no repetitions within itself
- a & b are the input lists, while c & d are the output lists. In set notation c = a -b; d = b - a;
- Their elements can themselves be lists.
- Parity sign is defined as the parity (+ even, - odd) of the total number  of permutations in both lists needed to reduce them to their intersection with the operation of removing the shared elements on the same position

# Motivation

If a and b represent multi-particle wavefunctions in secondary quantized representations, then the matrix element can be calculated as:
< a | b > = sign < c | d >
Similarly for an oparator O, we get:
< a | O | b > = sign < c | O | d >
assuming the intersection of a and b is equal to the number of particles acted on by O (since < a | O | b > = 0 if it is larger)
