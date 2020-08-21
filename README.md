# `compiler-builtins`
Fork of [compiler-builtin](https://github.com/rust-lang/compiler-builtins) from
rust for zynq, with fast memcpy function adapted from newlib. We have to fork it
because the compiler-builtins would use their slow memcpy implementation for
compiler intrinsics regardless if you provided you own memcpy.
[#253](https://github.com/rust-lang/compiler-builtins/issues/253).

The memcpy function is in assembly with neon optimization.

