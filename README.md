This is a bash script which functions as a todo list.
It was designed to work well for those who like to set their tasks on a day by day basis, rather than weekly or some other scheme.
In order to use you will need to go into the script and at the top of the file:

1) Change the TODO_PATH to a folder on your computer with read and write enabled.
2) change TEXT_EDITOR to a text editor of your choice.

In order to use run "todo h" and check out the output:
```
usage: todo [arg]
h: print this help
num: edit todo list num days into future
dd/mm/yyyy: edit date's todo list, can use dd/ or dd/mm as well
c: clear old dates
```
For instance "todo 0" will edit the current day's todo list, "todo 5/7" will edit the todo list for July 5th of the current year, and "todo" will print a todo list.

When making the todo list you should separate tasks by line breaks, for example:
```
run and frollick
eat cheese
write 20,000 lines of code
```
Now when you run "todo" it looks like:
```
(1) run and frollick
(2) eat cheese
(3) write 20,000 lines of code
```
The program will delete a todo file if it sees you edit it to be empty, otherwise it will leave them unless you run "todo c" to clear old dates.
This can function as a graveyard of failed tasks to feel badly about yourself.
