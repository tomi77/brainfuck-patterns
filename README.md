# brainfuck-starter
Brainfuck code examples

## Hello, World!

Print `Hello, World!` to console

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

## Mul

Calculate `#1 * #2`. Store result in `#1`

    >+++ [< ++++ >-]

Calculate `#1 * #2`. Store result in `#2`

    +++ [> ++++ <-]

## Div

Calculate `#1 / 3`. Store result in `#2`

    ++++++++++++ 12
    [>+ <---]    / 3 = 4 (store in #2)

## Clone

Clone `#1` to `#2`

    +++            #1 = 3
    [>>+<<-]       Move #1 to #3
    >>[<+ <+ >>-]  Clone #3 to #2 and #1
    <<             #1
