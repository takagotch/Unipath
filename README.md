### unipath
---
https://github.com/mikeorr/Unipath


```py
// test.py
from __future__ import print_function

import ntpath
import os

import pytest

from unipath import *
from unipath.errors import *
from unipath.tools import dict2dir, dump_path

AbstractPath.auto_norm = False

class PosixPath(AbstractPath):
  pathlib = posixpath
  
class NTPath(AbstractPath):
  pathlib = ntpath
  
cleanup = not bool(os.environ.get("NO_CLEANUP"))
dump = bool(os.environ.get("DUMP"))



```

```
```

```
```
