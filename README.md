# PowerSlot UNLEASHED RP2 firmware

This is essentially simply standard micropython, but the REPL is also duplicated to UART0 so it can be served over the network

## Build instructions

- Build micropython from master source according to docs
- apply micropython.patch to the master source
- create symlink ports/rp2/boards/powerslot pointing to ./board/
- Build with `make BOARD=powerslot PICO_BOARD_HEADER_DIRS=path/to/./board/`
