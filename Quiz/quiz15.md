# Quiz 15
## Prompt
There are N closed doors in a school and N students present. The first student opens all the doors. The second student closes every second door. The third student toggles every third door (closes if open, opens if closed) and so on.

HL: Create a function that shows number of doors that are open after N students have passed through the school.

## Folw Diagram

## Code Structure
#There are N closed doors in a school and N students present. The first student opens all the doors. The second student closes every second door. The third student toggles every third door (closes if open, opens if closed) and so on.
#HL: Create a function that shows number of doors that are open after N students have passed through the school.

#Example: Input 10 returns 3
#Example: Input 100 returns 10

def open_doors(n):
    doors = [False] * n
    for i in range(n):
        for j in range(i, n, i+1):
            doors[j] = not doors[j]
    return sum(doors)

print (open_doors(100))

print (open_doors(100))
```
![](quiz15.png)

