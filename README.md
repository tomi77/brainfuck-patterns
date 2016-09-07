# brainfuck-patterns
Brainfuck code patterns

## Mul

Calculate `#1 * #2`. Store result in `#1` [commented src](src/mul/store_in_1.b)

~~~brainfuck
>+++[<++++>-]
~~~

Calculate `#1 * #2`. Store result in `#2` [commented src](src/mul/store_in_2.b)

~~~brainfuck
+++[>++++<-]
~~~

## Div

Calculate `#1 / 3`. Store result in `#2` [commented src](src/div.b)

~~~brainfuck
++++++++++++[--->+<]
~~~

## Clone

Clone `#1` to `#2` [commented src](src/clone.b)

~~~brainfuck
+++[>>+<<-]>>[<+<+>>-]
~~~

## Add

Add `#1` to `#2`. Store result in `#1` [commented src](src/add/store_in_1.b)

~~~brainfuck
++++>+++[<+>-]
~~~

Add `#1` to `#2`. Store result in `#2` [commented src](src/add/store_in_2.b)

~~~brainfuck
++++>+++<[>+<-]
~~~

## Subtract

Subtract `#2` of `#1` [commented src](src/sub.b)

~~~brainfuck
++++>+++[<->-]
~~~

## Clean

Clean `#1` [commented src](src/clean.b)

~~~brainfuck
+++[-]
~~~

## Print

`Hello, World!` to console [commented src](src/print/hello_world.b)

~~~brainfuck
++++++++++[->++++>+++++++>++++++++++<<<]>>++.>+.+++++++..+++.<<++++.------------.>+++++++++++++++.>.+++.------.--------.<<+.<++++++++++
~~~

Single number [commented src](src/print/single_number.b)

~~~brainfuck
++>++++++[<++++++++>-]<.
~~~
