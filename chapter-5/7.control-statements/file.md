# Command Chaining in the Shell

## 5.7.1 Semicolon (`;`)

### Syntax
```bash
command1; command2; command3
```

The semicolon (`;`) character is used to execute multiple commands consecutively. Each command runs independently of the others. Regardless of the success or failure of the first command, the next command executes after the current one completes.

### Example
To display the calendars for January, February, and March of 2030:
```bash
cal 1 2030; cal 2 2030; cal 3 2030
```
#### Output:
```
    January 2030                                                        
Su Mo Tu We Th Fr Sa                                                            
       1  2  3  4  5                                                            
 6  7  8  9 10 11 12                                                            
13 14 15 16 17 18 19                                                            
20 21 22 23 24 25 26                                                            
27 28 29 30 31                                                                 
                                                                                
   February 2030                                                                
Su Mo Tu We Th Fr Sa                                                            
                1  2                                                            
 3  4  5  6  7  8  9                                                            
10 11 12 13 14 15 16                                                            
17 18 19 20 21 22 23                                                            
24 25 26 27 28                                                                 
                                                                                
     March 2030                                                                 
Su Mo Tu We Th Fr Sa                                                            
                1  2                                                            
 3  4  5  6  7  8  9                                                            
10 11 12 13 14 15 16                                                            
17 18 19 20 21 22 23                                                            
24 25 26 27 28 29 30                                                            
31                       
```

---

## 5.7.2 Double Ampersand (`&&`)

### Syntax
```bash
command1 && command2
```

The double ampersand (`&&`) acts as a logical "AND" operator. The second command runs only if the first command is successful. If the first command fails, the second command will not execute.

### Success and Failure in Commands
A command is considered **successful** if it completes without errors (exit code 0) and **fails** if it encounters an error (non-zero exit code).

### Examples
1. The first command succeeds, so the second command executes:
   ```bash
   ls /etc/ppp && echo success
   ```
   
   #### Output:
   ```
   ip-down.d  ip-up.d
   success
   ```

2. The first command fails, so the second command does not execute:
   ```bash
   ls /etc/junk && echo success
   ```

   #### Output:
   ```
   ls: cannot access /etc/junk: No such file or directory
   ```

---

## 5.7.3 Double Pipe (`||`)

### Syntax
```bash
command1 || command2
```

The double pipe (`||`) acts as a logical "OR" operator. If the first command runs successfully, the second command is skipped. If the first command fails, the second command executes.

### Examples
1. The first command succeeds, so the second command is skipped:
   ```bash
   ls /etc/ppp || echo failed
   ```
   #### Output:
   ```
   ip-down.d  ip-up.d
   ```

2. The first command fails, so the second command executes:
   ```bash
   ls /etc/junk || echo failed
   ```
   #### Output:
   ```
   ls: cannot access /etc/junk: No such file or directory
   failed
   ```

---
