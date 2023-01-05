<h4> How to cat a file which name starts with - </h4>

```shell
cat ./-
```

<h4> How to cat a file which name has spaces fileName- "spaces in this filename" </h4>

```shell
cat 'spaces in this filename'
```
or
```shell
cat spaces\ in\ this\ filename
```
Here we used escape character

<h4> How to print content of each file in a directory with new line in the end </h4>

```shell
find . -exec awk 1 {} +
```
<h4> How to check file type </h4>

```shell
file fileName
```

<h4> Find file which is human readable, 1033 bytes in size and not executable </h4>
In 1033c, c reperents bytes.  
```shell
find . -readable -size 1033c -not -executable
```

<h4> The password for the next level is stored somewhere on the server and has all of the following properties:
owned by user bandit7, owned by group bandit6, 33 bytes in size </h4>
 
```shell
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
```
Here 2>/dev/null means redirect all the problematic message to linux dustbin called /dev/null  



