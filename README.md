# Lucky

Project initialized with:
- `cargo init`
- `cargo new sena`
- `cargo new cli`

Then to imports in packages, cargo build and cargo run build properly the Cargo.toml file were initialized with _virtual workspace_ config:

```toml
[workspace]
members = [ "cli","sena" ]
resolver = '2'

[workspace.package]
name = "lucky"
version = "0.1.0"
edition = "2021"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[workspace.dependencies]

# internal libraries
sena = { path = "sena" }
```

### Adding packages:

- `cargo new sena`