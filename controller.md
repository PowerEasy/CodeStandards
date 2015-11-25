
## Action

Action的返回类型均为`ActionResult`， 返回正确的ActionResult可以让客户端正确识别MINE类型，特别在使用jQuery.ajax请求服务器端数据时，可以正确的得知数据类型。

bad code
```cs
public string GetMenuNodes(string keyValue, int moldId, int? nodeId)
{
}
```

good code

```cs
public ActionResult GetMenuNodes(string keyValue, int moldId, int? nodeId)
{
}
```
