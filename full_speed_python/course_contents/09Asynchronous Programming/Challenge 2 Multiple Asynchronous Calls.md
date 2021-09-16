# Challenge 2: Multiple Asynchronous Calls

In this challenge, you are required to call the asynchronous function multiple times.

<details open="" class="styles__PageTOCStyled-sc-1u9xzlw-0 jghHvN" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; --tw-bg-opacity:1; background-color: rgba(245,245,245,var(--tw-bg-opacity)); border-radius: 4px; min-width: 280px; user-select: text !important;"><summary role="button" tabindex="0" class="styles__HeadingWrap-sc-1u9xzlw-1 kEPnVM" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; cursor: pointer; outline-style: none; padding: 4px 4px 4px 16px; border-width: 1px; border-style: solid; --tw-border-opacity:1; border-color: rgba(229,229,229,var(--tw-border-opacity)); border-top-left-radius: 4px; border-top-right-radius: 4px; user-select: text !important;"><div class="styles__HeadingWrapInner-sc-1u9xzlw-2 lazzRz" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: flex; -webkit-box-align: center; align-items: center; user-select: text !important;"><span class="text-base font-bold tracking-wide" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; font-size: 1rem; line-height: 1.5rem; font-weight: 700; letter-spacing: 0.025em; user-select: text !important;">We'll cover the following</span><button class="icon-default ml-auto rounded-none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; color: rgba(0, 0, 0, 0.5); font-style: inherit; font-variant: inherit; font-weight: 400; font-stretch: inherit; font-size: 0.9375rem; line-height: 1.5; font-family: inherit; margin: 0px 0px 0px auto; overflow: visible; text-transform: none; appearance: button; cursor: pointer; display: flex; align-items: center; justify-content: center; white-space: nowrap; border-radius: 0px; border-width: 0px; padding: 0.75rem; letter-spacing: 0.025em; --tw-text-opacity:1; transition-duration: 0.2s; user-select: text !important; background-color: transparent; outline: transparent solid 2px; outline-offset: 2px;"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-chevron-up"><polyline points="18 15 12 9 6 15"></polyline></svg></button></div></summary><div class="p-4" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; padding: 1rem; user-select: text !important;"><div class="markdown-container-div Markdown__MarkdownContainerDiv-sc-1j2yuel-6 jhbODO" height="auto" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; height: auto; width: 248.011px; user-select: text !important;"><div class="markdownViewer Markdown__Viewer-sc-1j2yuel-1 cMsgN" role="none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; --tw-text-opacity:1; color: rgba(61,61,78,var(--tw-text-opacity)); line-height: 1.7; outline: none; font-size: 18px; overflow-wrap: break-word; font-family: &quot;Nunito Sans&quot;; user-select: text !important;"><ul style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-top: 0px; margin-bottom: 10px; user-select: text !important; margin-left: -20px;"><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; user-select: text !important; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#Problem-Statement" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; user-select: text !important; --tw-text-opacity:1; display: flex;">Problem Statement</a></li><ul style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-top: 0px; margin-bottom: 0px; user-select: text !important; margin-left: -20px;"><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; user-select: text !important; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#Input" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; user-select: text !important; --tw-text-opacity:1; display: flex;">Input</a></li><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; user-select: text !important; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#Output" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; user-select: text !important; --tw-text-opacity:1; display: flex;">Output</a></li></ul><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; user-select: text !important; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#Coding-Exercise" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; user-select: text !important; --tw-text-opacity:1; display: flex;">Coding Exercise</a></li></ul></div></div></div></details>

## Problem Statement[#](https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#Problem-Statement)

Change the previous program to schedule the execution of two calls to the sum function.

### Input[#](https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#Input)

Two number n1 and n2

### Output[#](https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#Output)

The sum of two numbers in the order of the execution.

## Coding Exercise[#](https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#Coding-Exercise)

Write your code below. It is recommended that you try solving the exercise yourself before viewing the solution.

[Exercise](https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#)[Solution](https://www.educative.io/courses/full-speed-python/gxMKEQLwBPZ#)

``` python
import asyncio
async def sum(n1,n2):
  #Write code here
    return 
# Create event loop
# Run async function and wait for completion
# Close the loop
```

`Solution`

``` python
import asyncio

async def sum(n1,n2):
    print('Sum numbers',n1,'+',n2)
    await asyncio.sleep(1)
    print('End Sum',n1,'+',n2)
    return n1 + n2

# Create event loop
loop = asyncio.get_event_loop()

# Run async function and wait for completion
results = loop.run_until_complete(asyncio.gather(
    sum(1, 2),
    sum(2, 3),
    sum(3, 4)
))
print(results)

# Close the loop
loop.close()
```





Now, let’s move on to the detailed solution review of the above problem.