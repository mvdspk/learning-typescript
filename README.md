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
