Wordsmith tools
===============

Put keywords in a separate column.


Example
-------

Wordsmith output:

    N | Concordance              |
    1 | ...foo foo***bar baz...  |
    2 | ...foo Foo***bar, baz... |
    3 | ...foo bar***bar baz...  |

Columns in Excel:

    N | Before | Word   | After    | Simple |
    1 | ...foo | foobar |  baz...  | foobar |
    2 | ...foo | Foobar | , baz... | foobar |
    3 | ...foo | barbar |  baz...  | barbar |


Usage
-----

    python3 wordsmith-cleanup < input.txt > output.csv

Here:

- input.txt = export from Wordsmith
- output.csv = something you can open in Excel
