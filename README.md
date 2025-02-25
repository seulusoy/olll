This repo is forked from https://github.com/orisano/olll/.
When installation commands are run the original olll (https://github.com/orisano/olll/) is installed. You can change olll.py file of the original with olll.py here to run the optimized code.
Use on your own risk.

# oLLL

[![PyPI version](https://badge.fury.io/py/olll.svg)](https://badge.fury.io/py/olll)
[![Python Versions](https://img.shields.io/pypi/pyversions/olll.svg)](https://pypi.org/project/olll/)

A Python3 Implementation of LLL.

## Installation
```bash
python3 -m pip install olll
```
or
```bash
curl -O https://raw.githubusercontent.com/orisano/olll/master/olll.py
```

## Example
https://en.wikipedia.org/wiki/Lenstra%E2%80%93Lenstra%E2%80%93Lov%C3%A1sz_lattice_basis_reduction_algorithm#Example

```python
import olll

reduced_basis = olll.reduction([
  [1, 1, 1],
  [-1, 0, 2],
  [3, 5, 6],
], 0.75)

print(reduced_basis)
# [[0, 1, 0], [1, 0, 1], [-1, 0, 2]]
```

## Author
Nao Yonashiro(@orisano)
Sırrı Erdem ULUSOY(@seulusoy)

## License
MIT

## Reference
https://en.wikipedia.org/wiki/Lenstra%E2%80%93Lenstra%E2%80%93Lov%C3%A1sz_lattice_basis_reduction_algorithm
