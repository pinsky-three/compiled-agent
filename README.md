# compiled-agent

Rust workspace for the `compiled-agent` project.

## Project Layout

```text
.
|-- Cargo.toml
|-- Cargo.lock
`-- crates
    `-- compiler
        |-- Cargo.toml
        |-- examples
        |   `-- basic
        |       `-- main.rs
        `-- src
            `-- main.rs
```

The workspace currently contains one binary crate:

- `compiler`: a Rust 2024 binary crate that currently prints `Hello, world!`.

## Requirements

- Rust toolchain with Rust 2024 edition support.
- Cargo.

If Rust is not installed, use [rustup](https://rustup.rs/) to install and manage the toolchain.

## Getting Started

Build the workspace:

```sh
cargo build
```

Run the compiler binary:

```sh
cargo run -p compiler
```

Run the basic example:

```sh
cargo run -p compiler --example basic
```

Run checks:

```sh
cargo check
```

Format the code:

```sh
cargo fmt
```

Run tests:

```sh
cargo test
```

## Development Notes

- Generated build output is written to `target/` and is ignored by Git.
- The workspace uses Cargo resolver version `3`.
- The `compiler` crate is intentionally minimal at this stage and is ready for future compiler implementation work.
