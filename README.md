# xor-crypto-js
A xor-crypto implements version of javascript, support nodejs &amp; broswer.  
params both support any utf8-character-string.

## Install
```bash
npm i xor-crypto-js 
```

## Example use

```javascript
// In NodeJs
var xor = require('xor-cypto-js');
// In broswer
// link with script tag in html: <script type="text/javascript" src="your-path-to/xor-crypto-js/index.js" ></script> 
// then:
var xor = window.xor;
// In es6:
import xor from 'xor-cypto-js'   // now, you should have babel support first.


var plain_text = '窝爱你，sigou';  // 待加密的原文

var cipher_key = 'dd哦en'; // 用来加密的密钥key

var cipher_text = xor.enc_xor(plain_text, cipher_key); //得到密文

console.log('cipher_text: ' + cipher_text); // '01etbgj77fig93ki1r6801703dq0ji3ri9hig0ig0hgqi0ih0iq'

var plain_is = xor.dec_xor(cipher_text, cipher_key);

console.log('plain_is:',plain_is); // '窝爱你，sigou'

```