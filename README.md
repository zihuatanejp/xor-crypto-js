# xor-cypto-js
A xor-crypto implements version of javascript, support nodejs &amp; broswer.  
params both support any utf8-character-string.

## Install
```bash
npm i xor-cypto-js 
```

## Example use

```javascript
var xor = require('xor-cypto-js');

var plain_text = '窝爱你，sigou';  // 待加密的原文

var cipher_key = 'dd哦en'; // 用来加密的密钥key

var cipher_text = xor.enc_xor(plain_text); //得到密文

console.log('cipher_text: ' + cipher_text); // ''

var plain_is = xor.dec_xor(cipher_text, cipher_key);

console.log('plain_is':); // ''
```