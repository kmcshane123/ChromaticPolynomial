# ChromaticPolynomial
This C++ program calculates the chromatic polynomial of a graph. It is limited to graphs with at most 64 nodes. The problem is NP hard, so ... The method is essentially the deletion/contraction algorithm. It checks for special cases: graphs with bridges, chordal graphs, complete graphs, and loops. The memoization may overflow if these checks are not fruitful. The code currently computes the solution modulo 998244353.

Input format: N M v0 w0 v1 n v2 w2 etc. where N is the number of vertices (or nodes), M is the number of edges. The nodes are numbered 0 through N-1, and edge i connects vertices vi and wi.

SAMPLE INPUT: 5 7 0 1 0 2 0 4 1 3 2 3 2 4 3 4

OUTPUT 0 10 998244330 19 998244346 1

Uses a modular integer class to handle the mod calculations and a power series class to deal with polynomials.

This code is verified, in that it solves https://judge.yosupo.jp/problem/chromatic_polynomial
