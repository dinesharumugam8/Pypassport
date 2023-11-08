# Pypassport

pypassport for python3

Tested working so far:

from pypassport.reader import ReaderManager
from pypassport.epassport import EPassport, mrz
r = ReaderManager()
reader = r.waitForCard()
p = EPassport(reader,"YOURMRZINFO")
p.register(print)
p.setCSCADirectory("C:\\TEMP")
p.doBasicAccessControl()
p.doActiveAuthentication()

p['DG2']

