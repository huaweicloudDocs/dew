# 查询SSH密钥对详情<a name="dew_02_0202"></a>

## 功能介绍<a name="s1e7d7cf7c81f4ccea8873f590cb1cae5"></a>

根据SSH密钥对的名称查询指定SSH密钥对。

## URI<a name="s9989a8d799ea410aa4549ae1057dabdf"></a>

-   URI格式

    GET /v2/\{project\_id\}/os-keypairs/\{keypair\_name\}

-   参数说明

    <a name="zh-cn_topic_0020212677_table51931981"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020212677_row62634432"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020212677_p40224245"><a name="zh-cn_topic_0020212677_p40224245"></a><a name="zh-cn_topic_0020212677_p40224245"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020212677_p36938398"><a name="zh-cn_topic_0020212677_p36938398"></a><a name="zh-cn_topic_0020212677_p36938398"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020212677_p39220260"><a name="zh-cn_topic_0020212677_p39220260"></a><a name="zh-cn_topic_0020212677_p39220260"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020212677_row22724462"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p28742116"><a name="zh-cn_topic_0020212677_p28742116"></a><a name="zh-cn_topic_0020212677_p28742116"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p46410096"><a name="zh-cn_topic_0020212677_p46410096"></a><a name="zh-cn_topic_0020212677_p46410096"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p1121399"><a name="zh-cn_topic_0020212677_p1121399"></a><a name="zh-cn_topic_0020212677_p1121399"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020212677_row10092597"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p12194051"><a name="zh-cn_topic_0020212677_p12194051"></a><a name="zh-cn_topic_0020212677_p12194051"></a>keypair_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p48194049"><a name="zh-cn_topic_0020212677_p48194049"></a><a name="zh-cn_topic_0020212677_p48194049"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p11403863"><a name="zh-cn_topic_0020212677_p11403863"></a><a name="zh-cn_topic_0020212677_p11403863"></a>SSH密钥对的名称信息。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="sb0d89416d8514c06a864a9b918fede75"></a>

请求参数

无

## 响应消息<a name="s5d60eac200ac49f0a14a92ce782e3404"></a>

响应参数 

<a name="zh-cn_topic_0020212677_table49096623"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212677_row20553506"><th class="cellrowborder" valign="top" width="23.057694230576942%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020212677_p54221300"><a name="zh-cn_topic_0020212677_p54221300"></a><a name="zh-cn_topic_0020212677_p54221300"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="30.76692330766923%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020212677_p1866374"><a name="zh-cn_topic_0020212677_p1866374"></a><a name="zh-cn_topic_0020212677_p1866374"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="46.17538246175382%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020212677_p16958614"><a name="zh-cn_topic_0020212677_p16958614"></a><a name="zh-cn_topic_0020212677_p16958614"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212677_row31470474"><td class="cellrowborder" valign="top" width="23.057694230576942%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p66080459"><a name="zh-cn_topic_0020212677_p66080459"></a><a name="zh-cn_topic_0020212677_p66080459"></a>keypair</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p30630481"><a name="zh-cn_topic_0020212677_p30630481"></a><a name="zh-cn_topic_0020212677_p30630481"></a>字典数据结构[1]</p>
</td>
<td class="cellrowborder" valign="top" width="46.17538246175382%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p49478440"><a name="zh-cn_topic_0020212677_p49478440"></a><a name="zh-cn_topic_0020212677_p49478440"></a>SSH密钥对信息。</p>
</td>
</tr>
</tbody>
</table>

\[1\] keypairs字段数据结构说明

<a name="zh-cn_topic_0020212677_table32323009"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212677_row56122340"><th class="cellrowborder" valign="top" width="23.119999999999997%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020212677_p49615719"><a name="zh-cn_topic_0020212677_p49615719"></a><a name="zh-cn_topic_0020212677_p49615719"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="30.64%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020212677_p50743509"><a name="zh-cn_topic_0020212677_p50743509"></a><a name="zh-cn_topic_0020212677_p50743509"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="46.239999999999995%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020212677_p16583569"><a name="zh-cn_topic_0020212677_p16583569"></a><a name="zh-cn_topic_0020212677_p16583569"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212677_row1091845"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p21330650"><a name="zh-cn_topic_0020212677_p21330650"></a><a name="zh-cn_topic_0020212677_p21330650"></a>public_key</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p28418246"><a name="zh-cn_topic_0020212677_p28418246"></a><a name="zh-cn_topic_0020212677_p28418246"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p47371280"><a name="zh-cn_topic_0020212677_p47371280"></a><a name="zh-cn_topic_0020212677_p47371280"></a>SSH密钥对对应的publicKey信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row23688339"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p39707298"><a name="zh-cn_topic_0020212677_p39707298"></a><a name="zh-cn_topic_0020212677_p39707298"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p2977371"><a name="zh-cn_topic_0020212677_p2977371"></a><a name="zh-cn_topic_0020212677_p2977371"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p23019892"><a name="zh-cn_topic_0020212677_p23019892"></a><a name="zh-cn_topic_0020212677_p23019892"></a>SSH密钥对的名称。</p>
</td>
</tr>
<tr id="r3c4e33fabc9540c68209359a32a980a2"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="aa970d73ce0284adf939a2aa27641ee7c"><a name="aa970d73ce0284adf939a2aa27641ee7c"></a><a name="aa970d73ce0284adf939a2aa27641ee7c"></a>fingerprint</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="ac7b8a303cc3844d984af9934f64f884f"><a name="ac7b8a303cc3844d984af9934f64f884f"></a><a name="ac7b8a303cc3844d984af9934f64f884f"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="a64be21efe04340d48300e885affd4470"><a name="a64be21efe04340d48300e885affd4470"></a><a name="a64be21efe04340d48300e885affd4470"></a>SSH密钥对对应的指纹信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row5852437"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p4285383"><a name="zh-cn_topic_0020212677_p4285383"></a><a name="zh-cn_topic_0020212677_p4285383"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p64894876"><a name="zh-cn_topic_0020212677_p64894876"></a><a name="zh-cn_topic_0020212677_p64894876"></a>String:DateTime</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p63724816"><a name="zh-cn_topic_0020212677_p63724816"></a><a name="zh-cn_topic_0020212677_p63724816"></a>SSH密钥对创建的时间。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row36652435"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p16057296"><a name="zh-cn_topic_0020212677_p16057296"></a><a name="zh-cn_topic_0020212677_p16057296"></a>deleted</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p58113810"><a name="zh-cn_topic_0020212677_p58113810"></a><a name="zh-cn_topic_0020212677_p58113810"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p19274797"><a name="zh-cn_topic_0020212677_p19274797"></a><a name="zh-cn_topic_0020212677_p19274797"></a>SSH密钥对删除的标记。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row39255446"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p25574597"><a name="zh-cn_topic_0020212677_p25574597"></a><a name="zh-cn_topic_0020212677_p25574597"></a>deleted_at</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p22776773"><a name="zh-cn_topic_0020212677_p22776773"></a><a name="zh-cn_topic_0020212677_p22776773"></a>String:DateTime</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p28378258"><a name="zh-cn_topic_0020212677_p28378258"></a><a name="zh-cn_topic_0020212677_p28378258"></a>SSH密钥对删除的时间。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row54077734"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p18220335"><a name="zh-cn_topic_0020212677_p18220335"></a><a name="zh-cn_topic_0020212677_p18220335"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p22737212"><a name="zh-cn_topic_0020212677_p22737212"></a><a name="zh-cn_topic_0020212677_p22737212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p66647176"><a name="zh-cn_topic_0020212677_p66647176"></a><a name="zh-cn_topic_0020212677_p66647176"></a>SSH密钥对的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row62953674"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p66082838"><a name="zh-cn_topic_0020212677_p66082838"></a><a name="zh-cn_topic_0020212677_p66082838"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p46241663"><a name="zh-cn_topic_0020212677_p46241663"></a><a name="zh-cn_topic_0020212677_p46241663"></a>String:DateTime</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p21523158"><a name="zh-cn_topic_0020212677_p21523158"></a><a name="zh-cn_topic_0020212677_p21523158"></a>SSH密钥对的更新时间。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row59490699"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212677_p54017281"><a name="zh-cn_topic_0020212677_p54017281"></a><a name="zh-cn_topic_0020212677_p54017281"></a>user_id</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212677_p5473047"><a name="zh-cn_topic_0020212677_p5473047"></a><a name="zh-cn_topic_0020212677_p5473047"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212677_p30428869"><a name="zh-cn_topic_0020212677_p30428869"></a><a name="zh-cn_topic_0020212677_p30428869"></a>SSH密钥对所属的用户信息。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section83012587215"></a>

如下以查询SSH密钥对详情为例。

响应样例

```
{
    "keypair": {
        "created_at": "2014-05-07T12:06:13.681238",
        "deleted": false,
        "deleted_at": null,
        "fingerprint": "9d:00:f4:d7:26:6e:52:06:4c:c1:d3:1d:fd:06:66:01",
        "id": 1,
        "name": "keypair-3582d8b7-e588-4aad-b7f7-f4e76f0e4314",
        "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDYJrTVpcMwFqQy/oMvtUSRofZdSRHEwrsX8AYkRvn2ZnCXM+b6+GZ2NQuuWj+ocznlnwiGFQDsL/yeE+/kurqcPJFKKp60mToXIMyzioFxW88fJtwEWawHKAclbHWpR1t4fQ4DS+/sIbX/Yd9btlVQ2tpQjodGDbM9Tr9/+/3i6rcR+EoLqmbgCgAiGiVV6VbM2Zx79yUwd+GnQejHX8BlYZoOjCnt3NREsITcmWE9FVFy6TnLmahs3FkEO/QGgWGkaohAJlsgaVvSWGgDn2AujKYwyDokK3dXyeX3m2Vmc3ejiqPa/C4nRrCOlko5nSgV/9IXRx1ERImsqZnE9usB Generated-by-Nova\n",
        "updated_at": null,
        "user_id": "fake"
    }
}
```

## 返回值<a name="seae59e871b2642bead4841fae23e5c85"></a>

请参考[状态码](状态码.md)。

