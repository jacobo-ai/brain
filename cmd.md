
#linux     [[linux]]
File nav
File= Director 

```shell
cd 
```

into a directly named downloads and test.




how you view files
```shell
cat readme.md
```



how you edit files
```shell
nano readme.md
```


search for the specific contents of files, for example file readme.md 
```shell
grep "THM" readme.md
```


locates files
```shell
find -name passwords.txt 
```

looking for anything .txt star means looking for 

```shell
find -name *.txt
```

make a folder called test or directly. 
```shell
mkdir test
```

| symbol/operator | Description                                                                                                                                            |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| &               | This operator allows you to run commands in the background of your terminal                                                                            |
| &&              | This operator allows you to combine multiple commands together in one line of your terminal(the first operator has to work for the second one to work) |
| >               | This operator is a redirector- meaning that we can take the output from a command (such as using cat to output a file) and direct it elsewhere.        |
| >>              | This operator does the same function of the > operator but appends the output rather then replacing (meaning nothing is overwritten).                  |
