# Solution Review: Implement Getter Methods

This lesson gives the solution to the previous exercise - implementing the getter methods to calculate the width and height of a rectangle.

<details open="" class="styles__PageTOCStyled-sc-1u9xzlw-0 jghHvN" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; --tw-bg-opacity:1; background-color: rgba(245,245,245,var(--tw-bg-opacity)); border-radius: 4px; min-width: 280px;"><summary role="button" tabindex="0" class="styles__HeadingWrap-sc-1u9xzlw-1 kEPnVM" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; cursor: pointer; outline-style: none; padding: 4px 4px 4px 16px; border-width: 1px; border-style: solid; --tw-border-opacity:1; border-color: rgba(229,229,229,var(--tw-border-opacity)); border-top-left-radius: 4px; border-top-right-radius: 4px;"><div class="styles__HeadingWrapInner-sc-1u9xzlw-2 lazzRz" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: flex; -webkit-box-align: center; align-items: center;"><span class="text-base font-bold tracking-wide" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; font-size: 1rem; line-height: 1.5rem; font-weight: 700; letter-spacing: 0.025em;">We'll cover the following</span><button class="icon-default ml-auto rounded-none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; color: rgba(0, 0, 0, 0.5); font-style: inherit; font-variant: inherit; font-weight: 400; font-stretch: inherit; font-size: 0.9375rem; line-height: 1.5; font-family: inherit; margin: 0px 0px 0px auto; overflow: visible; text-transform: none; appearance: button; cursor: pointer; display: flex; align-items: center; justify-content: center; white-space: nowrap; border-radius: 0px; border-width: 0px; padding: 0.75rem; letter-spacing: 0.025em; --tw-text-opacity:1; transition-duration: 0.2s; background-color: transparent; outline: transparent solid 2px; outline-offset: 2px;"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-chevron-up"><polyline points="18 15 12 9 6 15"></polyline></svg></button></div></summary><div class="p-4" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; padding: 1rem;"><div class="markdown-container-div Markdown__MarkdownContainerDiv-sc-1j2yuel-6 jhbODO" height="auto" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; height: auto; width: 248.008px;"><div class="markdownViewer Markdown__Viewer-sc-1j2yuel-1 hnixJj" role="none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; --tw-text-opacity:1; color: rgba(61,61,78,var(--tw-text-opacity)); line-height: 1.7; outline: none; font-size: 18px; overflow-wrap: break-word; font-family: &quot;Nunito Sans&quot;;"><ul style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-top: 0px; margin-bottom: 10px; margin-left: -20px;"><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/NEX1Y1VVwOL#Solution:" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; --tw-text-opacity:1; display: flex;">Solution:</a></li></ul></div></div></div></details>

## Solution:

The getter methods are written in the lines 11-15 in the following code playground. The `width()` and `height()` methods simply subtract the x and y coordinates respectively and return the result.

This solution is illustrated in the following figure:



![image-20210903112556392](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112556392.png)

![image-20210903112607329](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112607329.png)

![image-20210903112620070](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112620070.png)

![image-20210903112632675](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112632675.png)

![image-20210903112643215](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112643215.png)

![image-20210903112656445](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112656445.png)



![image-20210903112708180](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112708180.png)

![image-20210903112724400](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112724400.png)

![image-20210903112736533](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112736533.png)

![image-20210903112747410](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112747410.png)

![image-20210903112757867](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112757867.png)

![image-20210903112807750](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112807750.png)

![image-20210903112818944](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112818944.png)

![image-20210903112829123](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112829123.png)

![image-20210903112839213](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112839213.png)

![image-20210903112850985](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112850985.png)

![image-20210903112902347](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112902347.png)

![image-20210903112914305](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112914305.png)

![image-20210903112925875](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112925875.png)

![image-20210903112939623](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112939623.png)

![image-20210903112955861](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903112955861.png)

![image-20210903113005833](C:\Users\DEMO\AppData\Roaming\Typora\typora-user-images\image-20210903113005833.png)



The following code illustrates the concept:

``` python
class Rectangle:
  def __init__(self, x1, y1, x2, y2): # class constructor
    if x1<x2 and y1>y2:
      self.x1 = x1 # class variable
      self.y1 = y1 # class variable
      self.x2 = x2 # class variable
      self.y2 = y2 # class variable
    else:
      print("Incorrect coordinates of the rectangle!")
        
  def width(self):
    return self.x2-self.x1
      
  def height(self):
    return self.y1-self.y2
  
rectangle = Rectangle(2, 7, 8, 4)
print(rectangle.width())
print(rectangle.height())
```



Now, let’s expand this challenge by implementing the area and perimeter methods in the next lesson.