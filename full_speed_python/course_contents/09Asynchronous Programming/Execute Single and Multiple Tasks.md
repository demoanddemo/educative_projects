# Execute Single and Multiple Tasks

This lesson will teach you cooperative multitasking to execute single and multiple tasks using python.

<details open="" class="styles__PageTOCStyled-sc-1u9xzlw-0 jghHvN" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; --tw-bg-opacity:1; background-color: rgba(245,245,245,var(--tw-bg-opacity)); border-radius: 4px; min-width: 280px; user-select: text !important;"><summary role="button" tabindex="0" class="styles__HeadingWrap-sc-1u9xzlw-1 kEPnVM" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; cursor: pointer; outline-style: none; padding: 4px 4px 4px 16px; border-width: 1px; border-style: solid; --tw-border-opacity:1; border-color: rgba(229,229,229,var(--tw-border-opacity)); border-top-left-radius: 4px; border-top-right-radius: 4px; user-select: text !important;"><div class="styles__HeadingWrapInner-sc-1u9xzlw-2 lazzRz" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: flex; -webkit-box-align: center; align-items: center; user-select: text !important;"><span class="text-base font-bold tracking-wide" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; font-size: 1rem; line-height: 1.5rem; font-weight: 700; letter-spacing: 0.025em; user-select: text !important;">We'll cover the following</span><button class="icon-default ml-auto rounded-none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; color: rgba(0, 0, 0, 0.5); font-style: inherit; font-variant: inherit; font-weight: 400; font-stretch: inherit; font-size: 0.9375rem; line-height: 1.5; font-family: inherit; margin: 0px 0px 0px auto; overflow: visible; text-transform: none; appearance: button; cursor: pointer; display: flex; align-items: center; justify-content: center; white-space: nowrap; border-radius: 0px; border-width: 0px; padding: 0.75rem; letter-spacing: 0.025em; --tw-text-opacity:1; transition-duration: 0.2s; user-select: text !important; background-color: transparent; outline: transparent solid 2px; outline-offset: 2px;"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-chevron-up"><polyline points="18 15 12 9 6 15"></polyline></svg></button></div></summary><div class="p-4" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; padding: 1rem; user-select: text !important;"><div class="markdown-container-div Markdown__MarkdownContainerDiv-sc-1j2yuel-6 jhbODO" height="auto" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; height: auto; width: 248.011px; user-select: text !important;"><div class="markdownViewer Markdown__Viewer-sc-1j2yuel-1 cMsgN" role="none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; --tw-text-opacity:1; color: rgba(61,61,78,var(--tw-text-opacity)); line-height: 1.7; outline: none; font-size: 18px; overflow-wrap: break-word; font-family: &quot;Nunito Sans&quot;; user-select: text !important;"><ul style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-top: 0px; margin-bottom: 10px; user-select: text !important; margin-left: -20px;"><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; user-select: text !important; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/qVQxW4Dk8Ek#Co-operative-Multitasking" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; user-select: text !important; --tw-text-opacity:1; display: flex;">Co-operative Multitasking</a></li><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; user-select: text !important; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/qVQxW4Dk8Ek#Execute-a-Single-Task" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; user-select: text !important; --tw-text-opacity:1; display: flex;">Execute a Single Task</a></li><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; user-select: text !important; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/qVQxW4Dk8Ek#Execute-Multiple-Tasks" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; user-select: text !important; --tw-text-opacity:1; display: flex;">Execute Multiple Tasks</a></li></ul></div></div></div></details>

In **asynchronous programming**, the execution of a function is usually non-blocking. In other words, each time you call a function it returns immediately. However, that function does not necessarily get executed right away. Instead, there is usually a mechanism (called the “scheduler”) which is responsible for the future execution of the function.

The problem with asynchronous programming is that a program may end before any asynchronous function starts. A common solution for this is for asynchronous functions to return “futures” or “promises”. These are objects that represent the state of execution of an async function. Finally, asynchronous programming frameworks typically have mechanisms to block or wait for those async functions to end based on those “future” objects.

### Co-operative Multitasking[#](https://www.educative.io/courses/full-speed-python/qVQxW4Dk8Ek#Co-operative-Multitasking)

Since Python 3.6, the `asyncio` module combined with the `async` and `await` keyword allows us to implement what is called *co-operative multitasking programs*. In this type of programming, a coroutine function voluntarily yields control to another coroutine function when idle or when waiting for some input.

Asynchronous functions are declared with `async def`.

``` python
import asyncio
async def functionName():
    await asyncio.sleep(1)
    return

```



### Execute a Single Task[#](https://www.educative.io/courses/full-speed-python/qVQxW4Dk8Ek#Execute-a-Single-Task)

To call an asynchronous function once, do the following:-

1. Create an event loop
2. Run async function and wait for completion
3. Close the loop

``` python
# Create an event loop
loop = asyncio.get_event_loop()

# Run async function and wait for completion
results = loop.run_until_complete(functionName())

# Close the loop
loop.close()
```





Consider the following asynchronous function that squares a number and sleeps for one second before returning. (Ignore the `await` keyword for now.)

``` python
import asyncio

async def square(x):
    print('Square', x)
    await asyncio.sleep(1)
    print('End square', x)
    return x * x

# Create event loop
loop = asyncio.get_event_loop()

# Run async function and wait for completion
results = loop.run_until_complete(square(1))
print(results)

# Close the loop
loop.close()
```





The event loop for [asynchronous Programming](https://docs.python.org/3/library/asyncio-eventloop.html) is, among other things, the Python mechanism that schedules the execution of asynchronous functions. We use the loop to run the function until completion. This is a synchronizing mechanism that makes sure the next print statement doesn’t execute until we have some results.

### Execute Multiple Tasks[#](https://www.educative.io/courses/full-speed-python/qVQxW4Dk8Ek#Execute-Multiple-Tasks)

The previous example is not a good example of asynchronous programming because we don’t need that much complexity to execute only one function. However, imagine that you would need to execute the `square(x)` function three times, like this:

``` python
square(1)
square(2)
square(3)
```

To call an asynchronous function to execute multiple tasks, do the following:- 1.Create an event loop 2.Run async function and wait for completion

```python
# Create event loop
loop = asyncio.get_event_loop()

# Run async function and wait for completion
results = loop.run_until_complete(asyncio.gather(
functionName()
functionName()
.
.
.
functionName())

# Close the loop
loop.close()
```

Since the `square()` function has a sleep function inside, the total execution time of this program would be 3 seconds. However, given that the computer is going to be idle for a full second each time the function is executed, why can’t we start the next call while the previous is sleeping? Here’s how we do it:

``` python
import asyncio

async def square(x):
    print('Square', x)
    await asyncio.sleep(1)
    print('End square', x)
    return x * x

# Create event loop
loop = asyncio.get_event_loop()
…loop.close()
```





Basically, we use `asyncio.gather(*tasks)` to inform the loop to wait for all tasks to finish. Since the coroutines will start at almost the same time, the program will run for only 1 second. Asyncio **gather()** won’t necessarily run the coroutines by order, although it will return an ordered list of results.

Sometimes results may be needed as soon as they are available. For that, we can use a second coroutine that deals with each result using `asyncio.as_completed()`:

``` python
import asyncio

async def square(x):
    print('Square', x)
    await asyncio.sleep(1)
    print('End square', x)
    return x * x

# Create event loop
loop = asyncio.get_event_loop()

async def when_done(tasks):
    for res in asyncio.as_completed(tasks):
        print('Result:', await res)

loop = asyncio.get_event_loop()
loop.run_until_complete(when_done([
    square(1),
    square(2),
    square(3)
]))
```



Finally, async coroutines can call **other async coroutine functions** with the **await** keyword:

``` python
import asyncio

async def compute_square(x):
    await asyncio.sleep(1)
    return x * x

async def square(x):
    print('Square', x)
    res = await compute_square(x)
    print('End square', x)
    return res
  
# Create event loop
loop = asyncio.get_event_loop()

async def when_done(tasks):
    for res in asyncio.as_completed(tasks):
        print('Result:', await res)

loop = asyncio.get_event_loop()
loop.run_until_complete(when_done([
    square(1),
    square(2),
    square(3)
]))
```



Now that you have a clear concept of asynchronous programming, let’s test your knowledge in the upcoming exercises.