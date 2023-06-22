- The Global Object
  - Value Properties of the Global Object
    - `globalThis`
    - `Infinity`
    - `NaN`
    - `undefined`
  - Function Properties of the Global Object
    - `eval(x)`
    - `isFinite(number)`
      ```js
      let a = 1
      let result = isFinite(a) // true
      ```
    - `isNaN(value)`
      ```js
      let a = 'JS'
      let result = isNaN(a) // true
      ```
    - `parseFloat(string)`
      ```js
      let a = '12.74 TFLOPS'
      let result = parseFloat(a) // 12.74

      let b = 'ES13'
      let result = parseFloat(b) // NaN
      ```
    - `parseInt(string, radix)`
      ```js
      let a = '12.74 TFLOPS'
      let result = parseInt(a) // 12

      let b = 'ES13'
      let result = parseInt(b) // NaN

      let c = '0xFF'
      let result = parseInt(c, 16) // 255

      let d = '11'
      let result = parseInt(d, 2) // 3
      ```
- Fundamental Objects
  - Objects
    - Properties of the Object Constructor
      - `Object.assign(target, ...sources)`
        ```js
        let a = { x: 1, y: 2 }
        let b = {}
        let result = Object.assign(a, b)
