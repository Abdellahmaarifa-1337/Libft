# Libft: My Very First Own Library

This project is a fundamental exploration into the world of C programming, requiring you to create My own C library known as "libft." The library comprises a collection of general-purpose functions, mimicking some of the standard functions found in the C library. This initiative aims to enhance My understanding of how these functions operate, encouraging you to implement and utilize them. Not only will this library serve as a valuable tool for future C assignments, but it will also deepen My grasp of low-level programming concepts.

## Implemented Functions

### Part 1 - Libc Functions

1. **ft_isalpha**

   - **Description:** Check if a character is an alphabetic character.
   - **Prototype:** `int ft_isalpha(int c);`

2. **ft_isdigit**

   - **Description:** Check if a character is a digit (0-9).
   - **Prototype:** `int ft_isdigit(int c);`

3. **ft_isalnum**

   - **Description:** Check if a character is alphanumeric.
   - **Prototype:** `int ft_isalnum(int c);`

4. **ft_isascii**

   - **Description:** Check if a character is a 7-bit ASCII character.
   - **Prototype:** `int ft_isascii(int c);`

5. **ft_isprint**

   - **Description:** Check if a character is a printable character.
   - **Prototype:** `int ft_isprint(int c);`

6. **ft_strlen**

   - **Description:** Calculate the length of a string.
   - **Prototype:** `size_t ft_strlen(const char *s);`

7. **ft_memset**

   - **Description:** Fill memory with a constant byte.
   - **Prototype:** `void *ft_memset(void *s, int c, size_t n);`

8. **ft_bzero**

   - **Description:** Set the first n bytes of the memory area pointed to by s to zero.
   - **Prototype:** `void ft_bzero(void *s, size_t n);`

9. **ft_memcpy**

   - **Description:** Copy memory area.
   - **Prototype:** `void *ft_memcpy(void *dest, const void *src, size_t n);`

10. **ft_memmove**

- **Description:** Copy memory area, handling overlapping memory regions.
- **Prototype:** `void *ft_memmove(void *dest, const void *src, size_t n);`

11. **ft_strlcpy**

- **Description:** Copy strings with source and destination size control.
- **Prototype:** `size_t ft_strlcpy(char *dest, const char *src, size_t size);`

12. **ft_strlcat**

- **Description:** Concatenate strings with source and destination size control.
- **Prototype:** `size_t ft_strlcat(char *dest, const char *src, size_t size);`

13. **ft_toupper**

- **Description:** Convert a lowercase letter to its corresponding uppercase letter.
- **Prototype:** `int ft_toupper(int c);`

14. **ft_tolower**

- **Description:** Convert an uppercase letter to its corresponding lowercase letter.
- **Prototype:** `int ft_tolower(int c);`

15. **ft_strchr**

- **Description:** Locate the first occurrence of a character in a string.
- **Prototype:** `char *ft_strchr(const char *s, int c);`

16. **ft_strrchr**

- **Description:** Locate the last occurrence of a character in a string.
- **Prototype:** `char *ft_strrchr(const char *s, int c);`

17. **ft_strncmp**

- **Description:** Compare two strings up to a specified number of characters.
- **Prototype:** `int ft_strncmp(const char *s1, const char *s2, size_t n);`

18. **ft_memchr**

- **Description:** Locate the first occurrence of a character in a memory block.
- **Prototype:** `void *ft_memchr(const void *s, int c, size_t n);`

19. **ft_memcmp**

- **Description:** Compare two memory blocks.
- **Prototype:** `int ft_memcmp(const void *s1, const void *s2, size_t n);`

20. **ft_strnstr**

- **Description:** Locate a substring in a string, but with a specified maximum length.
- **Prototype:** `char *ft_strnstr(const char *haystack, const char *needle, size_t len);`

21. **ft_atoi**

- **Description:** Convert a string to an integer.
- **Prototype:** `int ft_atoi(const char *str);`

### Part 2 - Additional Functions

1. **ft_substr**

   - **Description:** Allocate and return a substring from a given string.
   - **Prototype:** `char *ft_substr(char const *s, unsigned int start, size_t len);`

2. **ft_strjoin**

   - **Description:** Concatenate two strings into a new string.
   - **Prototype:** `char *ft_strjoin(char const *s1, char const *s2);`

3. **ft_strtrim**

   - **Description:** Allocate and return a trimmed version of a string.
   - **Prototype:** `char *ft_strtrim(char const *s1, char const *set);`

4. **ft_split**

   - **Description:** Split a string into an array of substrings based on a delimiter.
   - **Prototype:** `char **ft_split(char const *s, char c);`

5. **ft_itoa**

   - **Description:** Convert an integer to a string.
   - **Prototype:** `char *ft_itoa(int n);`

6. **ft_strmapi**

   - **Description:** Apply a function to each character of a string, creating a new string.
   - **Prototype:** `char *ft_strmapi(char const *s, char (*f)(unsigned int, char));`

7. **ft_striteri**

   - **Description:** Apply a function to each character of a string with its index as an argument.
   - **Prototype:** `void ft_striteri(char *s, void (*f)(unsigned int, char*));`

8. **ft_putchar_fd**

   - **Description:** Output a character to a specified file descriptor.
   - **Prototype:** `void ft_putchar_fd(char c, int fd);`

9. **ft_putstr_fd**

   - **Description:** Output a string to a specified file descriptor.
   - **Prototype:** `void ft_putstr_fd(char *s, int fd);`

10. **ft_putendl_fd**

- **Description:** Output a string followed by a newline to a specified file descriptor.
- **Prototype:** `void ft_putendl_fd(char *s, int fd);`

11. **ft_putnbr_fd**

- **Description:** Output an integer to a specified file descriptor.
- **Prototype:** `void ft_putnbr_fd(int n, int fd);`

## Bonus Part - Linked List Functions

To represent a node of the linked list, the following structure is used. Add its declaration to your `libft.h` file:

```c
typedef struct s_list
{
    void *content;
    struct s_list *next;
} t_list;


```

1. **ft_lstnew**

   - **Description:** Create a new node with the specified content.
   - **Prototype:** `t_list *ft_lstnew(void *content);`

2. **ft_lstadd_front**

   - **Description:** Add a new node at the beginning of a linked list.
   - **Prototype:** `void ft_lstadd_front(t_list **lst, t_list *new);`

3. **ft_lstsize**

   - **Description:** Count the number of nodes in a linked list.
   - **Prototype:** `int ft_lstsize(t_list *lst);`

4. **ft_lstlast**

   - **Description:** Retrieve the last node of a linked list.
   - **Prototype:** `t_list *ft_lstlast(t_list *lst);`

5. **ft_lstadd_back**

   - **Description:** Add a new node at the end of a linked list.
   - **Prototype:** `void ft_lstadd_back(t_list **lst, t_list *new);`

6. **ft_lstdelone**

   - **Description:** Delete a node from a linked list.
   - **Prototype:** `void ft_lstdelone(t_list *lst, void (*del)(void *));`

7. **ft_lstclear**

   - **Description:** Delete and free a linked list.
   - **Prototype:** `void ft_lstclear(t_list **lst, void (*del)(void *));`

8. **ft_lstiter**

   - **Description:** Apply a function to each node of a linked list.
   - **Prototype:** `void ft_lstiter(t_list *lst, void (*f)(void *));`

9. **ft_lstmap**
   - **Description:** Create a new list by applying a function to each node of an existing list.
   - **Prototype:** `t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *));`
