# ft_printf

**ft_printf** recreates the behavior of the standard C function `printf()`.  

It reinforces my understanding of:
- **Variadic functions** (`stdarg.h`), which takes a variable number of arguments.
- **printf function's argument formatting**
---

## Features

`ft_printf` handles the following format specifiers:

| Specifier | Description | Example |
|------------|--------------|----------|
| `%c` | Print a single character | `'A' → A` |
| `%s` | Print a string | `"Hello" → Hello` |
| `%p` | Print a pointer address | `0x7ffeea1f42c0` |
| `%d` | Print a signed decimal integer | `42 → 42` |
| `%i` | Print a signed integer (same as `%d`) | `-42 → -42` |
| `%u` | Print an unsigned decimal integer | `3000000000 → 3000000000` |
| `%x` | Print a number in lowercase hexadecimal | `255 → ff` |
| `%X` | Print a number in uppercase hexadecimal | `255 → FF` |
| `%%` | Print a literal `%` character | `% → %` |

---
## Usage
### Requirement: 
Linux OS
### Installment:
#### 1. Clone the Repository
   ```bash
   git clone https://github.com/TrangPham93/ft_printf.git ft_printf
   cd ft_printf
   ```
#### 2. Compile the Project

```bash 
cc *.c 
```
#### 3. Run
 
```bash 
./a.out
```
