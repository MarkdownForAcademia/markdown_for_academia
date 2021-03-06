---
abstract: 'This is the abstract.

  It consists of two paragraphs.

  '
author: [Author One, Author Two]
tags: [nothing, nothingness]
title: 'This is the title: it contains a colon'
...

\newtheorem{MARKDOWN!}{MARKDOWN!}

\newtheorem{Theorem}{Theorem}

\newtheorem{lemma}{lemma}

\newtheorem{testing}{testing}




# test code

## use raw


~~~~{ .python caption="this is a test" label="raw code" }
for i in range([@testLabel])
  %---embed\---%
  test backslash \\
~~~~


## use file


~~~~{ .python caption="testing 2"  }
def resource():
    return "this file is used for testing"


print(resource())

~~~~


## minimal


~~~~{    }
for i in range(10):
    return i
~~~~



# test figure

## regular

![testing figure](./image/figure.PNG){  width=30% height=20 }

## minimal

![](./image/figure.PNG){    }

# test include

Hello, World
"'quote", good
"lala", "haha"
"testing", 2


# test table

## with file


Hello     World
-------  --------
'quote   good
lala     "haha"
testing  2

: testing table \label{tbl:test}

## with content


+---------------+---------------+--------------------+
| Fruit         | Price         | Advantages         |
+===============+===============+====================+
| Bananas       | $1.34         | - built-in wrapper |
|               |               | - bright color     |
+---------------+---------------+--------------------+
| Oranges       | $2.10         | - cures scurvy     |
|               |               | - tasty            |
+---------------+---------------+--------------------+

: I am excited \label{great table!}

## minimal


+---------------+---------------+--------------------+
| Fruit         | Price         | Advantages         |
+===============+===============+====================+
| Bananas       | $1.34         | - built-in wrapper |
|               |               | - bright color     |
+---------------+---------------+--------------------+
| Oranges       | $2.10         | - cures scurvy     |
|               |               | - tasty            |
+---------------+---------------+--------------------+

:  \label{}

# test theorem

## theorem


\begin{Theorem}
\label{tremendous}
this is a great theorem
\end{Theorem}

## lemma


\begin{MARKDOWN!}
\label{tremendous 2}
this is a great theorem
\end{MARKDOWN!}

## minimal


\begin{Theorem}
\label{}
this is another great theorem
\end{Theorem}


# test embedded block

## embed table file using include


+---------------+---------------+--------------------+
| Fruit         | Price         | Advantages         |
+===============+===============+====================+
| Bananas       | $1.34         | - built-in wrapper |
|               |               | - bright color     |
+---------------+---------------+--------------------+
| Oranges       | $2.10         | - cures scurvy     |
|               |               | - tasty            |
+---------------+---------------+--------------------+


:  \label{embeded table}

## embed file into code


~~~~{   label="should not compile embedded" }
==== table
screw up
====
~~~~


## embedded block with meta block


\begin{lemma}
\label{embedded theorem}

+---------------+---------------+--------------------+
| Fruit         | Price         | Advantages         |
+===============+===============+====================+
| Bananas       | $1.34         | - built-in wrapper |
|               |               | - bright color     |
+---------------+---------------+--------------------+
| Oranges       | $2.10         | - cures scurvy     |
|               |               | - tasty            |
+---------------+---------------+--------------------+

: this table is embedded into theorem \label{theorem table}
\end{lemma}

# test ref

## regular test

this is a ref to table \ref{great table!}

page ref \pageref{tremendous 2}


## test for later

see later theorem \ref{later_theorem}


\begin{testing}
\label{later_theorem}
another a great theorem
\end{testing}


# test escape

[@notfoundlabel]

[@tremendous 2]

[@tremendous 2]

[@test1]

# test constants

test 2

test1









