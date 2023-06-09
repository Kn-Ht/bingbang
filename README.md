# bingbang

*bingbang* is a stack-based esoteric programming language, developed just for fun.

#### hello world program:

```
'Hello World!'P
```

this is first parsed into `Instructions`,

```
[ Instruction::PushString('hello world!'), Instructions::PrintLine ]
```

then it is run by the interpreter.

---

# todo

- [ ] nested if statements
- [ ] functions (goto)
- [ ] error handling
- [ ] Assembly backend

# operators

operators require at least 2 elements on the stack

| operator | instruction  |
| -------- | ------------ |
| +        | plus         |
| -        | sub          |
| *        | mul          |
| /        | div          |
| =        | is equal to  |
| >        | greater than |
| <        | less than    |

# character table

| character | actions                               | requirements      |
| --------- | ------------------------------------- | ----------------- |
| ''        | push string                           | -                 |
| 0..9      | push number                           | -                 |
| ,         | ignore (push)                         | -                 |
| ?         | if                                    | stack length >= 2 |
| a         | print stack                           | -                 |
| A         | print stack with newlines             | -                 |
| b         |                                       |                   |
| B         |                                       |                   |
| c         | clear stack                           | -                 |
| C         | clear screen                          | -                 |
| d         | drop element from stack               | -                 |
| D         |                                       |                   |
| e         |                                       |                   |
| E         |                                       |                   |
| f         |                                       |                   |
| F         |                                       |                   |
| g         |                                       |                   |
| G         |                                       |                   |
| h         |                                       |                   |
| H         |                                       |                   |
| i         | read input                            | -                 |
| I         |                                       |                   |
| j         |                                       |                   |
| J         |                                       |                   |
| k         |                                       |                   |
| K         |                                       |                   |
| l         |                                       |                   |
| L         |                                       |                   |
| m         |                                       |                   |
| M         |                                       |                   |
| n         | parse number                          | stack length >= 1 |
| N         |                                       |                   |
| o         |                                       |                   |
| O         |                                       |                   |
| p         | print                                 | stack length >= 1 |
| P         | print line                            | stack length >= 1 |
| q         | quit                                  | -                 |
| Q         |                                       |                   |
| r         | reverse string                        | stack length >= 1 |
| R         | reverse stack                         | -                 |
| s         | sum                                   | stack length >= 1 |
| S         | show stack (not popping)              |                   |
| t         | get the time in the format %d-%m-%Y   | -                 |
| T         | get the time in user-specified format | stack length >= 1 |
| u         |                                       |                   |
| U         |                                       |                   |
| v         |                                       |                   |
| V         |                                       |                   |
| w         |                                       |                   |
| W         |                                       |                   |
| x         |                                       |                   |
| X         |                                       |                   |
| y         |                                       |                   |
| Y         |                                       |                   |
| z         |                                       |                   |
| Z         |                                       |                   |
