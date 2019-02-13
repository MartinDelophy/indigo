---
title: "react 嵌套标签"
layout: post
date: 2019-02-13 12:10
tag: react
category: blog
author: martindelophy

---



```
const test = React.createClass({
render : function (){
return (
{this.props.children}
)
}
});

ReactDom.render(
<test>
<div></div>
</test>
)
```
