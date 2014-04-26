# Rust syntax highlighting problems

Good: function
``` rust
fn foo() {

}
```

Bad: function
``` rust
fn foo<'a>() {

}
```

Good: constant
``` rust
static bar: int = 5;
```

Bad: constant
``` rust
static bar: &'static str = "hello";
```

Good: struct
``` rust
struct Baz<T> {
    baz: T,
}
```

Bad: struct
``` rust
struct Baz<'a> {
    baz: &'a str,
}
```
