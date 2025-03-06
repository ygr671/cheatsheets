# C Cheatsheet
## Hello World
```c
#include <stdio.h>

int main(void)
{
  printf("Hello World\n");
  return 0;
}
```
## Basics
### Program structure
```c
#include <header_file.h>

int main()
{
  // code
  return 0; // optional since C99 
}
```
### Compilation and execution
#### Compilation
```bash
gcc program.c -o program
```
Add there flags options for compilations etc (warnings, including object files, headers, ...).
#### Execution
```bash
./program
```
### Data types
#### Primitive data types
```c
// All the types size depends on the architecture. Here, x86_64 sizes are taken for example.
char a = 'a'; // containing a single character (8 bits) available in signed and unsigned variants.
short b = 1; // signed short integer (going from -32768 to +32767, 16 bits).
unsigned short c = 65535; // unsigned short integer (going from 0 to +65535).
int d = 100; // signed integer (going from -2147483648 to +2147483647, at least 16 bits but could go to 32).
unsigned int e = 4294967295; // unsigned integer (going from 0 to +4294967295, at least 16 bits but could go to 32)
long f = 1337; // signed long integer (going from -2147483648 to +2147483647, 32 or 64 bits)
unsigned long g = 99; // unsigned long integer (going from 0 to +4294967295, 32 or 64 bits)
long long h = 123456789; // signed long long integer (going from -9223372036854775808 to +9223372036854775807, 64 bits)
unsigned long long i = 1234567890987654321; // unsigned long long integer (going from 0 to 18446744073709551615, 64 bits)
float j = 3.14; // single precision floating point (going from 1.175494351 × 10⁻³⁸ to 3.402823466 × 10³⁸, 6 to 9 significant digits, 32 bits on nearly every architecture)
double k = 9.99; // double precision floating point (going from 2.2250738585072014 × 10⁻³²³ to 1.7976931348623157 × 10³⁰⁸, 15 to 17 significant digits, 64 bits on nearly every architecture)
long double l = 4.44; // extended precision floating point (going from 3.3621031431120935 × 10⁻³²⁸ to 1.1897314953572317 × 10³²⁸, 33 to 36 significant digits, 128 bits)
void m; // void

```

