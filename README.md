# libft

My implementation of the 42 school's libft project - a remake of C libraries with additional utility functions.

## 📚 About

This project is my extended version of the 42 school's libft assignment. While it includes all the required functions from the curriculum, I've added several useful additions to make it more practical for real-world usage.

## 📂 Project Structure
```
.
├── libft.h         # Main header file
├── Makefile        # Build configuration
├── obj/            # Object files directory (created during build)
└── *.c             # Source files
```

## 🛠️ Functions

### IS Functions (11)
```c
int ft_isalnum(int c);    // Check if character is alphanumeric
int ft_isalpha(int c);    // Check if character is alphabetic
int ft_isascii(int c);    // Check if character is ASCII
int ft_isdigit(int c);    // Check if character is digit
int ft_isprint(int c);    // Check if character is printable
int ft_isblank(int c);    // Check if character is blank
int ft_isspace(int c);    // Check if character is whitespace
int ft_isodd(int n);      // Check if number is odd
int ft_iseven(int n);     // Check if number is even
int ft_iswithin(long long n, long long l, long long h);  // Check if number is within range
int ft_isvalid_integer_str(const char *str, int base);   // Validate integer string
```

### String Functions (14)
```c
size_t  ft_strlen(const char *s);
size_t  ft_strlcpy(char *dest, const char *src, size_t size);
size_t  ft_strlcat(char *dest, const char *src, size_t size);
char    *ft_strchr(const char *s, int c);
char    *ft_strrchr(const char *s, int c);
char    *ft_strnstr(const char *big, const char *little, size_t len);
char    *ft_strdup(const char *s);
char    *ft_substr(char const *s, unsigned int start, size_t len);
char    *ft_strjoin(char const *s1, char const *s2);
char    *ft_strtrim(char const *s1, char const *set);
char    **ft_split(char const *s, char c);
int     ft_strncmp(const char *s1, const char *s2, size_t n);
char    *ft_strmapi(char const *s, char (*f)(unsigned int, char));
void    ft_striteri(char *s, void (*f)(unsigned int, char*));
```

### Memory Functions (7)
```c
void    ft_bzero(void *s, size_t n);
void    *ft_memset(void *s, int c, size_t n);
void    *ft_memcpy(void *dest, const void *src, size_t n);
void    *ft_memmove(void *dest, const void *src, size_t n);
void    *ft_memchr(const void *s, int c, size_t n);
int     ft_memcmp(const void *s1, const void *s2, size_t n);
void    *ft_calloc(size_t nobj, size_t size);
```

### Translation Functions (6)
```c
int     ft_toupper(int c);
int     ft_tolower(int c);
int     ft_atoi(const char *str);
int     ft_abs(int num);
char    *ft_itoa(int n);
long    ft_strtol(const char *str, char **endptr, int base);
```

### I/O Functions (4)
```c
void    ft_putchar_fd(char c, int fd);
void    ft_putstr_fd(char *s, int fd);
void    ft_putendl_fd(char *s, int fd);
void    ft_putnbr_fd(int n, int fd);
```

## 🚀 Compilation and Usage

### Building the Library

The project includes a Makefile with the following rules:

```bash
make        # Compile the library
make clean  # Remove object files
make fclean # Remove object files and library
make re     # Rebuild everything
```

Compilation flags used:
- `-Wall -Wextra -Werror -g`
- Compiler: cc
- Archiver: ar rcs

### Using in Your Project

1. Clone the repository:
```bash
git clone https://github.com/hermeszi/libft.git
```

2. Include the header in your source files:
```c
#include "libft.h"
```

3. Compile with the library:
```bash
cc your_program.c -L. -lft
```

## 📜 License

This project is part of 42 school's curriculum. Feel free to use it as a reference, but please be mindful of the school's academic integrity policies.
Also, I am constantly experimenting with different code, so the functions may not work as described.


## 👤 Author

- myuen (42 Singapore)
