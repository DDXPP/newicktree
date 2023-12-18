# newicktree

This is an expansion of the newicktree LaTeX package developed by [Geroge Savva](https://academic.oup.com/bioinformatics/article/20/14/2322/213985) which allows the drawing of phylogenetic trees from Newick format. The package is an interface to PSTricks and requires the use of XeLaTeX compiler to function correctly.

The expansion include the ability of change node color, node shape, and branch color. 

An example to use this updated version is shown below.

```
\usepackage{newicktree}
\begin{newicktree}
    \Curvedbranches
    \Uptree
    \drawtree{(A:1[bn=a,bc=orange,nc=violet,ns=\TC], 
            ((B:2[bn=b,bc=green,nc=pink,ns=\Ttri], 
                    (D:1[bn=d,bc=red,nc=purple,ns=\Toval], 
                    E:2[bn=e,bc=brown,nc=yellow,ns=\Tdia]):1.5):1,
            C:1.5[bn=c,bc=blue,nc=cyan,ns=\Tf]):2.5[bn=,bc=green,nc=,ns=]):1;}
\end{newicktree}

```


The paper introducing newicktree provides a link to a page which no longer exists. No further development of the package has been done to my knowledge.

This repo was originally forked from GitHub user [Qiang Wang](https://github.com/wang-q).
