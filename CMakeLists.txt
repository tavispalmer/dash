cmake_minimum_required(VERSION 3.10.0)
project(dash VERSION 0.1.0 LANGUAGES C)

add_compile_definitions(BSD=1 SHELL)
add_compile_options(-Wall -include config.h)

include_directories(. src)

add_executable(dash
    src/alias.c
    src/arith_yacc.c
    src/arith_yylex.c
    src/cd.c
    src/error.c
    src/eval.c
    src/exec.c
    src/expand.c
    src/histedit.c
    src/input.c
    src/jobs.c
    src/mail.c
    src/main.c
    src/memalloc.c
    src/miscbltin.c
    src/mystring.c
    src/options.c
    src/parser.c
    src/redir.c
    src/show.c
    src/trap.c
    src/output.c
    src/bltin/printf.c
    src/system.c
    src/bltin/test.c
    src/bltin/times.c
    src/var.c
    src/builtins.c
    src/init.c
    src/nodes.c
    src/signames.c
    src/syntax.c
)
