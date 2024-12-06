# libft
My implementation of the 42 school's libft project - a custom C library with essential functions.

## 📚 About

This project is my extended version of the 42 school's libft assignment. While it includes all the required functions from the curriculum, I've added several useful additions to make it more practical for real-world usage.

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

## 🚀 Usage

1. Clone the repository:
```bash
git clone https://github.com/[your-username]/libft.git
```

2. Compile the library:
```bash
make
```
This will create `libft.a`

3. To use in your project:
- Include the header:
```c
#include "libft.h"
```
- Compile with the library:
```bash
cc your_program.c -L. -lft
```

## ⚙️ Testing

- `make` - Compile the library
- `make clean` - Remove object files
- `make fclean` - Remove object files and the library
- `make re` - Recompile everything

## 📝 Notes

- All functions are norm-compliant (42 coding standards)
- Includes additional utility functions beyond the base requirements
- All memory operations are leak-free
- Compiles with -Wall -Wextra -Werror
- Includes useful macros (commented out in header due to norm)

## 📜 License

This project is part of 42 school's curriculum. Feel free to use it as a reference, but please be mindful of the school's academic integrity policies.

## ✨ Contributing

If you find any bugs or have suggestions for improvements:
1. Fork the project
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 👤 Author

- myuen (42 Singapore)
