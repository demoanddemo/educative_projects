# Solution Review: Find Maximum in a List

This lesson will explain how to find the maximum number in a list using for loop.

<details open="" class="styles__PageTOCStyled-sc-1u9xzlw-0 jghHvN" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; --tw-bg-opacity:1; background-color: rgba(245,245,245,var(--tw-bg-opacity)); border-radius: 4px; min-width: 280px;"><summary role="button" tabindex="0" class="styles__HeadingWrap-sc-1u9xzlw-1 kEPnVM" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; cursor: pointer; outline-style: none; padding: 4px 4px 4px 16px; border-width: 1px; border-style: solid; --tw-border-opacity:1; border-color: rgba(229,229,229,var(--tw-border-opacity)); border-top-left-radius: 4px; border-top-right-radius: 4px;"><div class="styles__HeadingWrapInner-sc-1u9xzlw-2 lazzRz" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: flex; -webkit-box-align: center; align-items: center;"><span class="text-base font-bold tracking-wide" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; font-size: 1rem; line-height: 1.5rem; font-weight: 700; letter-spacing: 0.025em;">We'll cover the following</span><button class="icon-default ml-auto rounded-none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; color: rgba(0, 0, 0, 0.5); font-style: inherit; font-variant: inherit; font-weight: 400; font-stretch: inherit; font-size: 0.9375rem; line-height: 1.5; font-family: inherit; margin: 0px 0px 0px auto; overflow: visible; text-transform: none; appearance: button; cursor: pointer; display: flex; align-items: center; justify-content: center; white-space: nowrap; border-radius: 0px; border-width: 0px; padding: 0.75rem; letter-spacing: 0.025em; --tw-text-opacity:1; transition-duration: 0.2s; background-color: transparent; outline: transparent solid 2px; outline-offset: 2px;"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-chevron-up"><polyline points="18 15 12 9 6 15"></polyline></svg></button></div></summary><div class="p-4" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; padding: 1rem;"><div class="markdown-container-div Markdown__MarkdownContainerDiv-sc-1j2yuel-6 jhbODO" height="auto" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; height: auto; width: 437.17px;"><div class="markdownViewer Markdown__Viewer-sc-1j2yuel-1 hnixJj" role="none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; --tw-text-opacity:1; color: rgba(61,61,78,var(--tw-text-opacity)); line-height: 1.7; outline: none; font-size: 18px; overflow-wrap: break-word; font-family: &quot;Nunito Sans&quot;;"><ul style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-top: 0px; margin-bottom: 10px; margin-left: -20px;"><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/N8pDgD7WBvK#Solution-for-Problem-Statement1:-Use-for-loop" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; --tw-text-opacity:1; display: flex;">Solution for Problem Statement1: Use for loop</a></li><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/N8pDgD7WBvK#Solution-For-Problem-Statement2:-Use-enumerate" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; --tw-text-opacity:1; display: flex;">Solution For Problem Statement2: Use enumerate</a></li></ul></div></div></div></details>

## Solution for Problem Statement1: Use `for` loop

The problem statement 1 states that the task is to find the maximum number in the list. The straight forward solution to the problem is:

- Save the value of the first index.
- Use for loop to iterate over the list, then compare the saved value with each value in the list. If any value in the list is greater than the saved value, update the saved value.

This can be seen more clearly in the following illustration.

![image-20210902103941914](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902103941914.png)

![image-20210902104003610](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902104003610.png)

![image-20210902104021916](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902104021916.png)



![image-20210902104036506](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902104036506.png)



The following python code helps to find a maximum number in a list using for loop.

``` python
def findMaximum(list):
    maximum = list[0]
    for x in list:
        if x > maximum:
            maximum = x
    return maximum
list=[1, 2, 3, 4, 5]
print(findMaximum(list))
```





Now, look at the solution below: you are required to print the index of the maximum value and also a maximum of a list.

## Solution For Problem Statement2: Use `enumerate`

The problem statement 2 states that the task is to find the maximum number along with the index of that max number in the list. The straight forward solution to the problem is:

- Save the first value in the list as the maximum.
- Use for loop to iterate over the enumerate list, then compare the saved value with each value in the list. If any value in the list is greater than the saved value, update the saved value.

This can be seen more clearly in the following illustration.

 ![image-20210902104412572](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902104412572.png)

![image-20210902104425670](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902104425670.png)

![image-20210902104438434](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902104438434.png)



![image-20210902104451365](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902104451365.png)

![image-20210902104504483](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902104504483.png)

![image-20210902104515738](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210902104515738.png)



The following python code helps to find a maximum number in a list and the index of a maximum number using for loop.

``` python
def findMaximumValueIndex(list):
    maximum = list[0]
    index = 0
    for i, value in enumerate(list):
        if value > maximum:
            maximum = value
            index = i
    return [index, maximum]
list = [1, 2, 3, 4, 5]
[index, maximum] = findMaximumValueIndex(list)

print("Index: ", index)
print("Maximum Value: ", maximum)
        
```



Let’s move on to the next problem.