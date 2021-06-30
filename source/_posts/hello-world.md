---
title: Bye Bye World
date: 2021-06-23 12:33:03
tags: photography
---

![pic](https://wx1.sinaimg.cn/mw2000/a01bc3fbgy1gnvbldq7c6j21bb1r3tu5.jpg)


**测试中文在页面的显示效果**

*Test the display of English on the page*

测试代码在页面的显示效果
```
 <script>
	//设定图片数量，如果图片数为3，这个参数就设为2，以此类推
   bg = new Array(1);
   bg[0] = 'https://wx1.sinaimg.cn/mw2000/edbc6d1agy1gksf9xojr4j20u60u0kjt.jpg' 
   bg[1] = 'https://wx4.sinaimg.cn/mw1024/edbc6d1agy1gksf9oiusvj20ub0u0kjr.jpg'
   index = Math.floor(Math.random() * bg.length);
   	//通过打印方式创建body的起始节点
	//因为伪元素必须包含在body节点之外，将js函数放置在此才不会报错
   document.write("<BODY BACKGROUND="+bg[index]+">");
	//将所随机背景写入伪元素
   var sty=document.createElement('style');
   sty.innerText="body,.box1::before {background: url("+bg[index]+")";
   document.body.appendChild(sty);
</script>

```
