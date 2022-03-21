# Fizzy VM

## Quick Start

	docker run -it -v %cd%/samples:/samples zimkal/vm-fizzy bash

	root@f7a6c4086bd0:/# ./fizzy/build/bin/fizzy-wasi /samples/helloworld.wasm
	hello world
