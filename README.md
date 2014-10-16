WordSmith tools
===============

Put keywords in a separate column.


Example
-------

WordSmith output (with *** as search word marker):

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

- input.txt = export from WordSmith
- output.csv = something you can open in Excel
