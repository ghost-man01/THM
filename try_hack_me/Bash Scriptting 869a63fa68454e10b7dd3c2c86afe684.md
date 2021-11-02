# Bash Scriptting

## #### Bash Scripting

- **$#** is used to get number of arguments used in whole script.
- **$0** is used to get the first argument of script.

## #### Variables

~~To declare **variable**  **name=“Siddhant”**echo $name~~

> #!/bin/bash
> 
> 
> echo “enter your name”
> read name  echo $name is awesome.
> 

## #### Arrays

In **Array** each items stands for a number.  ~~Number indexing with **0** **@** is used for printing all arguments.  If we want to change or delete element we use** unset** array~~

> #!/bin/bash transport=(‘car’ ‘train’ ‘bus’) echo “${transport[@]}" echo "${transport[1]}”
> 

> unset transport[1] transport[1]=trainride echo “$transport[@]”
>