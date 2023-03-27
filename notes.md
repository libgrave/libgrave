# Note 1

I want to be able to write some C code and have Watcom translate it to assembly. Based on
[this](https://stackoverflow.com/questions/74209302/how-to-make-watcom-c-compiler-wcc-and-wasm-generate-the-same-8086-machine-code),
I can use:

    wcc -s -ms -os -0 test.c


# Note 2

I want to be able to create a function in asm file and have it linked with the main program in c file. Based on
[this](https://cboard.cprogramming.com/c-programming/22587-linking-functions-asm-file.html)
I need to use something along those lines:

```
.model large,c
.code

public _asmf1
_asmf1	proc
	nop
	ret
_asmf1	endp
 
end
```

and in C code, declare:

    extern void asmf1(void);
