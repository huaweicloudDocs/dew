# 删除SSH密钥对\(V2\)<a name="dew_02_0204"></a>

## 功能介绍<a name="s9636d7e16b064e68a5c68d5c50a738e2"></a>

根据SSH密钥对的名称，删除指定SSH密钥对。

## URI<a name="sce81dd29969b483b929fba7c1713dacf"></a>

-   URI格式

    DELETE /v2/\{project\_id\}/os-keypairs/\{keypair\_name\}

-   参数说明

    **表 1**  参数说明

    <a name="zh-cn_topic_0020212680_table48776445"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020212680_row64721603"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0020212676_p1591698"><a name="zh-cn_topic_0020212676_p1591698"></a><a name="zh-cn_topic_0020212676_p1591698"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0020212676_p61818739"><a name="zh-cn_topic_0020212676_p61818739"></a><a name="zh-cn_topic_0020212676_p61818739"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p334014371274"><a name="p334014371274"></a><a name="p334014371274"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0020212676_p41262001"><a name="zh-cn_topic_0020212676_p41262001"></a><a name="zh-cn_topic_0020212676_p41262001"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020212680_row8464456"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212680_p14532322"><a name="zh-cn_topic_0020212680_p14532322"></a><a name="zh-cn_topic_0020212680_p14532322"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020212680_p36267453"><a name="zh-cn_topic_0020212680_p36267453"></a><a name="zh-cn_topic_0020212680_p36267453"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1848331112813"><a name="p1848331112813"></a><a name="p1848331112813"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212680_p51982593"><a name="zh-cn_topic_0020212680_p51982593"></a><a name="zh-cn_topic_0020212680_p51982593"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020212680_row65190153"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212680_p45911036"><a name="zh-cn_topic_0020212680_p45911036"></a><a name="zh-cn_topic_0020212680_p45911036"></a>keypair_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020212680_p27806444"><a name="zh-cn_topic_0020212680_p27806444"></a><a name="zh-cn_topic_0020212680_p27806444"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1284818311283"><a name="p1284818311283"></a><a name="p1284818311283"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212680_p37729472"><a name="zh-cn_topic_0020212680_p37729472"></a><a name="zh-cn_topic_0020212680_p37729472"></a>SSH密钥对的名称。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="s9d23df5d05ef41d1b95749c2985493f0"></a>

无

## 响应消息<a name="s305e1f901cd84000aea98cc7bc18f8d9"></a>

无

## 状态码<a name="s1d5dbc7aa4614ef9b6d9729b4cd150bd"></a>

请参考[状态码](状态码.md)。

