---
title: 拥抱ES6：iterator & generator & yield
date: 2017-04-08 00:01:01
tags: [ES6, JavaScript]
---

## 迭代器（iterator）
### 可迭代协议
`可迭代协议`允许JavaScript对象去定义或定制它们的迭代行为。一些内置类型都是内置的可遍历对象且拥有默认的迭代行为。比如Array、Map等。
为了变成可迭代对象，一个对象必须实现`@@interator`方法，也就是说该对象或它的原型链上必须有一个名字为`Symbol.interator`的属性。
当一个对象需要被遍历时，它的`@@interator`会被调用并且没有参数，然后返回一个用于在遍历中获得值的迭代器。
### 迭代器协议

## 生成器（generator）

### Generator
### function*
```javascript
function* name([param[, param[, ... param]]]) { statements }
```


## yield

## for...of..