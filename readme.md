# simple-gacha
A very simple gacha function that picks an element based off a lootTable

## Example
```javascript
const gacha = require("simple-gacha");

const lootTable = [
    {
        "name" : "Golden Knife",
        "weight" : 10
    },
    {
        "name" : "Diamond Pickaxe",
        "weight" : 5
    },
    {
        "name" : "Invisibility Cap",
        "weight" : 2
    }
]

const { pick } = gacha.simple(lootTable);
console.log(pick);
```
Since `Golden Knife` has the biggest weight, there's a higher chance that it will return Golden Knife.
```json
{
    "name" : "Golden Knife",
    "weight" : 10
}
```

## License
MIT License

Copyright (c) 2020 Regan Iwadha

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.