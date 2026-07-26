# hexcoder

POSIX `sh` script that encodes a string to hexadecimal or decodes a hexadecimal string to ASCII (via `xxd`).

### Requirements

- `sh` (any POSIX shell)
- `xxd`
- `grep` (for hex / printable checks)

### Usage

```sh
./hexcoder <string>
```

- If the argument looks like hex (`0-9`, `a-f`, `A-F`), it is **decoded** to ASCII.
- Otherwise, if it is printable text, it is **encoded** to uppercase hex.

### Examples

```sh
./hexcoder hello
# 68656C6C6F

./hexcoder 68656C6C6F
# hello
```

### Install (optional)

```sh
install -m 755 hexcoder /usr/local/bin/hexcoder
```
