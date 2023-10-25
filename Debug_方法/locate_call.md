# 定位代码中哪里调用了函数
```
import inspect

def ....
   frame = inspect.currentframe()
   caller_frame = inspect.getouterframes(frame, 2)
   print(f"Function called from {caller_frame[1][1]} at line {caller_frame[1][2]}")
```
  最终能够输出:
 ``` 
  Function called from /your/code/path at line XXX
```
