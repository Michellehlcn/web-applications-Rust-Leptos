## JavaScript and ECMAScript

Potential downsides
- Dynamic typing - limits compile time safety checks and performance
- Null values - limits compile time safety checks 
- Garbage collection - can limit performance 

## Full stack Rust

- Front end - all the benefits of WebAssembly
- Front end and backend - memory and type safety guarantees of RYst
- Backend - Rust back-end frameworks are some of the highest performing options available
- Language isomorphism (one programming language accross all the entire stack)
- Frameworks for writing front-end and full-stack Rust 
    - Yew
    - Dioxus
    - Sycamore
    - Perseus
    - Leptos

- Leptos
    - Full stack in one project
    - Isomorphic functions 
    - Modeled after Solid.js
    - Actix Web or axum 
    - Hot-loading

## Installation
```
cargo install cargo-leptos
rustup target add wasm32-unknown-unknown
cargo leptos new --git leptos-rs/start
cargo leptos watch
```
## SSR Features

- Enabled by the bin crate
- Dependencies don't need to compile to WASM 
- Not part of the binary sent to the user's browser
- Backend logic will have the access to dependencies

## Hydrate Feature 

- Enabled by the lib crate
- Dependencies don't need to compile to WASM and will be sent to the user's browser
