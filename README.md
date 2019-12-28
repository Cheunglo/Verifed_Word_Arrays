# Verifed_Word_Arrays
Cogent is a restricted, pure, polymorphic functional programming language
with uniqueness types and no runtime environment and nor garbage
collector. It has a certifying compiler which produces, when given a Cogent
program, an Isabelle/HOL shallow embedding of the Cogent program, C code
and an Isabelle/HOL proof that the C code is a refinement of the shallow
embedding. Cogent was designed to be used to implement trustworthy and
efficient systems code. Cogent currently does not support recursion,
instead it has a foreign function interface (FFI) to C, where recursive
functions and data types that require iteration are defined and called by
Cogent through its FFI.

The main task of this project is to verify the functional correctness of
Cogent's word array datatype which is written in C.
Word arrays are a commonly used data structure, especially in low level
systems, so verifying these would be beneficial as this would reduce the
overall cost of verification of any project that requires word arrays.

[![DOI](https://zenodo.org/badge/230601479.svg)](https://zenodo.org/badge/latestdoi/230601479)
