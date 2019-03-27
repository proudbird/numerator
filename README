
# numerator [![Build Status](http://github.com/proudbird/numerator)] #

A simple script, that increments serial numbers, containing non-digit symbols

## Quickstart - CommonJS (Recommended)

```shell
npm install numerator
```

Then make reference inside yor module...

```javascript
const numerator = require('numerator');

// ... start numeration from begining with given template
numerator.next('IN/2019/000'); // ⇨ 'IN/2019/001'

// ... or get next of the given number
numerator.next('IN/2019/056'); // ⇨ 'IN/2019/057'

```

## API

### Version 1

```javascript
const numerator = require('numerator');

// Incantations
next(number);
```

Generate and return next number based on given number.

* `number` - (String | Number) A number, that must be icremented

Returns `number`

Note: The <node> id is generated guaranteed to stay constant for the lifetime of the current JS runtime. (Future versions of this module may use persistent storage mechanisms to extend this guarantee.)

Example: Generate string UUID with fully-specified options

```javascript
const v1options = {
  node: [0x01, 0x23, 0x45, 0x67, 0x89, 0xab],
  clockseq: 0x1234,
  msecs: new Date('2011-11-01').getTime(),
  nsecs: 5678
};
uuidv1(v1options); // ⇨ '710b962e-041c-11e1-9234-0123456789ab'

```
## Testing

```shell
npm test
```