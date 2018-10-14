# Python

- <a href="variable">variable</a>
- <a href="condition">condition</a>
- <a href="loop">loop</a>

Module

- <a href="file">File</a>
- JSON
- System

## Variable

```python
var1 = "Hello"
print(var1)
```

## Condition

```python
test = False

if not test:
    print("Hello world")
else:
    print("Never print")
```

## Loop

```python
some_data = ["test","testing","foo"]

for i,val in enumerate(some_data):
    print(str(i) + "-" + val)
```

## File

### Read

```python
# Read each line of a file and store the result
result = []
with open(filename) as domains:
    results = domains.read().splitlines()
```

```python
# Read all the file and store it
file = open('testfile.text', 'r') 
print file.read() 
```