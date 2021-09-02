# Recursion

Now that we are familiar with functions, let's have a review on the most important concept using a function: recursion.

<details open="" class="styles__PageTOCStyled-sc-1u9xzlw-0 cgYZlm" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; --tw-bg-opacity:1; background-color: rgba(245,245,245,var(--tw-bg-opacity)); border-radius: 4px; min-width: 280px;"><summary role="button" tabindex="0" class="styles__HeadingWrap-sc-1u9xzlw-1 kEPnVM" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; cursor: pointer; outline-style: none; padding: 4px 4px 4px 16px; border-width: 1px; border-style: solid; --tw-border-opacity:1; border-color: rgba(229,229,229,var(--tw-border-opacity)); border-top-left-radius: 4px; border-top-right-radius: 4px;"><div class="styles__HeadingWrapInner-sc-1u9xzlw-2 lazzRz" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: flex; -webkit-box-align: center; align-items: center;"><span class="text-base font-bold tracking-wide" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; font-size: 1rem; line-height: 1.5rem; font-weight: 700; letter-spacing: 0.025em;">We'll cover the following</span><button class="icon-default ml-auto rounded-none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; color: rgba(0, 0, 0, 0.5); font-style: inherit; font-variant: inherit; font-weight: 400; font-stretch: inherit; font-size: 0.9375rem; line-height: 1.5; font-family: inherit; margin: 0px 0px 0px auto; overflow: visible; text-transform: none; appearance: button; cursor: pointer; display: flex; align-items: center; justify-content: center; white-space: nowrap; border-radius: 0px; border-width: 0px; padding: 0.75rem; letter-spacing: 0.025em; --tw-text-opacity:1; transition-duration: 0.2s; background-color: transparent; outline: transparent solid 2px; outline-offset: 2px;"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-chevron-up"><polyline points="18 15 12 9 6 15"></polyline></svg></button></div></summary><div class="p-4" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; padding: 1rem;"><div class="markdown-container-div Markdown__MarkdownContainerDiv-sc-1j2yuel-6 jhbODO" height="auto" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; height: auto; width: 248.021px;"><div class="markdownViewer Markdown__Viewer-sc-1j2yuel-1 jwYbFw" role="none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; --tw-text-opacity:1; color: rgba(61,61,78,var(--tw-text-opacity)); line-height: 1.7; outline: none; font-size: 18px; overflow-wrap: break-word; font-family: &quot;Nunito Sans&quot;;"><ul style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-top: 0px; margin-bottom: 10px; margin-left: -20px;"><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/JYWP54Eq549#What-Is-Recursion?" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; --tw-text-opacity:1; display: flex;">What Is Recursion?</a></li><ul style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-top: 0px; margin-bottom: 0px; margin-left: -20px;"><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/JYWP54Eq549#Parts-of-a-Recursion" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; --tw-text-opacity:1; display: flex;">Parts of a Recursion</a></li></ul></ul></div></div></div></details>

## What Is Recursion?

Recursion is when a function calls itself again and again until it reaches the base condition.

### Parts of a Recursion

There are two parts of recursion: `base condition` and `recursive function`.

For instance, take the example of a Factorial function.

Factorial(!) of a number n is the product of all positive numbers from our chosen number n down to 1.

```python
factorial(n) = 0   if n is 0 #base case
                        
factorial (n) = n * factorial(n-1) #recursive function                      
```

Let’s use an example of factorial of 5.

```python
5! = 5 × 4!
   = 5 × 4 × 3!
   = 5 × 4 × 3 ×2! 
   = 5 × 4 ×3 ×2 ×1
   = 120 
```

Below is the call to the function factorial given 5 as a parameter to the function. factorial(5)

It is calculated recursively in the following manner:

![image-20210826154355530](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210826154355530.png)

![image-20210826154410897](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210826154410897.png)

![image-20210826154424793](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210826154424793.png)

![image-20210826154442105](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210826154442105.png)

![image-20210826154454058](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210826154454058.png)

![image-20210826154504115](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210826154504115.png)

![image-20210826154515910](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210826154515910.png)

![image-20210826154526125](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210826154526125.png)







Basically, the factorial of 5 is 5 times the factorial of 4, etc. Finally, the factorial of 1 (or of zero) is 1 which breaks the recursion. In Python, we could write the following recursive function:

``` python
def factorial(n):
    if(n <= 1):
        return 1
    else:
        return (n * factorial(n - 1))
print("Factorial:")
print(factorial(5))
```





The trick with recursive functions is that there must be a “base” case where the recursion must end with a recursive case that iterates towards the base case. In the case of factorial, we know that the factorial of zero is one, and the factorial of a number greater than zero will depend on the factorial of the previous number until it reaches zero.

Now that the concept of ‘Recursion’ in python is clear, let’s check your knowledge in the upcoming exercises before moving on to the next chapter —‘Iteration and Loops’.