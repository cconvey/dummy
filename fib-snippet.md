``` C
#include <stdio.h>
#include <stdlib.h>

int fib(int n) {
    if (n < 1) {
        return 0;
    }
    else if (n < 3) {
        return n;
    }
    return fib(n-1) + fib(n-2);
}

int main(int argc, const char* argv[]) {
    int n = atoi(argv[1]);
    printf("fib(%d) = %d\n", n, fib(n));
    return 0;
}
```

