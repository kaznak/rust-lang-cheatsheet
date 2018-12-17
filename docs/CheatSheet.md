---
title: The Rust Programming Language Cheat Sheet
---

# Keywords
See : [Appendix A](https://doc.rust-lang.org/book/appendix-01-keywords.html)

## Currently in Use
	
as, break, const, continue, crate, dyn, else, enum, extern, false, fn, for, if, impl, in, let, loop, match, mod, move, mut, pub, ref, return, Self, self, static, struct, super, trait, true, type, unsafe, use, where, while

## Keywords Reserved for Future Use

abstract, async, become, box, do, final, macro, override, priv, try, typeof, unsized

## Raw identifiers
Raw identifiers let you use keywords where they would not normally be allowed by prefixing them with r#.

~~~
let r#fn = "this variable is named 'fn' even though that's a keyword";

// call a function named 'match'
r#match();
~~~

# Variables and Mutability
See : [Section 3.1](https://doc.rust-lang.org/book/ch03-01-variables-and-mutability.html)

~~~
let x = 5;                       // immutable variable x
x = 10;          // !!ERROR!!    // immutable variable raises an error on changing.
let x = "new value";             // immutable variable can be redefined of same name but even diffrent type of value.
let mut y = 5;                   // mutable variable y
y = 10;                          // mutable variable allow change its value.
y = "new value"; // !!ERROR!!    // changeing to different type value is profibited
const MAX_POINTS: u32 = 100_000; // constant require type annotation
~~~
