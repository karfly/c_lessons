# 01_pointers: task
#### 1) Declare 2 int pointers.
Hint: to declare 2 int's you can use:
```c
int num1 = 1, num2 = 2;
```
#### 2) What this code will print (do not compile, use your head)?
```c
int num1 = 42;
int ptr = &num1;

printf("%d\n", *ptr);
```

#### 3) What this code will print (compile it, and prepare a screenshot)?
```c
int num1 = 42;
int ptr = &num1;

printf("%p\n", ptr);
```
What does "%p" mean?

#### 4) What this code will print (do not compile, use your head)?
```c
int arr[3];
arr[0] = arr[1] = arr[2] = 42;

printf("%d %d %d\n", arr[1], arr[2], arr[3]);

printf("%d\n", arr[1] == *(arr + 1));
printf("%d\n", arr[3] == *(arr + 3));

printf("%d\n", arr == &arr[0]);
printf("%d\n", arr[2] == *(&arr[0] + 2));
printf("%d\n", arr[1] == (&arr[0])[1]);

```

#### 5) Write code for allocating matrix n*m (n - row, m - column)
Hint: remember, that matrix is an array of arrays. To allocate array for n elements, you can use:
```c
int * arr = (int *)calloc(n, sizeof(int))
```

#### 6) Write program, that allocates 2 squre matricies size of n*n (n is given from keyboard), fills them from keyboard and then multiply them (whatch this video to understand matrix multiplication https://www.youtube.com/watch?v=xMNOI8YRQIo or see Wiki).