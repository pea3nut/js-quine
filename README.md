# js-quine
The quine in js without Function.toString.

```js
!function (v) {
    console.log(v +'(`' + v.replace(new RegExp(String.fromCharCode(96),'g'), String.fromCharCode(92) + String.fromCharCode(96)) + '`);');
}(`!function (v) {
    console.log(v +'(\`' + v.replace(new RegExp(String.fromCharCode(96),'g'), String.fromCharCode(92) + String.fromCharCode(96)) + '\`);');
}`);
```
