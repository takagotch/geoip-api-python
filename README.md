### geoip-api-python
---
https://github.com/appliedsec/pygeoip

```py
// tests/test_nespeed_cell.py
import unittest

import pygeoip
from tests.config import NETSPEEDCELL_DB_PATH

class TestGeoIPNetspeedCellFunctions(unittest.TestCase):
  
  def setUp(self):
    self.gi = pygeoip.GeoIP(NETSPEEDCELL_DB_PATH)
  
  def testNetSpeedByAddrWrapper(self):
    netspeed = self.gi.netspeed_by_addr('2.125.160.1')
    self.assertEqual(netspeed, 'Dialup')

```

```
```

```
```


