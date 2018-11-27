# 查询SSH密钥对列表<a name="dew_02_0208"></a>

## 功能介绍<a name="s306004e5a98e4283a1bfcb4adc2fa508"></a>

查询SSH密钥对列表。

## URI<a name="sbbff16336947456f8342473caef444e2"></a>

-   URI格式

    GET /v2.1/\{project\_id\}/os-keypairs

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
    </tbody>
    </table>


## 请求消息<a name="section66616625145216"></a>

请求参数

无

## 响应消息<a name="s5ced3e283dd94140975a617fcfe7abe6"></a>

响应参数

<a name="zh-cn_topic_0020212676_table46959463"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row9766180"><th class="cellrowborder" valign="top" width="24.122412241224122%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020212676_p52863116"><a name="zh-cn_topic_0020212676_p52863116"></a><a name="zh-cn_topic_0020212676_p52863116"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="31.453145314531454%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020212676_p16299242"><a name="zh-cn_topic_0020212676_p16299242"></a><a name="zh-cn_topic_0020212676_p16299242"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.42444244424442%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020212676_p45170224"><a name="zh-cn_topic_0020212676_p45170224"></a><a name="zh-cn_topic_0020212676_p45170224"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row34909498"><td class="cellrowborder" valign="top" width="24.122412241224122%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212676_p9097072"><a name="zh-cn_topic_0020212676_p9097072"></a><a name="zh-cn_topic_0020212676_p9097072"></a>keypairs</p>
</td>
<td class="cellrowborder" valign="top" width="31.453145314531454%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212676_p26115459"><a name="zh-cn_topic_0020212676_p26115459"></a><a name="zh-cn_topic_0020212676_p26115459"></a>列表数据结构[1]</p>
</td>
<td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212676_p46361647"><a name="zh-cn_topic_0020212676_p46361647"></a><a name="zh-cn_topic_0020212676_p46361647"></a>SSH密钥对信息列表。</p>
</td>
</tr>
</tbody>
</table>

\[1.1\] keypairs字段数据结构说明

<a name="zh-cn_topic_0020212676_table41882197"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row19241577"><th class="cellrowborder" valign="top" width="23.932393239323932%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020212676_p15063922"><a name="zh-cn_topic_0020212676_p15063922"></a><a name="zh-cn_topic_0020212676_p15063922"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="31.83318331833183%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020212676_p50145164"><a name="zh-cn_topic_0020212676_p50145164"></a><a name="zh-cn_topic_0020212676_p50145164"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.23442344234424%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020212676_p35226478"><a name="zh-cn_topic_0020212676_p35226478"></a><a name="zh-cn_topic_0020212676_p35226478"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row34772456"><td class="cellrowborder" valign="top" width="23.932393239323932%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212676_p65105571"><a name="zh-cn_topic_0020212676_p65105571"></a><a name="zh-cn_topic_0020212676_p65105571"></a>keypair</p>
</td>
<td class="cellrowborder" valign="top" width="31.83318331833183%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212676_p9736186"><a name="zh-cn_topic_0020212676_p9736186"></a><a name="zh-cn_topic_0020212676_p9736186"></a>字典数据结构[1.1.1]</p>
</td>
<td class="cellrowborder" valign="top" width="44.23442344234424%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212676_p51249570"><a name="zh-cn_topic_0020212676_p51249570"></a><a name="zh-cn_topic_0020212676_p51249570"></a>SSH密钥对信息详情。</p>
</td>
</tr>
</tbody>
</table>

\[1.1.1\] keypair字段数据结构说明

<a name="zh-cn_topic_0020212676_table48408329"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row27259828"><th class="cellrowborder" valign="top" width="23.93%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020212676_p60562422"><a name="zh-cn_topic_0020212676_p60562422"></a><a name="zh-cn_topic_0020212676_p60562422"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="32.019999999999996%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020212676_p65580385"><a name="zh-cn_topic_0020212676_p65580385"></a><a name="zh-cn_topic_0020212676_p65580385"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.05%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020212676_p10410969"><a name="zh-cn_topic_0020212676_p10410969"></a><a name="zh-cn_topic_0020212676_p10410969"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row37982174"><td class="cellrowborder" valign="top" width="23.93%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212676_p56657239"><a name="zh-cn_topic_0020212676_p56657239"></a><a name="zh-cn_topic_0020212676_p56657239"></a>fingerprint</p>
</td>
<td class="cellrowborder" valign="top" width="32.019999999999996%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212676_p12150471"><a name="zh-cn_topic_0020212676_p12150471"></a><a name="zh-cn_topic_0020212676_p12150471"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.05%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212676_p66432381"><a name="zh-cn_topic_0020212676_p66432381"></a><a name="zh-cn_topic_0020212676_p66432381"></a>SSH密钥对应指纹信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212676_row61020521"><td class="cellrowborder" valign="top" width="23.93%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212676_p43715136"><a name="zh-cn_topic_0020212676_p43715136"></a><a name="zh-cn_topic_0020212676_p43715136"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="32.019999999999996%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212676_p58836357"><a name="zh-cn_topic_0020212676_p58836357"></a><a name="zh-cn_topic_0020212676_p58836357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.05%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212676_p9140568"><a name="zh-cn_topic_0020212676_p9140568"></a><a name="zh-cn_topic_0020212676_p9140568"></a>SSH密钥对的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212676_row15156252"><td class="cellrowborder" valign="top" width="23.93%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212676_p19696890"><a name="zh-cn_topic_0020212676_p19696890"></a><a name="zh-cn_topic_0020212676_p19696890"></a>public_key</p>
</td>
<td class="cellrowborder" valign="top" width="32.019999999999996%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212676_p46735588"><a name="zh-cn_topic_0020212676_p46735588"></a><a name="zh-cn_topic_0020212676_p46735588"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.05%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212676_p46049856"><a name="zh-cn_topic_0020212676_p46049856"></a><a name="zh-cn_topic_0020212676_p46049856"></a>SSH密钥对对应的publicKey信息。</p>
</td>
</tr>
<tr id="row372796214537"><td class="cellrowborder" valign="top" width="23.93%" headers="mcps1.1.4.1.1 "><p id="p3352949614537"><a name="p3352949614537"></a><a name="p3352949614537"></a>is_key_protection</p>
</td>
<td class="cellrowborder" valign="top" width="32.019999999999996%" headers="mcps1.1.4.1.2 "><p id="p3153465914537"><a name="p3153465914537"></a><a name="p3153465914537"></a>boolean</p>
</td>
<td class="cellrowborder" valign="top" width="44.05%" headers="mcps1.1.4.1.3 "><p id="p417056214537"><a name="p417056214537"></a><a name="p417056214537"></a>SSH密钥对是否私钥托管与保护。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section8112517104818"></a>

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


## 返回值<a name="s45a1d5602b9a4b5b942549cb65e046cc"></a>

请参考[状态码](状态码.md)。

