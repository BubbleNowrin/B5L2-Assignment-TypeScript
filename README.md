# TypeScript Concepts

This document covers some important TypeScript concepts.

## 1. Differences between Interfaces and Types in TypeScript

- `interface` is mainly for objects and can be extended.
- `type` is more flexible (can do unions, primitives, etc.).

## 2. Use of `keyof` in TypeScript (with example)

The `keyof` keyword gets the keys of a type as a union of strings.

```ts
type Person = { name: string; age: number };
type PersonKeys = keyof Person; // "name" | "age"
```

## 3. Difference between `any`, `unknown`, and `never`

- `any`: turns off type checking.Need to use carefully.
- `unknown`: must need to check the type before using it.
- `never`: used when something should never happen (like a function that always throws).

## 4. What is type inference and why it helps

- TypeScript guesses the type for us.
- It saves time and catches mistakes early.

```ts
let name = "Alice"; // guess that it's a string
```
