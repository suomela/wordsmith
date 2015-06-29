WordSmith utilities
===================

Put keywords in a separate column.


Example
-------

WordSmith output (with *** as search word marker):

    WordSmith Tools 4.0
    
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

    python3 wordsmith-cleanup MARKER INPUT OUTPUT

Example:

    python3 wordsmith-cleanup '***' input.txt output.xlsx

Here:

- input.txt = export from WordSmith (as text)
- output.xlsx = something you can open in Excel


Dependencies
------------

Python 3 and XlsxWriter.

If you have OS X and Homebrew, use the following commands to install
everything:

    brew install python3
    pip3 install xlsxwriter

