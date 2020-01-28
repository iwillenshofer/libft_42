<p align="center">
	<img width="130px;" src="https://raw.githubusercontent.com/iwillenshofer/resources/main/images/42_logo_black.svg" align="center" alt="42" />&nbsp;&nbsp;&nbsp;
	<img width="130px" src="https://raw.githubusercontent.com/iwillenshofer/resources/main/achievements/libft.png" align="center" alt="libft" />
	<h1 align="center">libft</h1>
</p>
<p align="center">
	<img src="https://img.shields.io/badge/Success-107/100_✓-gray.svg?colorA=61c265&colorB=4CAF50&style=for-the-badge">
	<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black">
	<img src="https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white">
</p>

<p align="center">
	<b><i>Development repository for the 42cursus Libft project @ 42 São Paulo</i></b><br>
</p>

<p align="center">
	<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/iwillenshofer/libft?color=blueviolet" />
	<img alt="GitHub top language" src="https://img.shields.io/github/languages/top/iwillenshofer/libft?color=blue" />
	<img alt="GitHub top language" src="https://img.shields.io/github/commit-activity/t/iwillenshofer/libft?color=brightgreen" />
	<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/iwillenshofer/libft?color=brightgreen" />
</p>
<br>

> _This project is your very first project as a student at 42. You will need to recode a few functions of the C standard library as well as some other utility functions that you will use during your whole cursus._



<br>

<p align="center">
	<table>
		<tr>
			<td><b>Est. Time</b></td>
			<td><b>Skills</b></td>
			<td><b>Allowed Functions</b></td>
			<td><b>Difficulty</b></td>
		</tr>
		<tr>
			<td valign="top">70 hours</td>
			<td valign="top">
				<img src="https://img.shields.io/badge/Algorithms & AI-555">
				<img src="https://img.shields.io/badge/Imperative programming-555"><br>
				<img src="https://img.shields.io/badge/Rigor-555">
			</td>
			<td valign="top">
				<img src="https://img.shields.io/badge/malloc()-lightgrey">
				<img src="https://img.shields.io/badge/free()-lightgrey">
				<img src="https://img.shields.io/badge/write()-lightgrey">
			</td>
			<td valign="top"> 462 XP</td>
		</tr>
	</table>
</p>

<br>

### Usage
```bash
# create a main file.
$ make
$ gcc -L. -lft main.c
$ ./a.out
```

#### Example of main() file
```c
#include "libft.h"

int	main(void)
{
	char *s;
	char *string = "hello world";
	int	size;

	size = ft_strlen(string);
	s = (char *)calloc(size + 1, sizeof(char));
	s = ft_memcpy((void*)s, (void*)s, size);
	ft_putstr(s);
	free(s);
	return (0);
}
```

### Included Functions
#### Part 1 - Libc functions

|name					|prototype																	|
|---					|---																		|
|	ft_atoi				|	int atoi(const char *str);												|
|	ft_bzero			|	void bzero(void *s, size_t n);											|
|	ft_calloc			|	void *calloc(size_t count, size_t size);								|
|	ft_isalnum			|	int isalnum(int c);														|
|	ft_isalpha			|	int ft_isalpha(int c);													|
|	ft_isascii			|	int isascii(int c);														|
|	ft_isdigit			|	int ft_isdigit(int c);													|
|	ft_isprint			|	int ft_isprint(int c);													|
|	ft_memccpy			|	void *ft_memcpy(void *dst, const void *src, size_t n);					|
|	ft_memchr			|	void *ft_memchr(const void *s, int c, size_t n);						|
|	ft_memcmp			|	int ft_memcmp(const void *s1, const void *s2, size_t n);				|
|	ft_memcpy			|	void *ft_memccpy(void *dst, const void *src, int c, size_t n);			|
|	ft_memmove			|	void *ft_memmove(void *dst, const void *src, size_t len);				|
|	ft_memset			|	void *ft_memset(void *b, int c, size_t len);							|
|	ft_strchr			|	char *ft_strchr(const char *s, int c);									|
|	ft_strdup			|	char *ft_strdup(const char *s1);										|
|	ft_strlcat			|	size_t ft_strlcat(char *dst, const char *src, size_t dstsize);			|
|	ft_strlcpy			|	size_t ft_strlcpy(char *dst, const char *src, size_t dstsize);			|
|	ft_strlen			|	size_t ft_strlen(const char *s);										|
|	ft_strncmp			|	int ft_strncmp(const char *s1, const char *s2, size_t n);				|
|	ft_strnstr			|	char *ft_strnstr(const char *haystack, const char *needle, size_t len);	|
|	ft_strrchr			|	char *ft_strrchr(const char *s, int c);									|
|	ft_tolower			|	int ft_tolower(int c);													|
|	ft_toupper			|	int ft_toupper(int c);													|

#### Part 2 - Additional Functions
|name					|prototype																	|
|---					|---																		|
|	ft_itoa				|	char *ft_itoa(int n);													|
|	ft_putchar_fd		|	void ft_putchar_fd(char c, int fd);										|
|	ft_putendl_fd		|	void ft_putendl_fd(char *s, int fd);									|
|	ft_putnbr_fd		|	void ft_putnbr_fd(int n, int fd);										|
|	ft_putstr_fd		|	void ft_putstr_fd(char *s, int fd);										|
|	ft_split			|	char **ft_split(char const *s, char c);									|
|	ft_strjoin			|	char *ft_strjoin(char const *s1, char const *s2);						|
|	ft_strmapi			|	char *ft_strmapi(char const *s, char (*f)(unsigned int, char));			|
|	ft_strtrim			|	char *ft_strtrim(char const *s1, char const *set);						|
|	ft_substr			|	char *ft_substr(char const *s, unsigned int start, size_t len);			|

#### Bonus Part
|name					|prototype																	|
|---					|---																		|
|ft_lstadd_back		|	void ft_lstadd_back(t_list **lst, t_list *new);								|
|ft_lstadd_front	|	void ft_lstadd_front(t_list **lst, t_list *new);							|
|ft_lstclear		|	void ft_lstclear(t_list **lst, void (*del)(void *));						|
|ft_lstdelone		|	void ft_lstdelone(t_list *lst, void (*del)(void *));						|
|ft_lstiter			|	void ft_lstiter(t_list *lst, void (*f)(void *));							|
|ft_lstlast			|	t_list *ft_lstlast(t_list *lst);											|
|ft_lstmap			|	t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *));	|
|ft_lstnew			|	t_list *ft_lstnew(void *content);											|
|ft_lstsize			|	int ft_lstsize(t_list *lst);												|
|ft_isblank			|	int		ft_isblank(int c);													|
|ft_islower			|	int		ft_islower(int c);													|
|ft_isspace			|	int		ft_isspace(int c);													|
|ft_isupper			|	int		ft_isupper(int c);													|
|ft_putchar			|	void	ft_putchar(char c);													|
|ft_putendl			|	void	ft_putendl(char *s);												|
|ft_putnbr			|	void	ft_putnbr(int nb);													|
|ft_putstr			|	void	ft_putstr(char *str);												|