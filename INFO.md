# Python Library Features
- AST library ([Python 2](https://docs.python.org/2/library/ast.html) | [Python 3](https://docs.python.org/3/library/ast.html))
  - Abstract Syntax Tree module that helps discover the grammar structure of Python 2 or 3 code. 
  - Full list of nodes located in section 32.2.2 for each library.
- Keywords ([Python 2](https://docs.python.org/2/library/keyword.html) | [Python 3](https://docs.python.org/3/library/keyword.html))
  - Reserved Python 2 or 3 keywords such as `if`, `else`, `True`, and `False`.
- Builtins ([Python 2](https://docs.python.org/2/library/__builtin__.html) | [Python 3](https://docs.python.org/3/library/builtins.html))
  - Built-in objects for Python 2 or 3, including built-in functions (`abs()`, `len()`), constants (`True`, `False`, `None`), and types like boolean operations (`or`, `and`, `not`), comparsion operations (`<`, `>`, `is`), and numeric types (`int`, `float`, `complex`).
# Stylometric Features 
- Derrived from [De-anonymizing Programmers via Code Stylometry, Caliskan et al.](https://www.usenix.org/system/files/conference/usenixsecurity15/sec15-paper-caliskan-islam.pdf)
  - We used the features present in tables 2, 3, and most features in table 4.
# Wordgrams
- Wordgrams extracted using regex to detect commonly used words in the code snippets.
  - Ex. ThisWordGram becomes [This, Word, Gram].
  - Wordgrams are extracted in hopes of discovering words associated with frustration.
# Frustration Score
- Obtained through user selection of affect on the HappyFace survey.
  - Scores from 1 to 5 (happy to frustrated).
