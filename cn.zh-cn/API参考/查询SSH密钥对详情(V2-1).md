# 查询SSH密钥对详情\(V2.1\)<a name="dew_02_0209"></a>

## 功能介绍<a name="s306004e5a98e4283a1bfcb4adc2fa508"></a>

查询SSH密钥对详细信息。

## URI<a name="sbbff16336947456f8342473caef444e2"></a>

-   URI格式

    GET /v2.1/\{project\_id\}/os-keypairs/\{keypair\_name\}

-   参数说明

    **表 1**  参数说明

    <a name="t084c49654137450aa8af2164a3c29635"></a>
    <table><thead align="left"><tr id="r58c97f5694404511b04d2fdc16bfe9b1"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0020212676_p1591698"><a name="zh-cn_topic_0020212676_p1591698"></a><a name="zh-cn_topic_0020212676_p1591698"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0020212676_p61818739"><a name="zh-cn_topic_0020212676_p61818739"></a><a name="zh-cn_topic_0020212676_p61818739"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p334014371274"><a name="p334014371274"></a><a name="p334014371274"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0020212676_p41262001"><a name="zh-cn_topic_0020212676_p41262001"></a><a name="zh-cn_topic_0020212676_p41262001"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r25f345fa8192463eb83292e5fbee8d7d"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="ac33f1671398f4429a81c5c3bfb3dc124"><a name="ac33f1671398f4429a81c5c3bfb3dc124"></a><a name="ac33f1671398f4429a81c5c3bfb3dc124"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="ae7d097da09fb43e5bd1dae10cdb80167"><a name="ae7d097da09fb43e5bd1dae10cdb80167"></a><a name="ae7d097da09fb43e5bd1dae10cdb80167"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p118732024172911"><a name="p118732024172911"></a><a name="p118732024172911"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="acf1687032c074bd0bd72b8b9b1fa31dc"><a name="acf1687032c074bd0bd72b8b9b1fa31dc"></a><a name="acf1687032c074bd0bd72b8b9b1fa31dc"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row43976585105625"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p5333658105625"><a name="p5333658105625"></a><a name="p5333658105625"></a>keypair_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p29373192105625"><a name="p29373192105625"></a><a name="p29373192105625"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p3873112416295"><a name="p3873112416295"></a><a name="p3873112416295"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p30418362105625"><a name="p30418362105625"></a><a name="p30418362105625"></a>SSH密钥对名称。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="sb0d89416d8514c06a864a9b918fede75"></a>

无

## 响应消息<a name="s5d60eac200ac49f0a14a92ce782e3404"></a>

**表 2**  响应参数

<a name="zh-cn_topic_0020212677_table49096623"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212677_row20553506"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p1314131083819"><a name="p1314131083819"></a><a name="p1314131083819"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p3315151016387"><a name="p3315151016387"></a><a name="p3315151016387"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p931512109388"><a name="p931512109388"></a><a name="p931512109388"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p231520102386"><a name="p231520102386"></a><a name="p231520102386"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212677_row31470474"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212677_p66080459"><a name="zh-cn_topic_0020212677_p66080459"></a><a name="zh-cn_topic_0020212677_p66080459"></a>keypair</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1697343215291"><a name="p1697343215291"></a><a name="p1697343215291"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212677_p30630481"><a name="zh-cn_topic_0020212677_p30630481"></a><a name="zh-cn_topic_0020212677_p30630481"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212677_p49478440"><a name="zh-cn_topic_0020212677_p49478440"></a><a name="zh-cn_topic_0020212677_p49478440"></a>SSH密钥对信息，详情请参见<a href="#zh-cn_topic_0020212677_table32323009">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  keypair字段数据结构说明

<a name="zh-cn_topic_0020212677_table32323009"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212677_row56122340"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p1492112121386"><a name="p1492112121386"></a><a name="p1492112121386"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p18921121223817"><a name="p18921121223817"></a><a name="p18921121223817"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p15921151213387"><a name="p15921151213387"></a><a name="p15921151213387"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p59211712173817"><a name="p59211712173817"></a><a name="p59211712173817"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212677_row1091845"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212677_p21330650"><a name="zh-cn_topic_0020212677_p21330650"></a><a name="zh-cn_topic_0020212677_p21330650"></a>public_key</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p557511364298"><a name="p557511364298"></a><a name="p557511364298"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212677_p28418246"><a name="zh-cn_topic_0020212677_p28418246"></a><a name="zh-cn_topic_0020212677_p28418246"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212677_p47371280"><a name="zh-cn_topic_0020212677_p47371280"></a><a name="zh-cn_topic_0020212677_p47371280"></a>SSH密钥对对应的publicKey信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row23688339"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212677_p39707298"><a name="zh-cn_topic_0020212677_p39707298"></a><a name="zh-cn_topic_0020212677_p39707298"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p13575436172919"><a name="p13575436172919"></a><a name="p13575436172919"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212677_p2977371"><a name="zh-cn_topic_0020212677_p2977371"></a><a name="zh-cn_topic_0020212677_p2977371"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212677_p23019892"><a name="zh-cn_topic_0020212677_p23019892"></a><a name="zh-cn_topic_0020212677_p23019892"></a>SSH密钥对的名称。</p>
</td>
</tr>
<tr id="r3c4e33fabc9540c68209359a32a980a2"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="aa970d73ce0284adf939a2aa27641ee7c"><a name="aa970d73ce0284adf939a2aa27641ee7c"></a><a name="aa970d73ce0284adf939a2aa27641ee7c"></a>fingerprint</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1575163642910"><a name="p1575163642910"></a><a name="p1575163642910"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="ac7b8a303cc3844d984af9934f64f884f"><a name="ac7b8a303cc3844d984af9934f64f884f"></a><a name="ac7b8a303cc3844d984af9934f64f884f"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="a64be21efe04340d48300e885affd4470"><a name="a64be21efe04340d48300e885affd4470"></a><a name="a64be21efe04340d48300e885affd4470"></a>SSH密钥对对应的指纹信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row5852437"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212677_p4285383"><a name="zh-cn_topic_0020212677_p4285383"></a><a name="zh-cn_topic_0020212677_p4285383"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p11575936172913"><a name="p11575936172913"></a><a name="p11575936172913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212677_p64894876"><a name="zh-cn_topic_0020212677_p64894876"></a><a name="zh-cn_topic_0020212677_p64894876"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212677_p63724816"><a name="zh-cn_topic_0020212677_p63724816"></a><a name="zh-cn_topic_0020212677_p63724816"></a>SSH密钥对创建的时间。时间戳，即从1970年1月1日至该时间的总秒数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row36652435"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212677_p16057296"><a name="zh-cn_topic_0020212677_p16057296"></a><a name="zh-cn_topic_0020212677_p16057296"></a>deleted</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p125753364293"><a name="p125753364293"></a><a name="p125753364293"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212677_p58113810"><a name="zh-cn_topic_0020212677_p58113810"></a><a name="zh-cn_topic_0020212677_p58113810"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212677_p19274797"><a name="zh-cn_topic_0020212677_p19274797"></a><a name="zh-cn_topic_0020212677_p19274797"></a>SSH密钥对删除的标记。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row39255446"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212677_p25574597"><a name="zh-cn_topic_0020212677_p25574597"></a><a name="zh-cn_topic_0020212677_p25574597"></a>deleted_at</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p5575203622913"><a name="p5575203622913"></a><a name="p5575203622913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212677_p22776773"><a name="zh-cn_topic_0020212677_p22776773"></a><a name="zh-cn_topic_0020212677_p22776773"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212677_p28378258"><a name="zh-cn_topic_0020212677_p28378258"></a><a name="zh-cn_topic_0020212677_p28378258"></a>SSH密钥对删除的时间。时间戳，即从1970年1月1日至该时间的总秒数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row54077734"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212677_p18220335"><a name="zh-cn_topic_0020212677_p18220335"></a><a name="zh-cn_topic_0020212677_p18220335"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p05756364295"><a name="p05756364295"></a><a name="p05756364295"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212677_p22737212"><a name="zh-cn_topic_0020212677_p22737212"></a><a name="zh-cn_topic_0020212677_p22737212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212677_p66647176"><a name="zh-cn_topic_0020212677_p66647176"></a><a name="zh-cn_topic_0020212677_p66647176"></a>SSH密钥对的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row62953674"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212677_p66082838"><a name="zh-cn_topic_0020212677_p66082838"></a><a name="zh-cn_topic_0020212677_p66082838"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p10575173642917"><a name="p10575173642917"></a><a name="p10575173642917"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212677_p46241663"><a name="zh-cn_topic_0020212677_p46241663"></a><a name="zh-cn_topic_0020212677_p46241663"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212677_p21523158"><a name="zh-cn_topic_0020212677_p21523158"></a><a name="zh-cn_topic_0020212677_p21523158"></a>SSH密钥对的更新时间。时间戳，即从1970年1月1日至该时间的总秒数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212677_row59490699"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212677_p54017281"><a name="zh-cn_topic_0020212677_p54017281"></a><a name="zh-cn_topic_0020212677_p54017281"></a>user_id</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p95751636192912"><a name="p95751636192912"></a><a name="p95751636192912"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212677_p5473047"><a name="zh-cn_topic_0020212677_p5473047"></a><a name="zh-cn_topic_0020212677_p5473047"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212677_p30428869"><a name="zh-cn_topic_0020212677_p30428869"></a><a name="zh-cn_topic_0020212677_p30428869"></a>SSH密钥对所属的用户信息。</p>
</td>
</tr>
<tr id="row11502018145731"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p59248279145731"><a name="p59248279145731"></a><a name="p59248279145731"></a>is_key_protection</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p55751336132911"><a name="p55751336132911"></a><a name="p55751336132911"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p64459916145837"><a name="p64459916145837"></a><a name="p64459916145837"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p29772019145838"><a name="p29772019145838"></a><a name="p29772019145838"></a>SSH密钥对是否私钥托管与保护。</p>
</td>
</tr>
<tr id="row43203711263"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p103037192615"><a name="p103037192615"></a><a name="p103037192615"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p12575536202918"><a name="p12575536202918"></a><a name="p12575536202918"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1393742613"><a name="p1393742613"></a><a name="p1393742613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p13193712619"><a name="p13193712619"></a><a name="p13193712619"></a>SSH密钥对的描述信息</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section8112517104818"></a>

-   请求样例

    无

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


## 状态码<a name="s45a1d5602b9a4b5b942549cb65e046cc"></a>

请参考[状态码](状态码.md)。

