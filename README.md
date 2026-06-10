# Merge Sorted Arrays TypeScript

This project implements this function:

```ts
merge(collection_1: number[], collection_2: number[], collection_3: number[]): number[]
```

It returns one sorted array in ascending order.

## Requirement

- `collection_1` is already sorted ascending: min to max
- `collection_2` is already sorted descending: max to min
- `collection_3` is already sorted ascending: min to max
- Do **not** use any sort function such as `Array.prototype.sort()`

## Approach

The implementation uses three pointers:

- `i` starts at the beginning of `collection_1`
- `j` starts at the end of `collection_2`, because the end contains the smallest value
- `k` starts at the beginning of `collection_3`

At each step, the function selects the smallest current value and pushes it into the result.

Time complexity: `O(n1 + n2 + n3)`

Space complexity: `O(n1 + n2 + n3)` for the returned array

## Setup

```bash
npm install
```

## Run example code

```bash
npm start
```

## Run unit tests

```bash
npm test
```

## Build project

```bash
npm run build
```

## Project structure

```text
merge-sorted-arrays-ts/
├── src/
│   ├── index.ts
│   └── merge.ts
├── tests/
│   └── merge.test.ts
├── jest.config.ts
├── package.json
├── tsconfig.json
└── README.md
```
