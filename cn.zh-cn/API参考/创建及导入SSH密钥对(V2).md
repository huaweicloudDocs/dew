# 创建及导入SSH密钥对\(V2\)<a name="dew_02_0203"></a>

## 功能介绍<a name="s02716ebaa1b94de5a935108e664aad10"></a>

创建SSH密钥对，或把公钥导入华为云中，生成SSH密钥对。

创建SSH密钥对成功后，请把响应数据中的私钥内容保存到本地文件，用户使用该私钥登录云服务器。为保证云服务器安全，私钥数据只能下载一次，请妥善保管。

## URI<a name="s63dadb0e694d4a49aeea23a7053b94a2"></a>

-   URI格式

    POST /v2/\{project\_id\}/os-keypairs

-   参数说明

    **表 1**  参数说明

    <a name="zh-cn_topic_0020212678_table909717"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020212678_row9180116"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0020212676_p1591698"><a name="zh-cn_topic_0020212676_p1591698"></a><a name="zh-cn_topic_0020212676_p1591698"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0020212676_p61818739"><a name="zh-cn_topic_0020212676_p61818739"></a><a name="zh-cn_topic_0020212676_p61818739"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p334014371274"><a name="p334014371274"></a><a name="p334014371274"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0020212676_p41262001"><a name="zh-cn_topic_0020212676_p41262001"></a><a name="zh-cn_topic_0020212676_p41262001"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020212678_row67029240"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p60659387"><a name="zh-cn_topic_0020212678_p60659387"></a><a name="zh-cn_topic_0020212678_p60659387"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020212678_p14463294"><a name="zh-cn_topic_0020212678_p14463294"></a><a name="zh-cn_topic_0020212678_p14463294"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1944051313285"><a name="p1944051313285"></a><a name="p1944051313285"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p30676137"><a name="zh-cn_topic_0020212678_p30676137"></a><a name="zh-cn_topic_0020212678_p30676137"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

## 请求消息<a name="s59fe797a7e2a4811a7b612618c246f91"></a>

>![](public_sys-resources/icon-note.gif) **说明：** 
>创建SSH密钥对时，只需要提交SSH密钥对的name属性。导入SSH密钥对时，才需要提交public\_key属性。

**表 2**  请求参数

<a name="zh-cn_topic_0020212678_table8287277"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212678_row6478825"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p1876964963620"><a name="p1876964963620"></a><a name="p1876964963620"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p1377094912362"><a name="p1377094912362"></a><a name="p1377094912362"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p57701849103612"><a name="p57701849103612"></a><a name="p57701849103612"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p4770154973619"><a name="p4770154973619"></a><a name="p4770154973619"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212678_row20547495"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p53734436"><a name="zh-cn_topic_0020212678_p53734436"></a><a name="zh-cn_topic_0020212678_p53734436"></a>keypair</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020212678_p57522049"><a name="zh-cn_topic_0020212678_p57522049"></a><a name="zh-cn_topic_0020212678_p57522049"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p28774374"><a name="zh-cn_topic_0020212678_p28774374"></a><a name="zh-cn_topic_0020212678_p28774374"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p38553569"><a name="zh-cn_topic_0020212678_p38553569"></a><a name="zh-cn_topic_0020212678_p38553569"></a>创建或导入的SSH密钥对的信息，详情请参见<a href="#zh-cn_topic_0020212678_table54046809">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  keypair字段数据结构说明

<a name="zh-cn_topic_0020212678_table54046809"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212678_row66830726"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p14865165293619"><a name="p14865165293619"></a><a name="p14865165293619"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p986519524366"><a name="p986519524366"></a><a name="p986519524366"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p5865145213366"><a name="p5865145213366"></a><a name="p5865145213366"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p1186615529369"><a name="p1186615529369"></a><a name="p1186615529369"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212678_row4961980"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p66376082"><a name="zh-cn_topic_0020212678_p66376082"></a><a name="zh-cn_topic_0020212678_p66376082"></a>public_key</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020212678_p7753598"><a name="zh-cn_topic_0020212678_p7753598"></a><a name="zh-cn_topic_0020212678_p7753598"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p24061669"><a name="zh-cn_topic_0020212678_p24061669"></a><a name="zh-cn_topic_0020212678_p24061669"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="aa7cbf58553c34a1bb1394f488a812361"><a name="aa7cbf58553c34a1bb1394f488a812361"></a><a name="aa7cbf58553c34a1bb1394f488a812361"></a>导入公钥的字符串信息。</p>
</td>
</tr>
<tr id="rb64458482ea34fba8256588268b8f61a"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p920333685015"><a name="zh-cn_topic_0020212678_p920333685015"></a><a name="zh-cn_topic_0020212678_p920333685015"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="aaf065d906ee04d49824ea3398b2e9066"><a name="aaf065d906ee04d49824ea3398b2e9066"></a><a name="aaf065d906ee04d49824ea3398b2e9066"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="adc06933fad264f229641cd343e894d87"><a name="adc06933fad264f229641cd343e894d87"></a><a name="adc06933fad264f229641cd343e894d87"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="aac79ef19bcec450e82d413e80acaa1fe"><a name="aac79ef19bcec450e82d413e80acaa1fe"></a><a name="aac79ef19bcec450e82d413e80acaa1fe"></a>SSH密钥对的类型，值为ssh或x509。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212678_row28567114"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p32234903"><a name="zh-cn_topic_0020212678_p32234903"></a><a name="zh-cn_topic_0020212678_p32234903"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020212678_p60890369"><a name="zh-cn_topic_0020212678_p60890369"></a><a name="zh-cn_topic_0020212678_p60890369"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p33172847"><a name="zh-cn_topic_0020212678_p33172847"></a><a name="zh-cn_topic_0020212678_p33172847"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p23814811"><a name="zh-cn_topic_0020212678_p23814811"></a><a name="zh-cn_topic_0020212678_p23814811"></a>SSH密钥对的名称。</p>
<p id="aaf6c29e7a36d445a8fba1ef700b79f6c"><a name="aaf6c29e7a36d445a8fba1ef700b79f6c"></a><a name="aaf6c29e7a36d445a8fba1ef700b79f6c"></a>新创建的密钥对名称不能和已有密钥对的名称相同。</p>
<p id="p12841442173714"><a name="p12841442173714"></a><a name="p12841442173714"></a>SSH密钥对名称由英文字母、数字、下划线、中划线组成，长度不能超过64个字节。</p>
</td>
</tr>
<tr id="rb2819f0a6e3f4a068d9bce82febf3b69"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="a55783aa2618640a2a2ad618854f25630"><a name="a55783aa2618640a2a2ad618854f25630"></a><a name="a55783aa2618640a2a2ad618854f25630"></a>user_id</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020212678_p167344512420"><a name="zh-cn_topic_0020212678_p167344512420"></a><a name="zh-cn_topic_0020212678_p167344512420"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="a0de5de4149bd46eebad74ceed05edde9"><a name="a0de5de4149bd46eebad74ceed05edde9"></a><a name="a0de5de4149bd46eebad74ceed05edde9"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="af90ee0d2badc4df5b22cc1a094d5e533"><a name="af90ee0d2badc4df5b22cc1a094d5e533"></a><a name="af90ee0d2badc4df5b22cc1a094d5e533"></a>SSH密钥对的用户ID。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="s0476b99ce1154332bfabc5a0e7cc839c"></a>

**表 4**  响应参数

<a name="zh-cn_topic_0020212678_table51598880"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212678_row44903457"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p470365593616"><a name="p470365593616"></a><a name="p470365593616"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p37039558368"><a name="p37039558368"></a><a name="p37039558368"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p18703125563618"><a name="p18703125563618"></a><a name="p18703125563618"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p87031755193617"><a name="p87031755193617"></a><a name="p87031755193617"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212678_row23474126"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p22356031"><a name="zh-cn_topic_0020212678_p22356031"></a><a name="zh-cn_topic_0020212678_p22356031"></a>keypair</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1376152012815"><a name="p1376152012815"></a><a name="p1376152012815"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1682815315255"><a name="p1682815315255"></a><a name="p1682815315255"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p30540622"><a name="zh-cn_topic_0020212678_p30540622"></a><a name="zh-cn_topic_0020212678_p30540622"></a>SSH密钥对的信息，详情请参见<a href="#zh-cn_topic_0020212678_table51079899">表5</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  keypair字段数据结构说明

<a name="zh-cn_topic_0020212678_table51079899"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212678_row66208776"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p1553445813362"><a name="p1553445813362"></a><a name="p1553445813362"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p20534165816362"><a name="p20534165816362"></a><a name="p20534165816362"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p253518581362"><a name="p253518581362"></a><a name="p253518581362"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p185359582362"><a name="p185359582362"></a><a name="p185359582362"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212678_row27729526"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p31499108"><a name="zh-cn_topic_0020212678_p31499108"></a><a name="zh-cn_topic_0020212678_p31499108"></a>fingerprint</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1040010235289"><a name="p1040010235289"></a><a name="p1040010235289"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p37455857"><a name="zh-cn_topic_0020212678_p37455857"></a><a name="zh-cn_topic_0020212678_p37455857"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p59121255"><a name="zh-cn_topic_0020212678_p59121255"></a><a name="zh-cn_topic_0020212678_p59121255"></a>SSH密钥对对应的指纹信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212678_row62329248"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p15504345"><a name="zh-cn_topic_0020212678_p15504345"></a><a name="zh-cn_topic_0020212678_p15504345"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p2040072392815"><a name="p2040072392815"></a><a name="p2040072392815"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p54079315"><a name="zh-cn_topic_0020212678_p54079315"></a><a name="zh-cn_topic_0020212678_p54079315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p30917775"><a name="zh-cn_topic_0020212678_p30917775"></a><a name="zh-cn_topic_0020212678_p30917775"></a>SSH密钥对的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212678_row9824527"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p57589242"><a name="zh-cn_topic_0020212678_p57589242"></a><a name="zh-cn_topic_0020212678_p57589242"></a>public_key</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p124001123142815"><a name="p124001123142815"></a><a name="p124001123142815"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p20116657"><a name="zh-cn_topic_0020212678_p20116657"></a><a name="zh-cn_topic_0020212678_p20116657"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p35311297"><a name="zh-cn_topic_0020212678_p35311297"></a><a name="zh-cn_topic_0020212678_p35311297"></a>SSH密钥对对应的publicKey信息。</p>
</td>
</tr>
<tr id="r6dc39ac44c8c41ab8d79778b4848dc06"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="a753827ce853b445fb144d9046e61e8d2"><a name="a753827ce853b445fb144d9046e61e8d2"></a><a name="a753827ce853b445fb144d9046e61e8d2"></a>private_key</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p12400423162812"><a name="p12400423162812"></a><a name="p12400423162812"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="a1691134145724a41a26fd126cb9b3abe"><a name="a1691134145724a41a26fd126cb9b3abe"></a><a name="a1691134145724a41a26fd126cb9b3abe"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="aaf44c1f3cdd64aa989b6086292b68ac5"><a name="aaf44c1f3cdd64aa989b6086292b68ac5"></a><a name="aaf44c1f3cdd64aa989b6086292b68ac5"></a>SSH密钥对对应的privateKey信息。</p>
<a name="ue7736e57e6a9425fb14bfeb35458d607"></a><a name="ue7736e57e6a9425fb14bfeb35458d607"></a><ul id="ue7736e57e6a9425fb14bfeb35458d607"><li>创建SSH密钥对时，响应中包括private_key的信息。</li><li>导入SSH密钥对时，响应中不包括private_key的信息。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0020212678_row49366219"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p39240784"><a name="zh-cn_topic_0020212678_p39240784"></a><a name="zh-cn_topic_0020212678_p39240784"></a>user_id</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p84001523202813"><a name="p84001523202813"></a><a name="p84001523202813"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p29185940"><a name="zh-cn_topic_0020212678_p29185940"></a><a name="zh-cn_topic_0020212678_p29185940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p3041091"><a name="zh-cn_topic_0020212678_p3041091"></a><a name="zh-cn_topic_0020212678_p3041091"></a>SSH密钥对所属的用户ID。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section243211314616"></a>

-   创建SSH密钥对
    -   创建SSH密钥对请求样例

        ```
        {     "keypair": {             
                  "type": "ssh",           
                  "name": "demo"              
               }
        }
        ```

    -   创建SSH密钥对响应样例

        ```
        {
            "keypair": {
                "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCyNtFZM04PFxERvZU5OBKTKr3mtRZABe5/+zX81lTgDFCBfq6OXia47M4qXOa3ciBEKKZF+fMfs8U2UNB9aK1R/uORsoEFtxSgZnWG6p4Ct1vnrqwDD934VaDFPEn+h3JeAfvTB+Ag1YQ9zh9uYyE9Z3qZcC9+Ui93BDGdBtQeav4odxdwXcr2mT2jJV0nsocV0O4UcKM8BaIm8eqbcroZEkyxqT3mUoSbmGx1hrngjBsP1ufgwJ6D85LFGQC1SjIOLvsR9i6v41BaLF8/kygvKOh2HlNVSMx38g52sTqoQ/xb3f8vR1VDXliAuD0frrG2Fy5wK4rOAnjuX9nh0bC9 Generated-by-Nova\n",
                "private_key": "-----BEGIN RSA PRIVATE KEY-----\nMIIEpAIBAAKCAQEAsjbRWTNODxcREb2VOTgSkyq95rUWQAXuf/s1/NZU4AxQgX6u\njl4muOzOKlzmt3IgRCimRfnzH7PFNlDQfWitUf7jkbKBBbcUoGZ1huqeArdb566s\nAw/d+FWgxTxJ/odyXgH70wfgINWEPc4fbmMhPWd6mXAvflIvdwQxnQbUHmr+KHcX\ncF3K9pk9oyVdJ7KHFdDuFHCjPAWiJvHqm3K6GRJMsak95lKEm5hsdYa54IwbD9bn\n4MCeg/OSxRkAtUoyDi77EfYur+NQWixfP5MoLyjodh5TVUjMd/IOdrE6qEP8W93/\nL0dVQ15YgLg9H66xthcucCuKzgJ47l/Z4dGwvQIDAQABAoIBAQCdTjXL/rVQLJQs\njKNDNnNu47NsCTvyl0nGPf+Rhb61ZSlKpH9/uyuC38O7MPWVx28jup3J9q7btNrG\n7t6ZU+RpFAvbdyzb1pamXsoupLmEvESrZEsBCOhtY2fdsTG/Md+Ji0a1J6Z2VQG9\nbEviLC4S/VwCRDwnzHOJInKIoJZroZv6SdK+KonQBS0Rq9bZrlvtBUUhaSGjBcJx\nmWKO78ikNOXP/5Yl92SAw2vOYWhZdMZQrkp1EUFMG18Akuj+jC9QKXXfsLYYfzsQ\nIGgpRdf6zYIV84QVMZ7NhQABM5DNmQfxrSIUSdbvOzOJzmShp41tH3sn9d+XS+bS\nLIoyuaQhAoGBAN7tpwgkcKddKI/Lp/CPqjkxP6lfO+xHEXjtnZd1Y//BavPSgq4v\nWuFHgx1sPQK49KcSLZfF6UxkPw0KHBc5R9RkfYBAIdGNwENF2xyoYLLdnUtF4hRq\n1q2DC3oklBZibH2tc6+hQ2aCWSeMvQbIvxTYV70EFzwR5f4O5LIskCm/AoGBAMyn\nA7DOQdvcf4aexSYL4kGp70ERMOCtwr/d+O5RswARoyAQOxp4a7/TyFuGjnlT//bR\nEYacXV1AieIdeJF3PgeUIR1QnUlNYD9Rufs14fs+5idQ7Evn1gvXv0HpBYTY7wNu\nWTrWbsznY0fNIrGT4bQR6QpdvIuR5TBJf6HIAKyDAoGAFhKf3D2HbfraXkqC6V3A\nNAN9Uy7bxwxOXZPha7Ky4QrspRGt4MNNk0q6X7ps3A0mJDi3jPSKoga2+3qJx37j\nbtM4Xe97qb0IUWDkThUZ5fvtbBuSRAVEFlAIXeKrSwAZz+PRtY0ZGFhFrZXQzZAo\n4058eXmjN05qYFpnKIEjEQ8CgYEAwELzW6oaAzR+dfk428p0UB4W0HkXAy0a9efS\nUgpc8Oag6qF09SRGjdunshySQvegU78MCPtjVxUntE7dk0OD+di213SBn3jawAHG\niHORjtkDndIPfCwcUdnpK0GAVtL6kK2dlIIZa9TB15WnT07Pzry4w21WkYSJ3Thf\neJyNzYMCgYA8OvpKMdaEXFeNZWHDE1Q2VmpxvP/D6u6s4SBuyy8eac1qqku/s7zc\nsuFd/o9wbBgzsf4eN8tNJ4bxrArRXvf9WyH7xd4PE3DvVJnz5S+8Nqj2Z0KCAqPD\nibDbFxBYHcMIdwC2JBGQZIXpkST2jG9wZho5KghX4yiHSOPr2V25/g==\n-----END RSA PRIVATE KEY-----\n",
                "user_id": "6fc0d2cbbfab40b199874b97097e913d",
                "name": "demo",
                "fingerprint": "b4:9a:c3:12:c4:90:bf:8e:7a:e2:70:10:c3:00:55:3f"
           }
        }
        ```

-   导入SSH密钥对
    -   导入SSH密钥对请求样例

        ```
        {
            "keypair": {
                "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCyNtFZM04PFxERvZU5OBKTKr3mtRZABe5/+zX81lTgDFCBfq6OXia47M4qXOa3ciBEKKZF+fMfs8U2UNB9aK1R/uORsoEFtxSgZnWG6p4Ct1vnrqwDD934VaDFPEn+h3JeAfvTB+Ag1YQ9zh9uYyE9Z3qZcC9+Ui93BDGdBtQeav4odxdwXcr2mT2jJV0nsocV0O4UcKM8BaIm8eqbcroZEkyxqT3mUoSbmGx1hrngjBsP1ufgwJ6D85LFGQC1SjIOLvsR9i6v41BaLF8/kygvKOh2HlNVSMx38g52sTqoQ/xb3f8vR1VDXliAuD0frrG2Fy5wK4rOAnjuX9nh0bC9 Generated-by-Nova\n",
                "type": "ssh",
                "name": "demo1"，
                "user_id": "fake"
            }
        }
        ```

    -   导入SSH密钥对响应样例

        ```
        {
            "keypair": {
                "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCyNtFZM04PFxERvZU5OBKTKr3mtRZABe5/+zX81lTgDFCBfq6OXia47M4qXOa3ciBEKKZF+fMfs8U2UNB9aK1R/uORsoEFtxSgZnWG6p4Ct1vnrqwDD934VaDFPEn+h3JeAfvTB+Ag1YQ9zh9uYyE9Z3qZcC9+Ui93BDGdBtQeav4odxdwXcr2mT2jJV0nsocV0O4UcKM8BaIm8eqbcroZEkyxqT3mUoSbmGx1hrngjBsP1ufgwJ6D85LFGQC1SjIOLvsR9i6v41BaLF8/kygvKOh2HlNVSMx38g52sTqoQ/xb3f8vR1VDXliAuD0frrG2Fy5wK4rOAnjuX9nh0bC9 Generated-by-Nova\n",
                "user_id": "6fc0d2cbbfab40b199874b97097e913d",
                "name": "demo1",
                "fingerprint": "b4:9a:c3:12:c4:90:bf:8e:7a:e2:70:10:c3:00:55:3f"
            }
        }
        ```

## 状态码<a name="s5d8cc52233f84ca9ad1f774ec90fa861"></a>

请参考[状态码](状态码.md)。

