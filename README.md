# r2tips

#1. Mostly Called Function

Want to see in the binary that which functions are called more frequently / Have higest xreference ?
```sh
afl,xref/sort/dec,1/head/10
```
![tips1](https://github.com/apkunpacker/r2tips/assets/27184655/087537b2-2ae6-42c6-82b3-dede74413df0)

#2. Syscalls Resolver
Stuck in reversing ? use r2 magic to reveal syscalls with name 
```sh
e asm.os=linux
/as
```
![tips2](https://github.com/apkunpacker/r2tips/assets/27184655/95e579fb-c5b6-4067-b297-56e6986a0401)

