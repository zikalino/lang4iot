# Rust on ESP32

https://github.com/espressif/rust-esp32-example#:~:text=%20Rust%20ESP32%20Example%20%201%20Setup.%20First,,Rust%20code.%20%204%20Flash.%20%20More%20


## Compiling HelloWorld!

    rustc +nightly --target wasm32-unknown-unknown -O /samples/helloworld-rust.rs

First output size is: helloworld-rust.wasm (1712472)

    wasm-gc /samples/helloworld-rust.wasm /samples/helloworld-rust-small.wasm

Then size is 49787
