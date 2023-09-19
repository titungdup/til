`Record utility type` helps us to define the shape of objects with specific key-value pairs, making it easier to work with structured data in Typescript.

Note:

- Keys in Record must be unique.

Syntax: `Record<Keys, Type>`

Eg: (Taken from official documentation)

```Typescript
interface CatInfo {
  age: number;
  breed: string;
}

type CatName = "miffy" | "boris" | "mordred";

const cats: Record<CatName, CatInfo> = {
  miffy: { age: 10, breed: "Persian" },
  boris: { age: 5, breed: "Maine Coon" },
  mordred: { age: 16, breed: "British Shorthair" },
};
```

Eg:

```Typescript
const record:Record<number, string> = {
  1: 'first',
  2: 'second',
  //1: 'another a as key is not allowed'
  //a: 'not allowed type because its not a number'
};

console.log(`first in the record : ${record[1]}`);
```

Source: [Official Documentation](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type), [Geshan's blog post](https://geshan.com.np/blog/2022/12/typescript-record/)
