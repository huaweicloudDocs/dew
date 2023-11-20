# 查询SSH密钥对列表\(V2.1\)<a name="dew_02_0208"></a>

## 功能介绍<a name="s306004e5a98e4283a1bfcb4adc2fa508"></a>

查询SSH密钥对列表。

## URI<a name="sbbff16336947456f8342473caef444e2"></a>

-   URI格式

    GET /v2.1/\{project\_id\}/os-keypairs

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
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p43391910102919"><a name="p43391910102919"></a><a name="p43391910102919"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="acf1687032c074bd0bd72b8b9b1fa31dc"><a name="acf1687032c074bd0bd72b8b9b1fa31dc"></a><a name="acf1687032c074bd0bd72b8b9b1fa31dc"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

## 请求消息<a name="section66616625145216"></a>

无

## 响应消息<a name="s5ced3e283dd94140975a617fcfe7abe6"></a>

**表 2**  响应参数

<a name="zh-cn_topic_0020212676_table46959463"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row9766180"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p121413546378"><a name="p121413546378"></a><a name="p121413546378"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p19214185416375"><a name="p19214185416375"></a><a name="p19214185416375"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p92140549371"><a name="p92140549371"></a><a name="p92140549371"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p1021415418374"><a name="p1021415418374"></a><a name="p1021415418374"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row34909498"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p9097072"><a name="zh-cn_topic_0020212676_p9097072"></a><a name="zh-cn_topic_0020212676_p9097072"></a>keypairs</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p182291813102917"><a name="p182291813102917"></a><a name="p182291813102917"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p26115459"><a name="zh-cn_topic_0020212676_p26115459"></a><a name="zh-cn_topic_0020212676_p26115459"></a>Array of objects</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p46361647"><a name="zh-cn_topic_0020212676_p46361647"></a><a name="zh-cn_topic_0020212676_p46361647"></a>SSH密钥对信息列表，详情请参见<a href="#zh-cn_topic_0020212676_table41882197">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  keypairs字段数据结构说明

<a name="zh-cn_topic_0020212676_table41882197"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row19241577"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p77718579372"><a name="p77718579372"></a><a name="p77718579372"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p15772557123716"><a name="p15772557123716"></a><a name="p15772557123716"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p11772157133716"><a name="p11772157133716"></a><a name="p11772157133716"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p14772185713375"><a name="p14772185713375"></a><a name="p14772185713375"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row34772456"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p65105571"><a name="zh-cn_topic_0020212676_p65105571"></a><a name="zh-cn_topic_0020212676_p65105571"></a>keypair</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1243441611297"><a name="p1243441611297"></a><a name="p1243441611297"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p9736186"><a name="zh-cn_topic_0020212676_p9736186"></a><a name="zh-cn_topic_0020212676_p9736186"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p51249570"><a name="zh-cn_topic_0020212676_p51249570"></a><a name="zh-cn_topic_0020212676_p51249570"></a>SSH密钥对信息详情，详情请参见<a href="#zh-cn_topic_0020212676_table48408329">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  keypair字段数据结构说明

<a name="zh-cn_topic_0020212676_table48408329"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row27259828"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p55698203813"><a name="p55698203813"></a><a name="p55698203813"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p18569625386"><a name="p18569625386"></a><a name="p18569625386"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p1156913213389"><a name="p1156913213389"></a><a name="p1156913213389"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p1756942113819"><a name="p1756942113819"></a><a name="p1756942113819"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row37982174"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p56657239"><a name="zh-cn_topic_0020212676_p56657239"></a><a name="zh-cn_topic_0020212676_p56657239"></a>fingerprint</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1475412192299"><a name="p1475412192299"></a><a name="p1475412192299"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p12150471"><a name="zh-cn_topic_0020212676_p12150471"></a><a name="zh-cn_topic_0020212676_p12150471"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p66432381"><a name="zh-cn_topic_0020212676_p66432381"></a><a name="zh-cn_topic_0020212676_p66432381"></a>SSH密钥对应指纹信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212676_row61020521"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p43715136"><a name="zh-cn_topic_0020212676_p43715136"></a><a name="zh-cn_topic_0020212676_p43715136"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p16754141982911"><a name="p16754141982911"></a><a name="p16754141982911"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p58836357"><a name="zh-cn_topic_0020212676_p58836357"></a><a name="zh-cn_topic_0020212676_p58836357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p9140568"><a name="zh-cn_topic_0020212676_p9140568"></a><a name="zh-cn_topic_0020212676_p9140568"></a>SSH密钥对的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212676_row15156252"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p19696890"><a name="zh-cn_topic_0020212676_p19696890"></a><a name="zh-cn_topic_0020212676_p19696890"></a>public_key</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p20754161912913"><a name="p20754161912913"></a><a name="p20754161912913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p46735588"><a name="zh-cn_topic_0020212676_p46735588"></a><a name="zh-cn_topic_0020212676_p46735588"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p46049856"><a name="zh-cn_topic_0020212676_p46049856"></a><a name="zh-cn_topic_0020212676_p46049856"></a>SSH密钥对对应的publicKey信息。</p>
</td>
</tr>
<tr id="row372796214537"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p3352949614537"><a name="p3352949614537"></a><a name="p3352949614537"></a>is_key_protection</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p18754151992914"><a name="p18754151992914"></a><a name="p18754151992914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p3153465914537"><a name="p3153465914537"></a><a name="p3153465914537"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p417056214537"><a name="p417056214537"></a><a name="p417056214537"></a>SSH密钥对是否私钥托管与保护。</p>
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
     "keypairs": [{
       "keypair": {
        "fingerprint": "15:b0:f8:b3:f9:48:63:71:cf:7b:5b:38:6d:44:2d:4a",
        "name": "keypair-601a2305-4f25-41ed-89c6-2a966fc8027a",
        "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAAAgQC+Eo/RZRngaGTkFs7I62ZjsIlO79KklKbMXi8F+KITD4bVQHHn+kV+4gRgkgCRbdoDqoGfpaDFs877DYX9n4z6FrAIZ4PES8TNKhatifpn9NdQYWA+IkU8CuvlEKGuFpKRi/k7JLos/gHi2hy7QUwgtRvcefvD/vgQZOVw/mGR9Q== Generated-by-Nova\n",
        "is_key_protection": true
       }
      }
     ]
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

