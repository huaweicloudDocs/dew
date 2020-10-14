# 解绑SSH密钥对<a name="DisassociateKeypair"></a>

## 功能介绍

给指定的虚拟机解除绑定SSH密钥对并恢复SSH密码登录。

## 调试

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=KPS&api=DisassociateKeypair)中调试该接口。

## URI

POST /v3/\{project\_id\}/keypairs/disassociate

**表 1**  路径参数

<table><thead align="left"><tr><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p>描述</p>
</th>
</tr>
</thead>
<tbody><tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p>项目ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p>描述</p>
</th>
</tr>
</thead>
<tbody><tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p>用户Token。 通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p>描述</p>
</th>
</tr>
</thead>
<tbody><tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p>server</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p><a href="#request_DisassociateEcsServerInfo">DisassociateEcsServerInfo</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p>需要绑定密钥对的虚拟机信息。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  DisassociateEcsServerInfo

<a name="request_DisassociateEcsServerInfo"></a>
<table><thead align="left"><tr><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p>描述</p>
</th>
</tr>
</thead>
<tbody><tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p>id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p>需要绑定(替换或重置)SSH密钥对的虚拟机id。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p>auth</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p><a href="#request_Auth">Auth</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p>可选字段，鉴权认证类型。替换时需要该参数，重置时不需要该参数。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  Auth

<a name="request_Auth"></a>
<table><thead align="left"><tr><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p>描述</p>
</th>
</tr>
</thead>
<tbody><tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p>type</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p>取值为枚举类型。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p>key</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><ul><li><p>type为枚举值password时，key表示密码；</p>
</li><li><p>type为枚举值keypair时，key表示私钥；</p>
</li></ul>
</td>
</tr>
</tbody>
</table>

## 响应参数

**状态码为 202 时: **

**表 6**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p>描述</p>
</th>
</tr>
</thead>
<tbody><tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p>task_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p>任务下发成功返回的ID。</p>
</td>
</tr>
</tbody>
</table>

**状态码为 400 时: **

**表 7**  响应Body参数

<a name="responseParameter_1"></a>
<table><thead align="left"><tr><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p>描述</p>
</th>
</tr>
</thead>
<tbody><tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p>错误码。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p>错误描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例

-   ```
{
  "server" : {
    "id" : "d76baba7-ef09-40a2-87ff-3eafec0696e7",
    "authentication" : {
      "type" : "keypair",
      "key" : "-----BEGINRSAPRIVATEKEY-----\nM..."
    }
  }
}
```

-   ```
{
  "server" : {
    "id" : "d76baba7-ef09-40a2-87ff-3eafec0696e7"
  }
}
```


## 响应示例

**状态码为 202 时: **

OK。

```
{
  "task_id" : "aee8d2fe-5484-4753-9177-5a38dc15546c"
}
```

**状态码为 400 时: **

Error response。

```
{
  "error_code" : "KPS.XXX",
  "error_msg" : "XXX"
}
```

## 状态码

<a name="table36069"></a>
<table><thead align="left"><tr><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p>状态码 </p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p>描述</p>
</th>
</tr>
</thead>
<tbody><tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p>202</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p>OK。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p>Error response。</p>
</td>
</tr>
</tbody>
</table>

## 错误码

请参见[错误码](错误码.md)。

