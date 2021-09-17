# 复制SSH密钥对\(V2\)<a name="dew_02_0206"></a>

## 功能介绍<a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_section33132068"></a>

在同一个租户下可能包含多个用户帐号，将同一租户下目标用户帐号下的密钥对复制到当前用户帐号下。

## URI<a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_section29753161"></a>

-   URI格式

    POST /v2/\{project\_id\}/os-keypairs/copy

-   参数说明

    **表 1**  参数说明

    <a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_table48776445"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0102102227_zh-cn_topic_0020212680_row64721603"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0020212676_p1591698"><a name="zh-cn_topic_0020212676_p1591698"></a><a name="zh-cn_topic_0020212676_p1591698"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0020212676_p61818739"><a name="zh-cn_topic_0020212676_p61818739"></a><a name="zh-cn_topic_0020212676_p61818739"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p334014371274"><a name="p334014371274"></a><a name="p334014371274"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0020212676_p41262001"><a name="zh-cn_topic_0020212676_p41262001"></a><a name="zh-cn_topic_0020212676_p41262001"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0102102227_zh-cn_topic_0020212680_row8464456"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0102102227_p20346069102656"><a name="zh-cn_topic_0102102227_p20346069102656"></a><a name="zh-cn_topic_0102102227_p20346069102656"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0102102227_p37418879102656"><a name="zh-cn_topic_0102102227_p37418879102656"></a><a name="zh-cn_topic_0102102227_p37418879102656"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p8514125702813"><a name="p8514125702813"></a><a name="p8514125702813"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0102102227_p11030378102656"><a name="zh-cn_topic_0102102227_p11030378102656"></a><a name="zh-cn_topic_0102102227_p11030378102656"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section66616625145216"></a>

**表 2**  请求参数

<a name="table4488133315350"></a>
<table><thead align="left"><tr id="row1563118915350"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p556733893713"><a name="p556733893713"></a><a name="p556733893713"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p1756793817375"><a name="p1756793817375"></a><a name="p1756793817375"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p5567938163712"><a name="p5567938163712"></a><a name="p5567938163712"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p2567238143713"><a name="p2567238143713"></a><a name="p2567238143713"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row401591615350"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p5685375915350"><a name="p5685375915350"></a><a name="p5685375915350"></a>user_name</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p3067406515659"><a name="p3067406515659"></a><a name="p3067406515659"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p5696368515529"><a name="p5696368515529"></a><a name="p5696368515529"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p5065578615529"><a name="p5065578615529"></a><a name="p5065578615529"></a>同一租户下的目标用户名。</p>
</td>
</tr>
<tr id="row385275841556"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p3143599415623"><a name="p3143599415623"></a><a name="p3143599415623"></a>force</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p157130715659"><a name="p157130715659"></a><a name="p157130715659"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p2602331515623"><a name="p2602331515623"></a><a name="p2602331515623"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p2751378615623"><a name="p2751378615623"></a><a name="p2751378615623"></a>是否强制覆盖已有密钥对。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section4990348015035"></a>

**表 3**  响应参数

<a name="zh-cn_topic_0020212676_table46959463"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row9766180"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p1069004133710"><a name="p1069004133710"></a><a name="p1069004133710"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p176901141153711"><a name="p176901141153711"></a><a name="p176901141153711"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p16690154116378"><a name="p16690154116378"></a><a name="p16690154116378"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p126901241173712"><a name="p126901241173712"></a><a name="p126901241173712"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19806183272219"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p37599211015"><a name="p37599211015"></a><a name="p37599211015"></a>changed</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p5146313291"><a name="p5146313291"></a><a name="p5146313291"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p975982405"><a name="p975982405"></a><a name="p975982405"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p137601221306"><a name="p137601221306"></a><a name="p137601221306"></a>复制的密钥对数量。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212676_row34909498"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p9097072"><a name="zh-cn_topic_0020212676_p9097072"></a><a name="zh-cn_topic_0020212676_p9097072"></a>success</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p614614116298"><a name="p614614116298"></a><a name="p614614116298"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p26115459"><a name="zh-cn_topic_0020212676_p26115459"></a><a name="zh-cn_topic_0020212676_p26115459"></a>Array of objects</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p46361647"><a name="zh-cn_topic_0020212676_p46361647"></a><a name="zh-cn_topic_0020212676_p46361647"></a>复制成功的密钥对列表，详情请参见<a href="#zh-cn_topic_0020212676_table41882197">表4</a>。</p>
</td>
</tr>
<tr id="row23380060175814"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p9093948175814"><a name="p9093948175814"></a><a name="p9093948175814"></a>failed</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p41466120291"><a name="p41466120291"></a><a name="p41466120291"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p65521217175814"><a name="p65521217175814"></a><a name="p65521217175814"></a>Array of objects</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p5618383175814"><a name="p5618383175814"></a><a name="p5618383175814"></a>复制失败的密钥对列表，详情请参见<a href="#zh-cn_topic_0020212676_table41882197">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  success/failed字段数据结构说明

<a name="zh-cn_topic_0020212676_table41882197"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212676_row19241577"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p47001544103714"><a name="p47001544103714"></a><a name="p47001544103714"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p16700344143718"><a name="p16700344143718"></a><a name="p16700344143718"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p170014453719"><a name="p170014453719"></a><a name="p170014453719"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p370012444377"><a name="p370012444377"></a><a name="p370012444377"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212676_row34772456"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212676_p65105571"><a name="zh-cn_topic_0020212676_p65105571"></a><a name="zh-cn_topic_0020212676_p65105571"></a>keypair</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p82206592915"><a name="p82206592915"></a><a name="p82206592915"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212676_p9736186"><a name="zh-cn_topic_0020212676_p9736186"></a><a name="zh-cn_topic_0020212676_p9736186"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212676_p51249570"><a name="zh-cn_topic_0020212676_p51249570"></a><a name="zh-cn_topic_0020212676_p51249570"></a>密钥对名称。</p>
</td>
</tr>
<tr id="row1632961175912"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p65160992175912"><a name="p65160992175912"></a><a name="p65160992175912"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1522012519298"><a name="p1522012519298"></a><a name="p1522012519298"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p43548988175912"><a name="p43548988175912"></a><a name="p43548988175912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p37807100175912"><a name="p37807100175912"></a><a name="p37807100175912"></a>任务消息</p>
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


## 状态码<a name="zh-cn_topic_0102102227_zh-cn_topic_0020212680_section13891457"></a>

请参考[状态码](状态码.md)。

