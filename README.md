# 0x19. C - Stacks, Queues - LIFO, FIFO

## Description

Tasks on .

What I learned from the tasks:

* What do LIFO and FIFO mean
* What is a stack, and when to use it
* What is a queue, and when to use it
* What are the common implementations of stacks and queues
* What are the most common use cases of stacks and queues
* What is the proper way to use global variables

---

## General Requirements
* Allowed editors: vi, vim and emacs.
* All files were created and compiled on Ubuntu 20.04.4 LTS using using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89```
* Code checked with betty-style.pl and betty-doc.pl

---

# Tasks

These are all the tasks of this project, the ones that are completed link to the corresponding files.

### [0. push, pall](./)
* Implement the push and pall opcodes.
* The push opcode
* The opcode push pushes an element to the stack.
  	- Usage: push <int>
		+ where <int> is an integer
	- if <int> is not an integer or if there is no argument given to push, print the error message L<line_number>: usage: push integer, followed by a new line, and exit with the status EXIT_FAILURE
		+ where is the line number in the file
	- You won’t have to deal with overflows. Use the atoi function
* The pall opcode
* The opcode pall prints all the values on the stack, starting from the top of the stack.
	- Usage pall
	- If the stack is empty, don’t print anything
### 1. pint
* Implement the pint opcode.
* The pint opcode
* The opcode pint prints the value at the top of the stack, followed by a new line.
	- Usage: pint
	- If the stack is empty, print the error message L<line_number>: can't pint, stack empty, followed by a new line, and exit with the status EXIT_FAILURE


### 2. pop
* Implement the pop opcode.
* The pop opcode
* The opcode pop removes the top element of the stack.
	- Usage: pop
	- If the stack is empty, print the error message L<line_number>: can't pop an empty stack, followed by a new line, and exit with the status EXIT_FAILURE


### 3. swap
* Implement the swap opcode.
	- Usage: swap
	- If the stack contains less than two elements, print the error message L<line_number>: can't swap, stack too short, followed by a new line, and exit with the status EXIT_FAILURE

### 4. add
* Implement the add opcode.
* The add opcode
* The opcode add adds the top two elements of the stack.
	- Usage: add
	- If the stack contains less than two elements, print the error message L<line_number>: can't add, stack too short, followed by a new line, and exit with the status EXIT_FAILURE
	- The result is stored in the second top element of the stack, and the top element is removed, so that at the end:
		+ The top element of the stack contains the result
		+ The stack is one element shorter

### 5. nop
* Implement the nop opcode.
* The nop opcode
* The opcode nop doesn’t do anything.
	- Usage: nop

### 6. sub
* Implement the sub opcode.
* The sub opcode
* The opcode sub subtracts the top element of the stack from the second top element of the stack.
	- Usage: sub
	- If the stack contains less than two elements, print the error message L<line_number>: can't sub, stack too short, followed by a new line, and exit with the status EXIT_FAILURE
	- The result is stored in the second top element of the stack, and the top element is removed, so that at the end:
	- The top element of the stack contains the result
	- The stack is one element shorter

### 7. div
* Implement the div opcode.
* The div opcode
* The opcode div divides the second top element of the stack by the top element of the stack.
	- Usage: div
	- If the stack contains less than two elements, print the error message L<line_number>: can't div, stack too short, followed by a new line, and exit with the status EXIT_FAILURE
	- The result is stored in the second top element of the stack, and the top element is removed, so that at the end:
		+ The top element of the stack contains the result
		+ The stack is one element shorter
	- If the top element of the stack is 0, print the error message L<line_number>: division by zero, followed by a new line, and exit with the status EXIT_FAILURE

### 8. mul
* Implement the mul opcode.
* The mul opcode
* The opcode mul multiplies the second top element of the stack with the top element of the stack.
	- Usage: mul
	- If the stack contains less than two elements, print the error message L<line_number>: can't mul, stack too short, followed by a new line, and exit with the status EXIT_FAILURE
	- The result is stored in the second top element of the stack, and the top element is removed, so that at the end:
		+ The top element of the stack contains the result
		+ The stack is one element shorter

### 9. mod
* Implement the mod opcode.
* The mod opcode
* The opcode mod computes the rest of the division of the second top element of the stack by the top element of the stack.
	- Usage: mod
	- If the stack contains less than two elements, print the error message L<line_number>: can't mod, stack too short, followed by a new line, and exit with the status EXIT_FAILURE
	- The result is stored in the second top element of the stack, and the top element is removed, so that at the end:
		+ The top element of the stack contains the result
		+ The stack is one element shorter
	- If the top element of the stack is 0, print the error message L<line_number>: division by zero, followed by a new line, and exit with the status EXIT_FAILURE

### 10. comments
* Every good language comes with the capability of commenting. When the first non-space character of a line is #, treat this line as a comment (don’t do anything).

### 11. pchar
* Implement the pchar opcode.
* The pchar opcode
* The opcode pchar prints the char at the top of the stack, followed by a new line.
	- Usage: pchar
	- The integer stored at the top of the stack is treated as the ascii value of the character to be printed
	- If the value is not in the ascii table (man ascii) print the error message L<line_number>: can't pchar, value out of range, followed by a new line, and exit with the status EXIT_FAILURE
	- If the stack is empty, print the error message L<line_number>: can't pchar, stack empty, followed by a new line, and exit with the status EXIT_FAILURE


# Manual


---

### Author
* **Dominic Samo** - (https://github.com/DominicSamoes)
