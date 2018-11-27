# 复制SSH密钥对（旧）<a name="dew_02_0205"></a>

## 功能介绍<a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_section33132068"></a>

在同一个租户下可能包含多个用户帐号，将同一租户下目标用户帐号下的密钥对复制到当前用户帐号下。

## URI<a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_section29753161"></a>

-   URI格式

    POST /v2/\{project\_id\}/kps/copy

-   参数说明

    <a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_table48776445"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0102102227_zh-cn_topic_0020212680_row64721603"><th class="cellrowborder" valign="top" width="25.44%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0102102227_zh-cn_topic_0020212680_p7958508"><a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_p7958508"></a><a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_p7958508"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.93%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0102102227_zh-cn_topic_0020212680_p40659381"><a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_p40659381"></a><a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_p40659381"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.63%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0102102227_zh-cn_topic_0020212680_p5075526"><a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_p5075526"></a><a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_p5075526"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0102102227_zh-cn_topic_0020212680_row8464456"><td class="cellrowborder" valign="top" width="25.44%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102102227_p20346069102656"><a name="zh-cn_topic_0102102227_p20346069102656"></a><a name="zh-cn_topic_0102102227_p20346069102656"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.93%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102102227_p37418879102656"><a name="zh-cn_topic_0102102227_p37418879102656"></a><a name="zh-cn_topic_0102102227_p37418879102656"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.63%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0102102227_p11030378102656"><a name="zh-cn_topic_0102102227_p11030378102656"></a><a name="zh-cn_topic_0102102227_p11030378102656"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section66616625145216"></a>

请求参数

<a name="table4488133315350"></a>
<table><thead align="left"><tr id="row1563118915350"><th class="cellrowborder" valign="top" width="21.62%" id="mcps1.1.5.1.1"><p id="p5699009117562"><a name="p5699009117562"></a><a name="p5699009117562"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.719999999999999%" id="mcps1.1.5.1.2"><p id="p2775421717562"><a name="p2775421717562"></a><a name="p2775421717562"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="22.74%" id="mcps1.1.5.1.3"><p id="p5693439117562"><a name="p5693439117562"></a><a name="p5693439117562"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.92%" id="mcps1.1.5.1.4"><p id="p5623969417562"><a name="p5623969417562"></a><a name="p5623969417562"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row401591615350"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.1.5.1.1 "><p id="p5685375915350"><a name="p5685375915350"></a><a name="p5685375915350"></a>user_name</p>
</td>
<td class="cellrowborder" valign="top" width="13.719999999999999%" headers="mcps1.1.5.1.2 "><p id="p3067406515659"><a name="p3067406515659"></a><a name="p3067406515659"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.74%" headers="mcps1.1.5.1.3 "><p id="p5696368515529"><a name="p5696368515529"></a><a name="p5696368515529"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.92%" headers="mcps1.1.5.1.4 "><p id="p5065578615529"><a name="p5065578615529"></a><a name="p5065578615529"></a>同一租户下的目标用户名。</p>
</td>
</tr>
<tr id="row385275841556"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.1.5.1.1 "><p id="p3143599415623"><a name="p3143599415623"></a><a name="p3143599415623"></a>force</p>
</td>
<td class="cellrowborder" valign="top" width="13.719999999999999%" headers="mcps1.1.5.1.2 "><p id="p157130715659"><a name="p157130715659"></a><a name="p157130715659"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.74%" headers="mcps1.1.5.1.3 "><p id="p2602331515623"><a name="p2602331515623"></a><a name="p2602331515623"></a>boolean</p>
</td>
<td class="cellrowborder" valign="top" width="41.92%" headers="mcps1.1.5.1.4 "><p id="p2751378615623"><a name="p2751378615623"></a><a name="p2751378615623"></a>是否强制覆盖已有密钥对。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section4990348015035"></a>

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
<tbody><tr id="row19806183272219"><td class="cellrowborder" valign="top" width="24.122412241224122%" headers="mcps1.1.4.1.1 "><p id="p37599211015"><a name="p37599211015"></a><a name="p37599211015"></a>changed</p>
</td>
<td class="cellrowborder" valign="top" width="31.453145314531454%" headers="mcps1.1.4.1.2 "><p id="p975982405"><a name="p975982405"></a><a name="p975982405"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.1.4.1.3 "><p id="p137601221306"><a name="p137601221306"></a><a name="p137601221306"></a>复制的密钥对数量。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212676_row34909498"><td class="cellrowborder" valign="top" width="24.122412241224122%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020212676_p9097072"><a name="zh-cn_topic_0020212676_p9097072"></a><a name="zh-cn_topic_0020212676_p9097072"></a>success</p>
</td>
<td class="cellrowborder" valign="top" width="31.453145314531454%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212676_p26115459"><a name="zh-cn_topic_0020212676_p26115459"></a><a name="zh-cn_topic_0020212676_p26115459"></a>[1]字典数据结构</p>
</td>
<td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212676_p46361647"><a name="zh-cn_topic_0020212676_p46361647"></a><a name="zh-cn_topic_0020212676_p46361647"></a>复制成功的密钥对列表。</p>
</td>
</tr>
<tr id="row23380060175814"><td class="cellrowborder" valign="top" width="24.122412241224122%" headers="mcps1.1.4.1.1 "><p id="p9093948175814"><a name="p9093948175814"></a><a name="p9093948175814"></a>failed</p>
</td>
<td class="cellrowborder" valign="top" width="31.453145314531454%" headers="mcps1.1.4.1.2 "><p id="p65521217175814"><a name="p65521217175814"></a><a name="p65521217175814"></a>[1]字典数据结构</p>
</td>
<td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.1.4.1.3 "><p id="p5618383175814"><a name="p5618383175814"></a><a name="p5618383175814"></a>复制失败的密钥对列表。</p>
</td>
</tr>
</tbody>
</table>

\[1\] success/failed字典数据结构说明

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
<td class="cellrowborder" valign="top" width="31.83318331833183%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020212676_p9736186"><a name="zh-cn_topic_0020212676_p9736186"></a><a name="zh-cn_topic_0020212676_p9736186"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.23442344234424%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020212676_p51249570"><a name="zh-cn_topic_0020212676_p51249570"></a><a name="zh-cn_topic_0020212676_p51249570"></a>密钥对名称。</p>
</td>
</tr>
<tr id="row1632961175912"><td class="cellrowborder" valign="top" width="23.932393239323932%" headers="mcps1.1.4.1.1 "><p id="p65160992175912"><a name="p65160992175912"></a><a name="p65160992175912"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="31.83318331833183%" headers="mcps1.1.4.1.2 "><p id="p43548988175912"><a name="p43548988175912"></a><a name="p43548988175912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.23442344234424%" headers="mcps1.1.4.1.3 "><p id="p37807100175912"><a name="p37807100175912"></a><a name="p37807100175912"></a>任务消息。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_section66451858"></a>

-   请求样例

    ```
    {
     "user_name": "kpsuser"
    }
    ```


-   响应样例

    ```
    {
        "changed": 2,
        "success": [
            {
                "keypair": "KeyPair-test1",
                "message": "imported"
            },
            {
                "keypair": "KeyPair-test2",
                "message": "imported"
            }
        ],
        "failed": [
            {
                "keypair": "KeyPair-test3",
                "message": "exist"
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


## 返回值<a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_section13891457"></a>

请参考[状态码](状态码.md)。

