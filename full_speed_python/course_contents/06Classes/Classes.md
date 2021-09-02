# Classes

This lesson introduces object-oriented programming using classes, attributes, and methods.

<details open="" class="styles__PageTOCStyled-sc-1u9xzlw-0 jghHvN" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; --tw-bg-opacity:1; background-color: rgba(245,245,245,var(--tw-bg-opacity)); border-radius: 4px; min-width: 280px;"><summary role="button" tabindex="0" class="styles__HeadingWrap-sc-1u9xzlw-1 kEPnVM" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: block; cursor: pointer; outline-style: none; padding: 4px 4px 4px 16px; border-width: 1px; border-style: solid; --tw-border-opacity:1; border-color: rgba(229,229,229,var(--tw-border-opacity)); border-top-left-radius: 4px; border-top-right-radius: 4px;"><div class="styles__HeadingWrapInner-sc-1u9xzlw-2 lazzRz" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; display: flex; -webkit-box-align: center; align-items: center;"><span class="text-base font-bold tracking-wide" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; font-size: 1rem; line-height: 1.5rem; font-weight: 700; letter-spacing: 0.025em;">We'll cover the following</span><button class="icon-default ml-auto rounded-none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; color: rgba(0, 0, 0, 0.5); font-style: inherit; font-variant: inherit; font-weight: 400; font-stretch: inherit; font-size: 0.9375rem; line-height: 1.5; font-family: inherit; margin: 0px 0px 0px auto; overflow: visible; text-transform: none; appearance: button; cursor: pointer; display: flex; align-items: center; justify-content: center; white-space: nowrap; border-radius: 0px; border-width: 0px; padding: 0.75rem; letter-spacing: 0.025em; --tw-text-opacity:1; transition-duration: 0.2s; background-color: transparent; outline: transparent solid 2px; outline-offset: 2px;"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-chevron-up"><polyline points="18 15 12 9 6 15"></polyline></svg></button></div></summary><div class="p-4" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; padding: 1rem;"><div class="markdown-container-div Markdown__MarkdownContainerDiv-sc-1j2yuel-6 jhbODO" height="auto" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; height: auto; width: 323.109px;"><div class="markdownViewer Markdown__Viewer-sc-1j2yuel-1 hnixJj" role="none" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; --tw-text-opacity:1; color: rgba(61,61,78,var(--tw-text-opacity)); line-height: 1.7; outline: none; font-size: 18px; overflow-wrap: break-word; font-family: &quot;Nunito Sans&quot;;"><ul style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-top: 0px; margin-bottom: 10px; margin-left: -20px;"><li style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; margin-bottom: 5px; list-style: none;"><a href="https://www.educative.io/courses/full-speed-python/N87lk1gRl48#Classes" style="box-sizing: border-box; --tw-shadow:0 0 transparent; --tw-ring-inset:var(--tw-empty, ); --tw-ring-offset-width:0px; --tw-ring-offset-color:#fff; --tw-ring-color:rgba(59,130,246,0.5); --tw-ring-offset-shadow:0 0 transparent; --tw-ring-shadow:0 0 transparent; background-color: transparent; color: rgba(0,0,0,var(--tw-text-opacity)); text-decoration: none; transition: color 0.2s ease 0s; --tw-text-opacity:1; display: flex;">Classes</a></li></ul></div></div></div></details>

# Classes

In object-oriented programming (OOP), a class is a structure that allows you to group together a set of properties (called **attributes**) and functions (called **methods**) to manipulate those properties. Take the following class that defines a person with the `name` and `age` properties and the `greet()` method.

``` python
class Person:
    def __init__(self, name, age): # class constructor
        self.name = name # class variable
        self.age = age # class variable
        
    def greet(self): # class function to print a greeting
        print("Hello, my name is %s!" % self.name)
```



Most classes will need the constructor method (`__init__`) to **initialize** the class’s attributes. In the above code snippet, the constructor of the class receives the person’s name and age and stores that information in the **class’s instance** (referenced by the `self` keyword). Finally, the `greet()` method prints the name of the person as stored in a **specific class instance (object)**.

Here’s how we can instantiate two objects:

``` python
class Person:
    
    def __init__(self, name, age): # class constructor
        self.name = name # class variable
        self.age = age # class variable
    def greet(self): # class function to print a greeting
        print("Hello, my name is %s!" % self.name)
a = Person("Peter", 20) # instantiation
b = Person("Anna", 19) # instantiation

a.greet() # call a's greet method
b.greet() # call b's greet method

print(a.name)
print(a.age) # We can also access the attributes of an object

print(b.name)
print(b.age) # We can also access the attributes of an object
```

Let’s solve an exercise to practice the concepts you just learnt.