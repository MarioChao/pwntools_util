# Welcome to pwntools util!

This Python package is a wrapper class for Gallopsled's [pwntools](https://www.pwntools.com). It's created to facilitate different aspects of writing a pwntools program.

```py
from pwntools_util import PwnUtil

ppp = PwnUtil()
ppp.connectRemote('example.com', 352)

n = ppp.getNumberFromLine()
ppp.sendline('the payload')
ppp.interactive()

ppp.disconnect()
```
