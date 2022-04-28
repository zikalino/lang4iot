## Example

    docker run -it -v %cd%/samples:/samples zimkal/wasm-cheerp bash

    /opt/cheerp/bin/clang++ -target cheerp-wasm /samples/helloworld-c.c -O3 -o /samples/target.js


# References

Cheerp setup instructions for Ubuntu can be found here:

https://github.com/leaningtech/cheerp-meta/blob/master/pages/Ubuntu-Debian-installation-using-PPA.md

It works on **xenial**, doesn't work on **bionic** or **jammy** and **focal** due to unexisting references.

Using Cheerp:

https://docs.leaningtech.com/cheerp/Getting-started#hello-world
