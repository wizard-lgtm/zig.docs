
# Introduction
## 'Your path trought to be a ziglang master'

Ziglang is an a really amazing programming language. But the documentation of ziglang is kinda basic and giving you not so much examples. ([For example check out here:](https://www.reddit.com/r/Zig/comments/11o70by/what_sucks_about_zig/))

So my goal is creating the best educative ziglang documentation ever created. Some of textes are directly copied from ziglang.org offical documentation or any other resources. You can check references section at the bottom of the post.



## External resources to read
Ziglang.org documentation: https://ziglang.org/documentation/master/

Zig standart library documentation: https://ziglang.org/documentation/master/std/

Zig learn: https://zig.guide/

## What is zig programming language?

Zig is a general-purpose programming language and toolchain for maintaining robust, optimal, and reusable software. The syntax and main focus of ziglang is being simple for developers. 
This documentation sources are tested in 0.14.0-dev version.

## Installing Ziglang
You can install ziglang binary from [releases](https://github.com/ziglang/zig/releases)

or you can install "Zig Version Manager (Zvm)"
[Installation insturctions for zvm](https://github.com/tristanisham/zvm?tab=readme-ov-file#installing-zvm)
After you install, you may type

```bash
zvm i master
zvm use master
zig version
```
Or: Master is the nightly version of zig, if you want to install any version you can type
```bash
zvm i 0.13.0 # for example
zvm use 0.13.0
zig version # 0.13.0
```

## Hello world!

Let's create are first hello world program, zig file extension is `.zig`

***hello.zig***
```zig
const std = @import("std"); // importing standart library of ziglang
pub fn main()!void{
    std.debug.print("Hello world!\n");
}
```
Then run the code with
```bash
zig run ./hello.zig
Hello world!
```





