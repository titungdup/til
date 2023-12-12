`string` is a primitive type in Typescript whereas `String` is a wrapper object for strings and should virtually never be used as types.

```typescript
/* WRONG */
function reverse(s: String): String

/* OK */
function reverse(s: string): string
```

The difference between primitives and objects is that primitives are immutable and don't have methods.
The reason we can use methods with string is because Javascript has a `String` object that have methods. So, Javascript wraps the `string` to `String` object, calls the method and then throws the object away.

TypeScript models this distinction by having distinct types for the primitives and their object wrappers:

- string and String
- number and Number
- boolean and Boolean
- symbol and Symbol
- bigint and BigInt

In Typescript, you will see `string` is assignable to `String`, but `String` is not assignable to `string`. So, Don’t ever use the types `Number`, `String`, `Boolean`, `Symbol`, or `Object`.

Source: [TSDoc](https://www.typescriptlang.org/docs/handbook/declaration-files/do-s-and-don-ts.html), [StackOverflow](https://stackoverflow.com/questions/14727044/what-is-the-difference-between-types-string-and-string), [TypeHero](https://typehero.dev/challenge/primitive-data-types)
