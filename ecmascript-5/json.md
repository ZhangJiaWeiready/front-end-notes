JSON 全称为 JavaScript Object Notation，译为 JavaScript 对象表示法。是一种轻量级的数据交换格式。






JSON 存储数据的类型可以是字符串（string）、数值(number)、true、false、 null、对象（object）或者数组（array）。这些结构可以嵌套。

## JavaScript 中的 JSON
var jsonTxt = ' { 
```

- 值的有序列表。
var jsonTxt =' [ "Tom", "Mary", "John" ] ';
```

> **值得注意的是:** 字符串必须用双引号括起来。

| 方法名 | 描述 |
| --- | --- |
| JSON.parse() | 解析JSON字符串，可以选择改变前面解析后的值及其属性，然后返回解析的值。|
| JSON.stringify() | 返回指定值的 JSON 字符串，可以自定义只包含某些特定的属性或替换属性值。|

> **值得注意的是:** IE 8 版本之前（包含 8 版本）并不支持 JSON 对象。必须下载 json2.js 或 json3.js 工具解决此问题。

## JSON 转换为 JavaScript

- 利用 JavaScript 中的 eval() 函数。该函数用于执行以字符串（String）形式出现的JavaScript代码。
var jsonTxt = ' { "x": 60, "y": 30 } ';
```

> **值得注意的是:**
> 
> - 根据 eval() 的严格语法要求，其接收的参数只能是 string 类型，而不能是 String 类型！
> - 使用 eval() 将 JSON 字符串解析为 JavaScript 对象时，若不添加左右的小括号，会抛出 SyntaxError。
var jsonTxt = ' { "x": 60, "y": 30 } ';
```

## JavaScript 转换为 JSON

利用 JavaScript 中 JSON 对象的 stringify() 方法将 JavaScript 转换为 JSON。
var jsObj = { 'x': 60, 'y': 30 } ;
```