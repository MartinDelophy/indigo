react 嵌套标签

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
