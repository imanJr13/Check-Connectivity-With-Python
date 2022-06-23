# Check-Connectivity-With-Python
Check Connectivity With Python 
in ths code with python we check connectivity of server or url and then use windows alarm to notify user;

```
import os
import winsound as ws 

hostname = "1.1.1.1" #example
response = os.system("ping -c 1 " + hostname)

#and then check the response...
if response == 0:
  ws.Beep(200,1000) 
  ws.Beep(2000,1000)
else:
  print (hostname, 'is down!')
```
