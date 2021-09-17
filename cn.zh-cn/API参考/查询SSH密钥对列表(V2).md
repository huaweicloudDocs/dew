# 查询SSH密钥对列表\(V2\)<a name="dew_02_0201"></a>

## 功能介绍<a name="s7cbd3305f2114e6bb336f9bcb5387b89"></a>

查询SSH密钥对信息列表。

## URI<a name="s045f38bdf49a4fb9a061806bf70c2998"></a>

-   URI格式

    GET /v2/\{project\_id\}/os-keypairs

-   参数说明

    **表 1**  参数说明

    <a name="zh-cn_topic_0020212676_table38623499"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020212676_row59671974"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0020212676_p1591698"><a name="zh-cn_topic_0020212676_p1591698"></a><a name="zh-cn_topic_0020212676_p1591698"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0020212676_p61818739"><a name="zh-cn_topic_0020212676_p61818739"></a><a name="zh-cn_topic_0020212676_p61818739"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p334014371274"><a name="p334014371274"></a><a name="p334014371274"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0020212676_p41262001"><a name="zh-cn_topic_0020212676_p41262001"></a><a name="zh-cn_topic_0020212676_p41262001"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020212676_row53887795"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p2835298"><a name="zh-cn_topic_0020212676_p2835298"></a><a name="zh-cn_topic_0020212676_p2835298"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020212676_p28332581"><a name="zh-cn_topic_0020212676_p28332581"></a><a name="zh-cn_topic_0020212676_p28332581"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1340637132717"><a name="p1340637132717"></a><a name="p1340637132717"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p13237733"><a name="zh-cn_topic_0020212676_p13237733"></a><a name="zh-cn_topic_0020212676_p13237733"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="s6ca6403b05934c2180363673865c260c"></a>

无

## 响应消息<a name="s5ced3e283dd94140975a617fcfe7abe6"></a>

**表 2**  响应参数

<a name="zh-cn_topic_0020212676_table46959463"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row9766180"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p1257117224367"><a name="p1257117224367"></a><a name="p1257117224367"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p18571142210368"><a name="p18571142210368"></a><a name="p18571142210368"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p6571622153612"><a name="p6571622153612"></a><a name="p6571622153612"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p957172214366"><a name="p957172214366"></a><a name="p957172214366"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row34909498"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p9097072"><a name="zh-cn_topic_0020212676_p9097072"></a><a name="zh-cn_topic_0020212676_p9097072"></a>keypairs</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1755954510273"><a name="p1755954510273"></a><a name="p1755954510273"></a>是</p>
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
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row19241577"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p14941425103610"><a name="p14941425103610"></a><a name="p14941425103610"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p1594112523618"><a name="p1594112523618"></a><a name="p1594112523618"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p9941025123617"><a name="p9941025123617"></a><a name="p9941025123617"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p16942255365"><a name="p16942255365"></a><a name="p16942255365"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row34772456"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p65105571"><a name="zh-cn_topic_0020212676_p65105571"></a><a name="zh-cn_topic_0020212676_p65105571"></a>keypair</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p11109104972713"><a name="p11109104972713"></a><a name="p11109104972713"></a>是</p>
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
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row27259828"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p87123291368"><a name="p87123291368"></a><a name="p87123291368"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p147126291367"><a name="p147126291367"></a><a name="p147126291367"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p47121029103610"><a name="p47121029103610"></a><a name="p47121029103610"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p57121629103611"><a name="p57121629103611"></a><a name="p57121629103611"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row37982174"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p56657239"><a name="zh-cn_topic_0020212676_p56657239"></a><a name="zh-cn_topic_0020212676_p56657239"></a>fingerprint</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p823245272718"><a name="p823245272718"></a><a name="p823245272718"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p12150471"><a name="zh-cn_topic_0020212676_p12150471"></a><a name="zh-cn_topic_0020212676_p12150471"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p66432381"><a name="zh-cn_topic_0020212676_p66432381"></a><a name="zh-cn_topic_0020212676_p66432381"></a>SSH密钥对应指纹信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212676_row61020521"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p43715136"><a name="zh-cn_topic_0020212676_p43715136"></a><a name="zh-cn_topic_0020212676_p43715136"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p132320527278"><a name="p132320527278"></a><a name="p132320527278"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p58836357"><a name="zh-cn_topic_0020212676_p58836357"></a><a name="zh-cn_topic_0020212676_p58836357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p9140568"><a name="zh-cn_topic_0020212676_p9140568"></a><a name="zh-cn_topic_0020212676_p9140568"></a>SSH密钥对的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212676_row15156252"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p19696890"><a name="zh-cn_topic_0020212676_p19696890"></a><a name="zh-cn_topic_0020212676_p19696890"></a>public_key</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p62321526275"><a name="p62321526275"></a><a name="p62321526275"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p46735588"><a name="zh-cn_topic_0020212676_p46735588"></a><a name="zh-cn_topic_0020212676_p46735588"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p46049856"><a name="zh-cn_topic_0020212676_p46049856"></a><a name="zh-cn_topic_0020212676_p46049856"></a>SSH密钥对对应的publicKey信息。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section116861411116"></a>

如下以查询SSH密钥列表为例。

-   请求样例

    无

-   响应样例

    ```
    {
        "keypairs": [
            {
                "keypair": {
                    "fingerprint": "15:b0:f8:b3:f9:48:63:71:cf:7b:5b:38:6d:44:2d:4a",
                    "name": "keypair-601a2305-4f25-41ed-89c6-2a966fc8027a",
                    "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAAAgQC+Eo/RZRngaGTkFs7I62ZjsIlO79KklKbMXi8F+KITD4bVQHHn+kV+4gRgkgCRbdoDqoGfpaDFs877DYX9n4z6FrAIZ4PES8TNKhatifpn9NdQYWA+IkU8CuvlEKGuFpKRi/k7JLos/gHi2hy7QUwgtRvcefvD/vgQZOVw/mGR9Q== Generated-by-Nova\n"
                }
            }
        ]
    }
    ```


## 状态码<a name="s1d07b15660e74df7ae0a9248cbfea1a5"></a>

请参考[状态码](状态码.md)。

