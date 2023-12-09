**Union**

Use/Combine multiple data types into one. It enables a variable to hold values of different types. It is denoted by symbol `|`

Example:

```typescript
let x: string | number
```

**Intersection**

Combine multiple types into a new type that contains all properties and methods from each individual type. It is denoted by `&` symbol.

Example:

```typescript
// Define two types
type Car = {
  brand: string
  year: number
}

type Features = {
  automatic: boolean
  airbags: boolean
}

// Intersection type combining Car and Features
type CarWithFeatures = Car & Features

// Creating an object that satisfies the CarWithFeatures type
let myCar: CarWithFeatures = {
  brand: 'Tesla',
  year: 2022,
  automatic: true,
  airbags: true,
}
```
