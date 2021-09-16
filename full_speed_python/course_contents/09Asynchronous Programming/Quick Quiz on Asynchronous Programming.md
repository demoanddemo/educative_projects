# Quick Quiz on Asynchronous Programming

1



Which of the following statements allow you to execute an asynchronous function `myPrint(x)` once?

Your Answer



A)

```python
import asyncio
async def myPrint(x): 
    print(x) 
    await asyncio.sleep(1)  
    return
loop = asyncio.get_event_loop()
results = loop.run_until_complete(myPrint(1))
loop.close()
```



B)

```pyhton
import asyncio
async def myPrint(x): 
    print(x) 
    await asyncio.sleep(1)  
    return
loop = asyncio.get_event_loop()results = loop.run_until_complete(asyncio.gather(myPrint(1))                                                      myPrint(2))
loop.close()
```

2

Which of the following statements allow you to execute an asynchronous function `myPrint(x)` multiple times?

A)

``` python
import asyncio
async def myPrint(x):
  print(x)
  await asyncio.sleep(1) 
  return

loop = asyncio.get_event_loop()
results = loop.run_until_complete(myPrint(1))
loop.close()
```

B)

``` python
import asyncio
async def myPrint(x):
  print(x)
  await asyncio.sleep(1) 
  return

loop = asyncio.get_event_loop()
results = loop.run_until_complete(asyncio.gather(myPrint(1), myPrint(2)))
loop.close()
```

