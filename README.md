# ES5file
ES5属性与方法的学习  

ES5中数组Array的方法总共有9个，
Array.prototype.indexOf  返回在该数组中第一个找到的元素位置，如果它不存在则返回-1。  
Array.prototype.lastIndexOf  
Array.prototype.every  
Array.prototype.some  
Array.prototype.forEach  forEach是用来替换for循环的  
Array.prototype.map  对数组的每个元素进行一定操作（映射）后，会返回一个新的数组，map()是处理服务器返回数据时是一个非常实用的函数。  
Array.prototype.filter  创建一个新的匹配过滤条件的数组。
Array.prototype.reduce  
Array.prototype.reduceRight  


```
arr.indexOf('1') !="-1";
arr.filter(function(item){})
arr.forEach(function(item,index){})
arr.map(function(item,index){})
arr.reduice(function(prev,next){},{})
```

数组是一组按次序排序的值，任何类型的数据，都可以放入数组。
```
var  arr = [
  {a:1},
  [1,2,3],
  function(){return true}
]
arr[0] //object {a:1}
```
多维数组
```
var a = [
  [1,2],
  [3,4]
]
a[0][1]//2
```
数组属于一种特殊的对象。typeof运算符会返回数组的类型是object。
```
typeof [1,2] //'object'

var arr = ['a', 'b', 'c'];
console.log(Object.keys(arr)) //// ["0", "1", "2"]

```

in运算符
```
var arr = [];
arr[100] = 'a';
100 in arr // true
1 in arr // false
```

```
var a = [1, 2, 3];

for (var i in a) {
  console.log(a[i]);
}
// 1
// 2
// 3


var colors = ['red', 'green', 'blue'];
colors.forEach(function (color) {
  console.log(color);
});
```

