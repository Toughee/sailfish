# Installation

In order to use sailfish templates, you have add two dependencies in your `Cargo.toml`.

```toml
[dependencies]
sailfish = "0.2.2"
sailfish-macros = "0.2.2"
```

`sailfish` crate contains runtime for rendering contents, and `sailfish-macros` serves you derive macros to compile and import the template files.

These crates are separated so that Rust compiler can compile them independently. This separation makes your compilation faster!

!!! Warning
    Make sure that the `sailfish-macros` version is larger than `sailfish`, otherwise the compilation may fail.
