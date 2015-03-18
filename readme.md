# A simple completion engine

Providing completion for text input is a typical use case for
[tries](https://en.wikipedia.org/wiki/Trie). The implementation is extremely
simple. For a given partial word, descend on the tree and return all words in
the subtree found at the last node of the partial word. Since
[directed acyclic word graphs (DAWG)](https://en.wikipedia.org/wiki/Deterministic_acyclic_finite_state_automaton).
are more space efficient, but otherwise similar to tries, this implementation is
based on a DAWG again.
