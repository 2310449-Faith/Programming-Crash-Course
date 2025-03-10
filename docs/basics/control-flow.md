# Control Flow

Control Flow is used to determine what code gets executed.

---

## Conditions

Conditions are statements that result in a [boolean](./variables.md#boolean).

``` python
ans = "the sky red?"
# ans = No
```

## Conditional Statements

### If-Else Statements

If-else are statement in which if the condition is true, the if block code is executed.
For values where condition is false, the else block is executed.

``` mermaid
graph LR
  A[Start]
  B{"Am I Tired"}
  C["Sleep"]
  D["Code More"]
  E["Do Something"]

  A --> B
  B -- Yes --> C --> E
  B -- No --> D ---> E
```

``` python
ans = 2
if ans >= 0:
  return "Yes"
else:
  return "No"
# Output: Yes
```
In this example, 2>0, hence return Yes.

## Loops

### For Loop
For loop goes through a sequence of element one by one, executing the block of code within itself

``` python
friends = ["alice","bella","charlie"]
for i in friends:
  print (i)
''' Output: alice
            bella
            charlie
'''
```

### While Loop
While loop executes the block of code within itself as long as the condition holds true

``` python
number = 5
while number > 0: 
  print (number)
  number -= 1  #reduces number by one each time, i.e. 5-1=4, 4-1=3, etc
''' Output: 5
            4
            3
            2
            1
'''
```
In this case, as long as number>0, the number gets printed.
At the point where number =0, while loop terminates. 
Hence, the final number printed is 1.

### Further Reading: Do-while loop, Nested loops.


