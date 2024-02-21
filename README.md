# learning-typescript

inter operable with javascript

```
npm install -g typescript
```

```ts
tsc -v
```

```
Version 5.3.3
```

## Data Types
```ts
let id:number = 5;
```
gets converted to js file eventhough there is error

converts `let` in TYpeScript to `var` in Javascript ES5

[more details](https://github.com/mvdspk/learning-typescript/blob/main/config-file.md#target-property)

need config file to map other requirements


```js
var id = 5;
id = "sdsd";
```
```
typescript sivakanta.eranki$ tsc index.ts
index.ts:3:1 - error TS2322: Type 'string' is not assignable to type 'number'.

3 id= "sdsd"
  ~~


Found 1 error in index.ts:3
```

### Any

```ts
let x: any = 5;

x = "hi" // no typecast error
```

## ARrays

```ts
let numbers: number [] = [1,2,3,4,5];
```

## Union

variabe can hold either of 2 types

```ts
let id: string | number = 2
```

## Tuple

```ts
let person:[number, string, boolean] = [1, 'Pavan', true]
```
## Functions

Parameters by default have types
to manage this rule see [Config > No Implicit ANy](https://github.com/mvdspk/learning-typescript/blob/main/config-file.md#noimplicitany)


FUnction with parameters and return value
```ts
// parameter x is a number,
// function returns number
function addNum(x: number, y: number): number{
return x+ y;
}

```

Function with union parameter and void return value

```ts
function logMessage(message: number | string): void {
 console.log(message);
}
```


## Type ( similar to Class in Java)
```ts

// define class User
type User = {
id: number
name: string
```
```ts
// create object

let user: User = {
id: 1,
 name: 'pavan'

 ```

### Type with Primitive
can be used with primitives

todo code snippet

### Type with Union


```ts
type Point = number | string

let p1 : Point = 1;
```


## Interface
- cannot be used with Unions
- cannot be used with primitives



