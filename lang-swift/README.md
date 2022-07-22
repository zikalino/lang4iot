


# Swift on ESP32



## Compiling HelloWorld!




........................................
    rustc +nightly --target wasm32-unknown-unknown -O /samples/helloworld-rust.rs

First output size is: helloworld-rust.wasm (1712472)

    wasm-gc /samples/helloworld-rust.wasm /samples/helloworld-rust-small.wasm

Then size is 49787


# References

https://swiftwasm.org


https://github.com/swiftwasm/swift


https://book.swiftwasm.org/getting-started/setup.html

https://github.com/swiftwasm/swiftwasm-docker/blob/main/5.6/ubuntu/18.04/Dockerfile

