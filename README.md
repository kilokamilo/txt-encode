# txt-encode

Encodes text.

## hexcoder

Zsh script that encodes a string to hexadecimal or decodes a hexadecimal string to ASCII (via `xxd`).

### Requirements

- `zsh`
- `xxd`

### Usage

```bash
./hexcoder <string>
```

- If the argument looks like hex (`0-9`, `a-f`, `A-F`), it is **decoded** to ASCII.
- Otherwise, if it is printable text, it is **encoded** to uppercase hex.

### Examples

```bash
./hexcoder hello
# 68656C6C6F

./hexcoder 68656C6C6F
# hello
```

### Install (optional)

```bash
install -m 755 hexcoder /usr/local/bin/hexcoder
```
