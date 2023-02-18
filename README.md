# std.py
Import Python Standard Library (and `numpy`) by default

## Installation
Just put the file `std.py` into your `${PYTHONPATH}`

## Usage Example
```python
from std import *

# now you have access to the python standard library
stdin = '\n'.join(map(str.rstrip, sys.stdin.readlines()))
prefix = sys.argv[1] if len(sys.argv) > 1 else f'{datetime.date.today()}: '
indented = textwrap.indent(stdin, prefix=prefix)
print(indented)
```
