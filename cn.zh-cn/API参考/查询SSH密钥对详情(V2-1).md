# 查询SSH密钥对详情<a name="dew_02_0209"></a>

## 功能介绍<a name="s306004e5a98e4283a1bfcb4adc2fa508"></a>

查询SSH密钥对详细信息。

## URI<a name="sbbff16336947456f8342473caef444e2"></a>

-   URI格式

    GET /v2.1/\{project\_id\}/os-keypairs/\{keypair\_name\}

-   参数说明

    <a name="t084c49654137450aa8af2164a3c29635"></a>
    <table><thead align="left"><tr id="r58c97f5694404511b04d2fdc16bfe9b1"><th class="cellrowborder" valign="top" width="25.44%" id="mcps1.1.4.1.1"><p id="aee3be31340374327af65a4618410f235"><a name="aee3be31340374327af65a4618410f235"></a><a name="aee3be31340374327af65a4618410f235"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.93%" id="mcps1.1.4.1.2"><p id="ab3a6b43f77e84e838963da2a5dfedd2e"><a name="ab3a6b43f77e84e838963da2a5dfedd2e"></a><a name="ab3a6b43f77e84e838963da2a5dfedd2e"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.63%" id="mcps1.1.4.1.3"><p id="a22ae7dc1457a449f84d5c5cafe1cb52c"><a name="a22ae7dc1457a449f84d5c5cafe1cb52c"></a><a name="a22ae7dc1457a449f84d5c5cafe1cb52c"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r25f345fa8192463eb83292e5fbee8d7d"><td class="cellrowborder" valign="top" width="25.44%" headers="mcps1.1.4.1.1 "><p id="ac33f1671398f4429a81c5c3bfb3dc124"><a name="ac33f1671398f4429a81c5c3bfb3dc124"></a><a name="ac33f1671398f4429a81c5c3bfb3dc124"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.93%" headers="mcps1.1.4.1.2 "><p id="ae7d097da09fb43e5bd1dae10cdb80167"><a name="ae7d097da09fb43e5bd1dae10cdb80167"></a><a name="ae7d097da09fb43e5bd1dae10cdb80167"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.63%" headers="mcps1.1.4.1.3 "><p id="acf1687032c074bd0bd72b8b9b1fa31dc"><a name="acf1687032c074bd0bd72b8b9b1fa31dc"></a><a name="acf1687032c074bd0bd72b8b9b1fa31dc"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row43976585105625"><td class="cellrowborder" valign="top" width="25.44%" headers="mcps1.1.4.1.1 "><p id="p5333658105625"><a name="p5333658105625"></a><a name="p5333658105625"></a>keypair_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.93%" headers="mcps1.1.4.1.2 "><p id="p29373192105625"><a name="p29373192105625"></a><a name="p29373192105625"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.63%" headers="mcps1.1.4.1.3 "><p id="p30418362105625"><a name="p30418362105625"></a><a name="p30418362105625"></a>SSH密钥对名称。</p>
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
<tr id="row11502018145731"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="p59248279145731"><a name="p59248279145731"></a><a name="p59248279145731"></a>is_key_protection</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="p64459916145837"><a name="p64459916145837"></a><a name="p64459916145837"></a>boolean</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="p29772019145838"><a name="p29772019145838"></a><a name="p29772019145838"></a>SSH密钥对是否私钥托管与保护。</p>
</td>
</tr>
<tr id="row43203711263"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.4.1.1 "><p id="p103037192615"><a name="p103037192615"></a><a name="p103037192615"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="30.64%" headers="mcps1.1.4.1.2 "><p id="p1393742613"><a name="p1393742613"></a><a name="p1393742613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.1.4.1.3 "><p id="p13193712619"><a name="p13193712619"></a><a name="p13193712619"></a>SSH密钥对的描述信息</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section8112517104818"></a>

-   响应样例

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
            "user_id": "fake",
            "is_key_protection": true,
            "description": "keypair test"
        }
    }
    ```

    或

    ```
    {
        "error_code": "KPS.XXXX",
        "error_msg": "XXXX"
    }
    ```


## 返回值<a name="s45a1d5602b9a4b5b942549cb65e046cc"></a>

请参考[状态码](状态码.md)。

