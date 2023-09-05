# format syntax (used by many languages)

example (format content of data as strings): `fmt.Println("%s", data)`

%d          decimal integer
%x, %o, %b  integer in hexadecimal, octal, binary
%f, %g, %e  floating point numbers
%t          boolean
%c          rune (in go) - Unicode
%s          string
%q          quoted string "abc" or 'abc'
%v          any value in natural format
%T          type of any value
%%          literal percent sign
