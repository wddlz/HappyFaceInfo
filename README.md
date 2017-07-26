# HappyFaceInfo
Descriptions for the HappyFace project and paper that is too long to fit within the limits of the VL/HCC submission
# Python Library Features
- AST library ([Python 2](https://docs.python.org/2/library/ast.html) | [Python 3](https://docs.python.org/3/library/ast.html))
  - Abstract Syntax Tree module that helps discover the grammar structure of Python 2 or 3 code. 
  - Full list of nodes located in section 32.2.2 for each library.
- Keywords ([Python 2](https://docs.python.org/2/library/keyword.html) | [Python 3](https://docs.python.org/3/library/keyword.html))
  - Reserved Python 2 or 3 keywords such as `if`, `else`, `True`, and `False`.
- Builtins ([Python 2](https://docs.python.org/2/library/__builtin__.html) | [Python 3](https://docs.python.org/3/library/builtins.html))
  - Built-in objects for Python 2 or 3, including built-in functions (`abs()`, `len()`), constants (`True`, `False`, `None`), and types like boolean operations (`or`, `and`, `not`), comparsion operations (`<`, `>`, `is`), and numeric types (`int`, `float`, `complex`).
# Stylometric Features 
- Derived from [De-anonymizing Programmers via Code Stylometry, Caliskan et al.](https://www.usenix.org/system/files/conference/usenixsecurity15/sec15-paper-caliskan-islam.pdf)
  - We used the features present in tables 2, 3, and most features in table 4. 
# Wordgrams
- Wordgrams extracted using regex to detect commonly used words in the code snippets.
  - Ex. ThisWordGram becomes [This, Word, Gram].
  - Wordgrams are extracted in hopes of discovering words associated with frustration.
# Frustration Score
- Obtained through user selection of affect on the HappyFace survey.
  - Scores from 1 to 5 (happy to frustrated).
# Table of Features
| Feature | Description  |
| :---:   | :-: |
| Wordgrams | Frequency of specfic words occuring in source code |
| Each count of the following | Chars, underscores, tabs, spaces, and all whitespace in source code |
| Lines start with comment | Frequency of lines starting with a comment |
| Comments | Amount of individual comments |
| Empty lines | Frequency of completely empty lines |
| Line count | Amount of lines in the code snippet |
| Tab starts line | How many lines start with a tab character |
| Average line length | The average length of the lines of code, in chars |
| Std of line length | Standard deviation of line length of the source code |
| Python keywords | Total count of reserved keywords in the Python language |
| Python builtins | Total count of builtin objects (functions, constants, and types) in the Python language |
| Unique keywords | Count of unique keywords and builtins used |
| AST nodes | Count of each AST node present in code, extracted by parsing and traversing the AST |
| Errors | Specific errors that occur when code is parsed into AST |
