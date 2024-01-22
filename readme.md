This is just a script on how to access remote terminal sessions through Socket connection using Reverse TCP Shellcode that is written in rust

## How to examine it ?

First install cargo , the project manager and the build tool for rust, assuming you are using linux , otherwise fuckOff

```Bash
    curl https://sh.rustup.rs -sSf | sh
```

Then clone the repository

```Bash
    git clone https://github.com/Skythrill256/reverse-shell
```

then install the dependencies that are listed in cargo.toml

```Bash
    cargo build
```

now compile and execute the rust code 

```Bash
    cargo run
```
now open a new terminal and go to the same directory and compile the c code

```Bash
    gcc main.c
```
you will see nothing here but in the first terminal that you compiled the rust code , run the command 

```Bash
    tty
```

you might see this output

```Bash
    /dev/pts/1
```

do the same thing in the terminal you have compiled the c code 

you might see the same output 

because you are in the same session of seconed in the first one :)

and yes it is a virus .....
