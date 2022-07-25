# contest-init
Simple utility to initialize the contest folder with .cpp files by some template. Probably will work on windows, as it's using unistd, but i don't actually care.

## Compile
```bash
$ gcc -O3 init.c -o init
```

## Usage
If the `template/init.cpp` dir is subdirectory of a current directory:
```bash
$ init div2.123 A B C D E
```
If you want to use the custom template:
```bash
$ init div2.123 A B C D E --custom-dir=/home/user/temp/custom.cpp
```

As the result you will get the subdirectory `div2.123` with `A.cpp-E.cpp` files, which will be basically the copies of your template.
