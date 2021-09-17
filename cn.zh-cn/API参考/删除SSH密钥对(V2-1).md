# 删除SSH密钥对\(V2.1\)<a name="dew_02_0211"></a>

## 功能介绍<a name="s306004e5a98e4283a1bfcb4adc2fa508"></a>

根据SSH密钥对的名称，删除指定SSH密钥对。

## URI<a name="sbbff16336947456f8342473caef444e2"></a>

-   URI格式

    DELETE /v2.1/\{project\_id\}/os-keypairs/\{keypair\_name\}

-   参数说明

    **表 1**  参数说明

    <a name="table189326204518"></a>
    <table><thead align="left"><tr id="row20932152012518"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0020212676_p1591698"><a name="zh-cn_topic_0020212676_p1591698"></a><a name="zh-cn_topic_0020212676_p1591698"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0020212676_p61818739"><a name="zh-cn_topic_0020212676_p61818739"></a><a name="zh-cn_topic_0020212676_p61818739"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p334014371274"><a name="p334014371274"></a><a name="p334014371274"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0020212676_p41262001"><a name="zh-cn_topic_0020212676_p41262001"></a><a name="zh-cn_topic_0020212676_p41262001"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row893242075115"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p49321820135110"><a name="p49321820135110"></a><a name="p49321820135110"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1593232055110"><a name="p1593232055110"></a><a name="p1593232055110"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1365713263010"><a name="p1365713263010"></a><a name="p1365713263010"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p159321020165112"><a name="p159321020165112"></a><a name="p159321020165112"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row159325201517"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p169320206519"><a name="p169320206519"></a><a name="p169320206519"></a>keypair_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p59321420115112"><a name="p59321420115112"></a><a name="p59321420115112"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1665762133013"><a name="p1665762133013"></a><a name="p1665762133013"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p189321820205113"><a name="p189321820205113"></a><a name="p189321820205113"></a>SSH密钥对名称。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="sa2cfd6b2f5f34f879f1e1a21f8123f29"></a>

无

## 响应消息<a name="s212ddf26dea54058a346fa6a6a93f94b"></a>

无

## 状态码<a name="s45a1d5602b9a4b5b942549cb65e046cc"></a>

请参考[状态码](状态码.md)。

