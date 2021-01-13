### Module
#### interface vs type
| interface   | type
|--------------|-------|
| are restricted to an object type | alias for all kind of types including primitives (undefined, null, boolean, string and number), union, and intersection types | 
| Type aliases cannot be extended or implemented   |   | 
```ts
interface DudeInterface {
  name: string;
  age: number;
}

const pawel: DudeInterface = {
  name: "Pawel",
  age: 31
};

type DudeType = {
  name: string,
  age: number
};

const pawel: DudeType = {
  name: "Pawel",
  age: 31
};

type info = string | { name: string };
```
