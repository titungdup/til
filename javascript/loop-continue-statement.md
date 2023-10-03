You can skip the current iteration of the loop by using `continue` statement and it continues execution of the loop with the next iteration.

Eg:

```Javascript
for (let i = 1; i <= 5; i++) {
    // condition to continue
    if (i == 3) {
        continue;
    }

    console.log(i); // 1 2 4 5
}
```

When used inside a nested loop, it skips the current iteration of the inner loop.
