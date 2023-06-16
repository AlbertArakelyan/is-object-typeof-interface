# is-object-typeof-interface
> A simple package which returns `true` when object is type of some specific interface or type.

This is my first package, hope it will be helpful. :heart:

## Install
Install with [npm](https://www.npmjs.com/):
```sh
$ npm install is-object-typeof-interface
```

## Usage
```ts
import isObjectTypeOfInterface from 'is-object-typeof-interface';

interface IObj1 {
  foo: string;
  bar: number;
}

interface IObj2 {
  baz: boolean;
  biz: string;
}

const obj1: any = { foo: 'str', bar: 5 };
const obj2: any = { baz: true, biz: 'str' };

const result1 = isObjectTypeOfInterface<IObj1>(obj1, 'foo');
const result2 = isObjectTypeOfInterface<IObj2>(obj2, 'baz');

console.log('Result 1: ', result1); // true
console.log('Result 2: ', result2); // true
```

## About
<details>
<summary><strong>Contributing</strong></summary>
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/ALbert2504/is-object-typeof-interface/issues/new).
</details>

<details>
<summary><strong>Motivation</strong></summary>
Receving an object from Redux store had two different types as the same component was rendering different datas, and I needed check what interface my object has to get correct property. After googling I found [this](https://stackoverflow.com/questions/14425568/interface-type-check-with-typescript) question and published this package, which will be extended in future.
</details>

<br>

### Author
**Albert Arakelyan**
* [LinkedIn Profile](https://www.linkedin.com/in/albert-arakelyan/)
* [GitHub Profile](https://github.com/ALbert2504)

