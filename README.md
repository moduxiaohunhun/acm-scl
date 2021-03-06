# ACM - SCL

*This is the Standard Code Library (SCL) for Competitive Programming.*

Many commonly seen/used algorithms and data structures in competitive programming have been implemented. You can find the implementations in [`code`](/code).

A tool used to compare the output files has also been implemented, the source code of which can be found in [`_cmp`](/_cmp).

Word/PDF documents containing well-organized source code and some useful theorems and formulas can be found in [`_SCL`](/_SCL). Most of the theorems and formulas are from *Wikipedia* and *Concrete Mathematics*.

Some notes can be found in [`notes`](/notes). They are `Markdown` files with `LaTeX` formulas. I use `VSCode` + `Markdown All in One` + `Markdown Preview Enhanced` to read and edit these notes.

### Notes:
- My C++ compiler is [MinGW-W64](https://sourceforge.net/projects/mingw-w64/) 8.1.0. Compile the code with `c++0y` (a.k.a. C++ 14) compiling option.
- My Java compiler's version is 11.0.1.
- Surely, I am **NOT** the inventor of these amazing algorithms and data structures! I learned them (or the code) from the Internet or some textbooks!

### Tips:
- The code works. I have tested it in several contests. All the algorithms and data structures implemented here have been thoroughly checked. You are sure to get `AC` if they are correctly used.
- Many `vector`s can be replaced with arrays! So as to many other C++ STL classes in the code. If you are getting `TLE` or `MLE`, replace them with arrays or other self-implemented data structures. The SCL should be clear and easy to understand so I used C++ STL classes.
- There are few comments in the code. It would be appreciated if you add any! ^_^

## Table of Contents
- Data Structures [`code/`](/code)
    - Hash Table [`hash_table.h`](/code/hash_table.h)
        - Basic Hash Table [`dictionary`](/code/hash_table.h)
        - Skip List [`skip_list`](/code/hash_table.h)
    - Binary Search Tree (BST)
        - Basic BST [`search_tree.h:search_tree`](/code/search_tree.h)
        - AVL [`search_tree.h:avl_tree`](/code/search_tree.h) [`tree.h:avl_tree`](/code/tree.h)
        - Red-Black Tree [`search_tree.h:rb_tree`](/code/search_tree.h)
        - Treap [`search_tree.h:treap`](/code/search_tree.h) [`tree.h:treap`](/code/tree.h) [`tree.h:TREAP::treap`](/code/tree.h)
        - Splay [`search_tree.h:splay_tree`](/code/search_tree.h)
        - Modified Splay (Range Query) [`tree.h:splay_tree`](/code/tree.h)
    - Heap [`heap.h`](/code/heap.h)
        - Binary Heap [`binary_heap`](/code/heap.h)
        - Leftist Heap [`leftist_heap`](/code/heap.h)
        - Pairing Heap [`pairing_heap`](/code/heap.h)
    - Binary Indexed Tree [`tree.h:binary_indexed_tree`](/code/tree.h) [`tree.h:binary_indexed_tree_2`](/code/tree.h)
    - Segment Tree [`tree.h`](/code/tree.h)
        - Basic Segment Tree [`segment_tree`](/code/tree.h) [`segment_tree_2`](/code/tree.h)
        - Persistent Segment Tree [`persistent_segment_tree`](/code/tree.h) [`persistent_segment_tree_2`](/code/tree.h)
    - Automaton [`tree.h`](/code/tree.h)
        - Trie & Aho-Corasick Algorithm [`trie`](/code/tree.h) [`trie_2`](/code/tree.h) [`trie_01`](/code/tree.h)
        - Palindrome Automaton [`palindrome_automaton`](/code/tree.h)
        - Suffix Automaton [`suffix_automaton`](/code/tree.h)
        - Extended Suffix Automaton [`ext_suffix_automaton::suffix_automaton`](/code/tree.h) ([`ext_suffix_automaton::merge`](/code/tree.h) *is used to merge nodes in segment tree*)
    - Disjoint Set [`misc.h:disj_sets`](/code/misc.h)
    - Sparse Table [`misc.h:init_st`](/code/misc.h) `&` [`misc.h:query_min`](/code/misc.h)
    - Techniques in Tree [`tree.h`](/code/tree.h)
        - Heavy-Light Decomposition [`heavy_light_decomposition`](/code/tree.h)
        - Centroid Decomposition [`centroid_decomposition_of_tree`](/code/tree.h)
        - DSU [`dsu_on_tree`](/code/tree.h)
        - Auxiliary Tree [`auxiliary_tree`](/code/tree.h)
    - Dancing Links [`misc.h:DLX`](/code/misc.h)
- Sorting [`code/sort.h`](/code/sort.h)
    - Quick Sort [`quick_sort(vector<T> &)`](/code/sort.h)
    - Quick Select [`quick_select(vector<T> &, int k)`](/code/sort.h)
    - Merge Sort [`merge_sort` `merge_sort_2(vector<T> &)`](/code/sort.h)
    - Introspective Sort [`introspective_sort`](/code/sort.h)
    - Radix Sort [`radix_sort_1`](/code/sort.h) [`radix_sort_2`](/code/sort.h) [`counting_radix_sort`](/code/sort.h)
- String [`code/misc.h`](/code/misc.h)
    - Hash [`BKDR_hash(const char *)`](/code/misc.h) [`init_hash(const char *)`](/code/misc.h) `&` [`BKDR_hash(int, int)`](/code/misc.h)
    - KMP [`KMP_match`](/code/misc.h)
    - Extended KMP [`ext_KMP`](/code/misc.h)
    - Manacher [`manacher`](/code/misc.h)
    - Suffix Array & LCP Array
        - $O(n\log^2 n)$ Algorithm [`construct_sa`](/code/misc.h) `&` [`construct_lcp`](/code/misc.h)
        - $O(n\log n)$ Algorithm [`construct_sa_lcp`](/code/misc.h) [`da`](/code/misc.h) `&` [`calc_height`](/code/misc.h)
        - $O(n)$ Algorithm [`create_suffix_array`](/code/misc.h) [`SA_IS::suffix_array`](/code/misc.h) [`dc3`](/code/misc.h) `&` [`calc_height`](/code/misc.h)
- Computational Geometry (2D) [`code/computational_geometry.h`](/code/computational_geometry.h)
    - Points [`point`](/code/computational_geometry.h)
    - Vectors [`vec`](/code/computational_geometry.h)
    - Dot, Cross Product
    - Line, Segment Intersection
    - Distances
    - Areas [`area`](/code/computational_geometry.h)
    - Center of Mass [`gravity`](/code/computational_geometry.h)
    - Convex Hulls
        - Graham Scan [`graham`](/code/computational_geometry.h)
        - Andrew [`convex_hull`](/code/computational_geometry.h)
    - Rotating Calipers [`rotating_calipers`](/code/computational_geometry.h)
    - Fermat Point (Simulated Annealing) [`fermat_point`](/code/computational_geometry.h)
    - Closest Pair of Points [`find_closest_pair`](/code/computational_geometry.h)
    - Half Plane Intersection [`half_plane_intersection`](/code/computational_geometry.h) [`cut`](/code/computational_geometry.h)
- Graph Theory [`code/graph.h`](/code/graph.h)
    - Shortest Path
        - Bellman-Ford [`bellman_ford`](/code/graph.h)
        - Dijsktra [`dijkstra`](/code/graph.h)
        - Floyd Warshall [`floyd_warshall`](/code/graph.h)
    - Spanning Tree
        - Prim [`prim`](/code/graph.h)
        - Kruskal [`kruskal`](/code/graph.h)
    - Max Flow
        - Edmonds-Karp [`edmonds_karp`](/code/graph.h)
        - Dinic [`dinic`](/code/graph.h)
        - ISAP [`isap`](/code/graph.h)
    - Min Cost Max Flow
        - Stardard SPFA Version [`min_cost_max_flow`](/code/graph.h)
        - Dijsktra Optimized [`graph_ext::min_cost_max_flow`](/code/graph.h)
    - Bipartite Matching
        - Hungarian [`hungary`](/code/graph.h)
        - KM (BFS, DFS) [`KM_BFS::km`](/code/graph.h) [`KM_DFS::km`](/code/graph.h)
    - Strongly Connected Components
        - Tarjan [`tarjan(int)`](/code/graph.h)
        - Kosaraju [`scc`](/code/graph.h)
    - Cut Vertices & Bridges
        - Tarjan [`tarjan(int, int)`](/code/graph.h)
    - Lowest Common Ancestor
        - Binary Search [`lca_dfs`](/code/graph.h) `&` [`lca`](/code/graph.h)
        - RMQ [`graph_ext::init_rmq_lca`](/code/graph.h) `&` [`graph_ext::rmq_lca`](/code/graph.h)
        - Tarjan [`lca_tarjan`](/code/graph.h)
    - Topological Sort [`topological_sort`](/code/graph.h)
- Math [`code/`](/code)
    - Number Theory [`number_theory.h`](/code/number_theory.h)
        - Greatest Common Divisor (GCD) [`gcd`](/code/number_theory.h)
        - Extended GCD [`ext_gcd`](/code/number_theory.h)
        - Multiplicative Inverse [`inv`](/code/number_theory.h)
        - Chinese Remainder Theorem (CRT) [`CRT`](/code/number_theory.h)
        - Modular Linear Equations [`modular_linear_equations`](/code/number_theory.h)
        - Prime [`is_prime`](/code/number_theory.h) [`prime_factors`](/code/number_theory.h)
        - Euler's Totient Function [`euler`](/code/number_theory.h)
        - Sieve
            - Sieve of Eratosthenes [`sieve_of_eratosthenes` ](/code/number_theory.h)
            - Euler's Sieve [`eulers_sieve`](/code/number_theory.h)
        - Quick Power [`mod_pow`](/code/number_theory.h)
        - Lucas [`lucas`](/code/number_theory.h)
        - Extended Lucas [`ext_lucas`](/code/number_theory.h)
        - Baby Step Giant Step (BSGS) [`BSGS`](/code/number_theory.h)
        - Extended BSGS [`ext_BSGS`](/code/number_theory.h)
        - Sqrt [`mod_sqr`](/code/number_theory.h)
        - Primitive Root [`primitive_root`](/code/number_theory.h)
        - N-th Root [`nth_root`](/code/number_theory.h)
        - Miller-Rabin [`miller_rabin`](/code/number_theory.h)
        - Pollard-Rho [`find_prime_factors`](/code/number_theory.h)
    - Fast Fourier Transform (FFT)
        - FFT [`misc.h:FFT`](/code/misc.h)
        - Number-Theoretic Transform (NTT) [`number_theory.h:NTT`](/code/number_theory.h)
        - Fast Walsh-Hadamard Transform (FWT) [`number_theory.h:FWT`](/code/number_theory.h)
    - Matrix [`matrix.h`](/code/matrix.h)
        - Matrix [`matrix`](/code/matrix.h)
        - Gaussian Elimination [`gaussian_elimination`](/code/matrix.h)
- Misc [`code/`](/code)
    - Longest Increasing Sequence (LIS) [`extra.h:LIS::LIS`](/code/extra.h)
    - Counting DP [`extra.h:solve`](/code/extra.h)
    - Sprague-Grundy Function [`misc.h:get_SG`](/code/misc.h)
    - Mo's Algorithm [`extra.h`](/code/extra.h)
        - 2D [`MO::MO_2`](/code/extra.h)
        - 3D [`MO::MO_3`](/code/extra.h)
        - On Tree (2D) [`MO_on_tree::MO_2_on_tree`](/code/extra.h)
    - CDQ [`extra.h:CDQ::cdq`](/code/extra.h)
    - Divide & Conquer with FFT [`extra.h:divide_and_conquer_fft::solve`](/code/extra.h)
    - Fast Input [`extra.h:fast_input`](/code/extra.h)
