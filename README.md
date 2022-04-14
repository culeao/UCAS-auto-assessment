# UCAS-auto-asessment

国科大（中国科学院大学）2019 年自动教学评估脚本。
教学评估系统需要打二十几个勾，而且还要手动输入 15 字以上的问题回答，太懒怎么办！！！

![截屏2019-12-2220.06.10.png](https://i.loli.net/2019/12/22/62IGEijWK9JVzAL.png)

![截屏2019-12-2220.18.06.png](https://i.loli.net/2019/12/22/leImQMqCvAH1wVW.png)

## 代码
- 课程评估
```javascript
var x = document.getElementsByClassName('required');
for(var i = 0; i<x.length;i++){
    if(i < 109 && i % 5 == 0){
        x[i].checked=true;
    }
}
x[110].textContent="在课堂上可以学到很多有用的东西，老师讲的很清晰，让我受益匪浅！";
x[111].textContent="课堂互动再多一点，必要的时候可以停一下，与学生互动要增多！";
x[112].textContent="每周可以花费大概4个小时，不固定，有时多有时少。";
x[113].textContent="很有兴趣，喜欢这个学科和领域，想进行更深入的了解。";
x[114].textContent="保持全勤，从未旷课、早退和迟到。回答问题挺积极。";
x[115].checked=true;
x[121].checked=true;
x[124].checked=true;
```
- 教师评估
```javascript
var x = document.getElementsByClassName('required');
for(var i = 0; i<x.length;i++){
    if(i < 105 && i % 5 == 0){
        x[i].checked=true;
    }
}
x[105].textContent="最喜欢老师上课讲各种与课堂相关的趣事，老师上课认真，思路清晰。";
x[106].textContent="课堂互动再多一点，必要的时候可以停一下，与学生互动要增多！";
```

## 使用方法

打开课程评价/教师评价的页面，点击进行评估，然后按 F12 调出 chrome 的控制台，在下方的标签选 Console，然后粘贴上面的代码按回车即可。
![截屏2019-12-2220.22.06.png](https://i.loli.net/2019/12/22/Dy2SEXNFpg358kK.png)

或者，可以将如下代码保存到书签栏，打开对应页面时，点击对应的书签，即可完成评教。

- 课程评估

```JavaScript
javascript:(function(){var x = document.getElementsByClassName('required');for(var i = 0; i<x.length;i++){if(i < 109 && i % 5 == 0){x[i].checked=true;}}x[110].textContent="在课堂上可以学到很多有用的东西，老师讲的很清晰，让我受益匪浅！";x[111].textContent="课堂互动再多一点，必要的时候可以停一下，与学生互动要增多！";x[112].textContent="每周可以花费大概4个小时，不固定，有时多有时少。";x[113].textContent="很有兴趣，喜欢这个学科和领域，想进行更深入的了解。";x[114].textContent="保持全勤，从未旷课、早退和迟到。回答问题挺积极。";x[115].checked=true;x[121].checked=true;x[124].checked=true;})();
```

- 教师评估

```javascript
javascript:(function(){var x = document.getElementsByClassName('required');for(var i = 0; i<x.length;i++){if(i < 105 && i % 5 == 0){x[i].checked=true;}}x[105].textContent="最喜欢老师上课讲各种与课堂相关的趣事，老师上课认真，思路清晰。";x[106].textContent="课堂互动再多一点，必要的时候可以停一下，与学生互动要增多！";})();
```

![教程](https://s1.ax1x.com/2022/04/15/L3QfDs.jpg)