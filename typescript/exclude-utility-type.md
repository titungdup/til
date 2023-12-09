`Exclude utility type` creates a new type by removing certain members from a union type.

Syntax:

`Exclude<UnionType, ExcludedMembers>`

Behind the scene, it simply performs: `T extends U ? never : T;`

Example:

```typescript
type T0 = Exclude<'a' | 'b' | 'c', 'a'> // type T0 = 'b' | 'c'

// Using extends
type T1<T, U> = T extends U ? never : T
type T2 = T1<'a' | 'b' | 'c', 'a'> // type T2 = 'b' | 'c'
```
