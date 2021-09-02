# Quick Quiz on Modules and Functions

1

What is the output of the following function?

``` python
def function(fruit = "Orange"):
  print("I like " + fruit)

function("Banana")
function("Peach")
function()
function("Mango") 
```

A)

```
I like BananaI like PeachI like OrangeI like Mango
```

B)

```
I like BananaI like PeachI like PeachI like Mango
```

C)

```
I like BananaI like PeachI like Mango
```

2

What is the output of the following function?

``` python
def function(x):
  return 5 +x

print(function(2))
print(function(4))
print(function(6)) 
```

A)

```
7
9
11 
```

B)

```
5
5
5
```

3

What is the output of the following code?

```  python
def recursion(k):
  if(k>0):
    result = k+recursion(k-1)
  else:
    result = 0
  return result

print(recursion(2))
```

A)

1

B)

3

Now that you have learned about modules and functions in Python, what if you want a set of instructions or structures to be repeated in a sequence a specified number of times? Let’s learn about “Iterations and Loops” in the next chapter.