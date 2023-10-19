# r2tips
Radare2 project
https://github.com/radareorg/radare2

#1. Mostly Called Function

Want to see in the binary that which functions are called more frequently / Have higest xreference ?
```sh
afl,xref/sort/dec,1/head/10
```
![tips1](https://github.com/apkunpacker/r2tips/assets/27184655/087537b2-2ae6-42c6-82b3-dede74413df0)

#2. Syscalls Resolver

Stuck in reversing ? use r2 magic to reveal syscalls with its respective name and address
```sh
e asm.os=linux
/as
```
![tips2](https://github.com/apkunpacker/r2tips/assets/27184655/95e579fb-c5b6-4067-b297-56e6986a0401)

#3. Premium version of R2 🙂

Want to enjoy premium version of r2 , without buying a license ?
```sh
e scr.demo=true
```
![tips3](https://github.com/apkunpacker/r2tips/assets/27184655/7b394cbd-3bfb-4833-ba7f-b21ec1bbe709)

#4. Replace string with different string

Want to change any string present in the binary to something else ?
```sh
r2 -wqc 'w NewString @@/ OldString' FileName
```
Remember you have to change NewString and old string to your required one. Don't blindly run the command

Below I tried to chane /system/bin/ls to /system/bin/cp
![tips4](https://github.com/apkunpacker/r2tips/assets/27184655/8ac80610-4c1e-4852-a5eb-9316eed34702)

#5. Search values
Want to search specific value in the instructions which is present at the end of instruction but getting lots of result ?
```sh
/ad 0x10~0x10$
```
![tips5](https://github.com/apkunpacker/r2tips/assets/27184655/a25cd500-5704-44c0-bc5c-e7ad09d37ca4)
