# wabt

## Quick Start

	docker run -it -v %cd%/samples:/samples zimkal/wabt bash

	root@7cc57a094a63:/# /wabt/bin/wasm-decompile /samples/helloworld.wasm
	export memory memory(initial: 1, max: 0);

	data d_helloworld(offset: 8) = "hello world\0a";

	import function wasi_snapshot_preview1_fd_write(a:int, b:int, c:int, d:int):int;

	export function start() {
	0[0]:int = 8;
	4[0]:int = 12;
	wasi_snapshot_preview1_fd_write(1, 0, 1, 20);
	}
