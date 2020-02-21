# b7notes
This set of notes contains more rigorous extensions to the content of the B7: Symmetry course taught in Part II Chemistry at University of Cambridge.
The course itself is very interesting and insightful, but there is only so much that can be contained formally in the course.
I have therefore written these notes to provide, firstly, more preliminary mathematics so that the concepts in the course can be appreciated on more formal grounds, and secondly, a broader discussion for the supervision questions that aims to place the seemingly mundane exercises in a larger and hopefully more exciting context of quantum physics and chemistry.

## Current Status
I have decided to make public and share the whole `git` repository so that everyone can contribute to this, if they so wish.
At the moment, I am still writing the **Preliminaries** section to introduce group and representation theories more rigorously, but I hope to be able to advance to the core component of the notes where I can actually discuss the questions, and which will be more useful for exam purposes.

## Compilation
The required packages and libraries should be obvious from the preamble. But in particular:
  * `lualatex` with `-shell-escape` and ` PGFPLOTS 1.16` are required to compile the main TeX document and the `TikZ` and `PGFPLOTS` figures;
  * `biber` is required to compile the References (not that there is any reference at the moment).
 
`texlive 2019` as-is should contain all of the required packages and libraries. The latest packages updated via `MiKTeX` by June 2019 should do the job too.

Note that `tikzexternalize` is used in this document to generate some figures. All figures have thus been precompiled, so if one wants to avoid recompiling them, please make sure that the boolean `\tikzex` is set to `false`, i.e., comment out `\tikzextrue` and uncomment `\tikzexfalse` in the preamble:
```
%\tikzextrue
\tikzexfalse
```

A `Makefile` will be produced to simplify all of the above.
