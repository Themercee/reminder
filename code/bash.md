# Bash

- Variable
- Condition
- Loop
- Parse args from command line

## Variable

```bash
# Assign value to variable
myvar=1
echo $myvar

#Increment variable
myvar=1
let myvar+=1 # echo 2
```

## Condition

```bash
# String comparison
if [ "foo" = "foo" ]; then
    echo expression evaluated as true
fi

# Oneliner
if [ -z "foo" ]; then echo Hello; fi
```

## Loop
### Basic
```bash
for VAR in $(cat file.txt)
do
    echo $VAR
done
```


---

### Classic with range
```bash
for i in {1..5}
do
    echo "Welcome $i times"
done
```



### One line print file line by line
```bash
for VAR in $(cat file.txt); do echo $VAR; done;
```


## Parse arguments from command line

```bash
while [[ $1 ]]
do
    case "$1" in
        --all | -a)
            all=true
            shift
            ;;
        -h)
            printUsage
            exit 1
            ;;
        *)
            break
            ;;
    esac
done
```