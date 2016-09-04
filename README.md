# brainfuck-starter
Brainfuck code examples

## Mul

Calculate `#1 * #2`. Store result in `#1`

~~~brainfuck
> +++        #2 = 3
[< ++++ > -] Multiplication by 4. Store result in #1
~~~

Calculate `#1 * #2`. Store result in `#2`

~~~brainfuck
+++          #1 = 3
[> ++++ < -] Multiplication by 4. Store result in #2
~~~

## Div

Calculate `#1 / 3`. Store result in `#2`

~~~brainfuck
++++++++++++ #1 = 12
[--- > + <]  Divide by 3. Store in #2
~~~

## Clone

Clone `#1` to `#2`

~~~brainfuck
+++            #1 = 3
[>>+<<-]       Move #1 to #3
>>[<+ <+ >>-]  Clone #3 to #2 and #1
<<             #1
~~~

## Add

Add `#1` to `#2`. Store result in `#1`

~~~brainfuck
++++      #1 = 4
> +++     #2 = 3
[< + > -] Addition, store result in #1
~~~

Add `#1` to `#2`. Store result in `#2`

~~~brainfuck
++++        #1 = 4
> +++       #2 = 3
< [> + < -] Addition, store result in #2
~~~

## Subtract

Subtract `#2` of `#1`

~~~brainfuck
++++      #1 = 4
> +++     #2 = 3
[< - > -] Subtraction
~~~

## Print

`Hello, World!` to console

~~~brainfuck
Initialize tab: 40 70 100
++++++++++ [- > ++++ > +++++++ > ++++++++++ <<<]
>>++.             H (72)
>+.               e (101)
+++++++..         ll (108)
+++.              o (111)
<<++++.           comma (44)
------------.     space (32)
>+++++++++++++++. W (87)
>.                o (111)
+++.              r (114)
------.           l (108)
--------.         d (100)
<<+.              ! (33)
<++++++++++       LF (10)
~~~

Single number

~~~brainfuck
++                        #1 = 2
> ++++++ [< ++++++++ > -] Add 48
< .                       Print #1
~~~
