# C语言在线编译环境帮助文档
开发环境处于测试阶段，语言标准和标准库支持还不完整，请您谅解。  

## 小提示

*   网页可以保存到自己的电脑，不需要每次都从链接打开
*   开发环境会经常更新，请不定期从链接打开网页更新环境，然后保存到本地使用
*   按Ctrl+C可以终止程序运行

## 当前已知问题

*   开启中文输入法时会很难在下面的模拟终端里打字，切换成英文就好了
*   如果您想用printf "%p"输出指针的数值，请把后面对应的参数转换成void\*，如、printf("%p %p", (void\*)&a, (void\*)"hello")否侧输出可能会出错。
*   如果您在运行程序的时候遇到了诸如Internal xxx error的字样，请不要慌张，这是我们出了问题， 问题会自动汇报给我们，我们会尽快修复。

## 支持的头文件和库函数

### stdlib.h

*   void exit(int);
*   int rand();
*   void srand();
*   int abs(int);
*   long labs(long);
*   long long llabs(long long);

### time.h

*   time\_t
*   time\_t time(time\_t\*)

### stdio.h

*   int fprintf (FILE \* stream, const char \* format, ...);
*   int printf (const char \* format, ...);
*   int scanf (const char \* format, ...);
*   int getchar();
*   char\* gets(char\*)
*   char\* fgets(char\* str, int count, FILE\* stream);

### assert.h

*   void assert(int)

### stddef.h

*   size\_t
*   ptrdiff\_t
*   NULL

### ctype.h

*   int isalnum(int);
*   int isalpha(int);
*   int isblank(int);
*   int iscntrl(int);
*   int isdigit(int);
*   int isgraph(int);
*   int islower(int);
*   int isprint(int);
*   int ispunct(int);
*   int isspace(int);
*   int isupper(int);
*   int isxdigit(int);
*   int tolower(int);
*   int toupper(int);

### math.h

*   double acosh(double);
*   double asin(double);
*   double asinh(double);
*   double atan(double);
*   double atan2(double, double);
*   double atanh(double);
*   double cbrt(double);
*   double ceil(double);
*   double cos(double);
*   double cosh(double);
*   double exp(double);
*   double expm1(double);
*   double fabs(double);
*   double floor(double);
*   double fmax(double, double);
*   double fmin(double, double);
*   double fmod(double, double);
*   double hypot(double, double);
*   double log(double);
*   double log10(double);
*   double log1p(double);
*   double log2(double);
*   double logb(double);
*   double pow(double, double);
*   double round(double);
*   double sin(double);
*   double sinh(double);
*   double sqrt(double);
*   double tan(double);
*   double tanh(double);
*   double trunc(double);

### string.h

*   int strlen(const char\*);
*   int strcmp(const char\* lhs, const char\* rhs);
*   int strncmp(const char\* lhs, const char\* rhs, size\_t count);

### limits.h

*   CHAR\_BIT
*   SCHAR\_MIN
*   SCHAR\_MAX
*   UCHAR\_MAX
*   CHAR\_MIN
*   CHAR\_MAX
*   MB\_LEN\_MAX
*   SHRT\_MIN
*   SHRT\_MAX
*   USHRT\_MAX
*   INT\_MIN
*   INT\_MAX
*   UINT\_MAX
*   LONG\_MIN
*   LONG\_MAX
*   ULONG\_MAX
*   LLONG\_MIN
*   LLONG\_MAX
*   ULLONG\_MAX

### stdarg.h

*   va\_list
*   va\_start(ap, arg)
*   va\_end(ap)
*   va\_arg(ap, type)
*   va\_copy(ap, ap)
