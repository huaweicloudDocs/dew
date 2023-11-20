# 创建及导入SSH密钥对\(V2.1\)<a name="dew_02_0210"></a>

## 功能介绍<a name="s306004e5a98e4283a1bfcb4adc2fa508"></a>

创建SSH密钥对和导入SSH密钥对，同时可选择对私钥进行托管。

## URI<a name="sbbff16336947456f8342473caef444e2"></a>

-   URI格式

    POST /v2.1/\{project\_id\}/os-keypairs

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
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1457924222918"><a name="p1457924222918"></a><a name="p1457924222918"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="acf1687032c074bd0bd72b8b9b1fa31dc"><a name="acf1687032c074bd0bd72b8b9b1fa31dc"></a><a name="acf1687032c074bd0bd72b8b9b1fa31dc"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

## 请求消息<a name="s59fe797a7e2a4811a7b612618c246f91"></a>

>![](public_sys-resources/icon-note.gif) **说明：** 
>创建SSH密钥对时，只需要提交SSH密钥对的name属性。导入SSH密钥对时，才需要提交public\_key属性。

**表 2**  请求参数

<a name="zh-cn_topic_0020212678_table8287277"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212678_row6478825"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p1681882143815"><a name="p1681882143815"></a><a name="p1681882143815"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p12818132143817"><a name="p12818132143817"></a><a name="p12818132143817"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p7818122103814"><a name="p7818122103814"></a><a name="p7818122103814"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p281818211381"><a name="p281818211381"></a><a name="p281818211381"></a>描述</p>
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
<table><thead align="left"><tr id="zh-cn_topic_0020212678_row66830726"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p493702483820"><a name="p493702483820"></a><a name="p493702483820"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p1193712453812"><a name="p1193712453812"></a><a name="p1193712453812"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p1693716247383"><a name="p1693716247383"></a><a name="p1693716247383"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p1493732416387"><a name="p1493732416387"></a><a name="p1493732416387"></a>描述</p>
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
<tr id="row3982695410434"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p475781310434"><a name="p475781310434"></a><a name="p475781310434"></a>key_protection</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p4983857710434"><a name="p4983857710434"></a><a name="p4983857710434"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1039293310434"><a name="p1039293310434"></a><a name="p1039293310434"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p3652127410434"><a name="p3652127410434"></a><a name="p3652127410434"></a>SSH密钥对私钥托管与保护，详情请参见<a href="#table3936358110540">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  key\_protection字段数据结构说明

<a name="table3936358110540"></a>
<table><thead align="left"><tr id="row6664497910540"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p52221530143811"><a name="p52221530143811"></a><a name="p52221530143811"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p222219305389"><a name="p222219305389"></a><a name="p222219305389"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p18222430173816"><a name="p18222430173816"></a><a name="p18222430173816"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p8222173013383"><a name="p8222173013383"></a><a name="p8222173013383"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2833105410540"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p1311403710540"><a name="p1311403710540"></a><a name="p1311403710540"></a>private_key</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p5560406810540"><a name="p5560406810540"></a><a name="p5560406810540"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p763568410540"><a name="p763568410540"></a><a name="p763568410540"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p1451068510540"><a name="p1451068510540"></a><a name="p1451068510540"></a>导入私钥的字符串信息。</p>
</td>
</tr>
<tr id="row4667257410540"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p2238216210540"><a name="p2238216210540"></a><a name="p2238216210540"></a>encryption</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p101579710540"><a name="p101579710540"></a><a name="p101579710540"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p1517077010540"><a name="p1517077010540"></a><a name="p1517077010540"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p1297902810540"><a name="p1297902810540"></a><a name="p1297902810540"></a>对私钥进行加密存储的方式，详情请参见<a href="#table5307550110915">表5</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  encryption字段数据结构说明

<a name="table5307550110915"></a>
<table><thead align="left"><tr id="row839866710915"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p2013163414386"><a name="p2013163414386"></a><a name="p2013163414386"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p121311034153812"><a name="p121311034153812"></a><a name="p121311034153812"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p1213110341383"><a name="p1213110341383"></a><a name="p1213110341383"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p12131734143814"><a name="p12131734143814"></a><a name="p12131734143814"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row3660975910915"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p1260047510915"><a name="p1260047510915"></a><a name="p1260047510915"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p2338574291658"><a name="p2338574291658"></a><a name="p2338574291658"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p6071023410915"><a name="p6071023410915"></a><a name="p6071023410915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p2004648591759"><a name="p2004648591759"></a><a name="p2004648591759"></a>取值范围：<span class="parmvalue" id="parmvalue179180397338"><a name="parmvalue179180397338"></a><a name="parmvalue179180397338"></a>“kms”</span>或<span class="parmvalue" id="parmvalue3614204233315"><a name="parmvalue3614204233315"></a><a name="parmvalue3614204233315"></a>“default”</span>。</p>
<a name="ul116618499332"></a><a name="ul116618499332"></a><ul id="ul116618499332"><li><span class="parmvalue" id="parmvalue7661184993312"><a name="parmvalue7661184993312"></a><a name="parmvalue7661184993312"></a>“default”</span>为默认加密方式，适用于没有kms服务的局点。</li><li><span class="parmvalue" id="parmvalue46619498333"><a name="parmvalue46619498333"></a><a name="parmvalue46619498333"></a>“kms”</span>为采用kms服务加密方式。</li></ul>
<p id="p28062377164132"><a name="p28062377164132"></a><a name="p28062377164132"></a>若局点没有kms服务，请填<span class="parmvalue" id="parmvalue3988161818333"><a name="parmvalue3988161818333"></a><a name="parmvalue3988161818333"></a>“default”</span>。</p>
</td>
</tr>
<tr id="row3301966710915"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p5734733410915"><a name="p5734733410915"></a><a name="p5734733410915"></a>kms_key_name</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1462251510915"><a name="p1462251510915"></a><a name="p1462251510915"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="p4357305610915"><a name="p4357305610915"></a><a name="p4357305610915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p26163296164312"><a name="p26163296164312"></a><a name="p26163296164312"></a>kms密钥的名称。</p>
<p id="p34143078164312"><a name="p34143078164312"></a><a name="p34143078164312"></a>若<span class="parmname" id="parmname1318535717333"><a name="parmname1318535717333"></a><a name="parmname1318535717333"></a>“type”</span>为<span class="parmvalue" id="parmvalue1252845920336"><a name="parmvalue1252845920336"></a><a name="parmvalue1252845920336"></a>“kms”</span>，则必须填入kms服务密钥名称。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="s0476b99ce1154332bfabc5a0e7cc839c"></a>

**表 6**  响应参数

<a name="zh-cn_topic_0020212678_table51598880"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212678_row44903457"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p125801537103816"><a name="p125801537103816"></a><a name="p125801537103816"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p11580123733817"><a name="p11580123733817"></a><a name="p11580123733817"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p185801937113819"><a name="p185801937113819"></a><a name="p185801937113819"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p105801375388"><a name="p105801375388"></a><a name="p105801375388"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212678_row23474126"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p22356031"><a name="zh-cn_topic_0020212678_p22356031"></a><a name="zh-cn_topic_0020212678_p22356031"></a>keypair</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p19225014294"><a name="p19225014294"></a><a name="p19225014294"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p45057304"><a name="zh-cn_topic_0020212678_p45057304"></a><a name="zh-cn_topic_0020212678_p45057304"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p30540622"><a name="zh-cn_topic_0020212678_p30540622"></a><a name="zh-cn_topic_0020212678_p30540622"></a>SSH密钥对的信息，详情请参见<a href="#zh-cn_topic_0020212678_table51079899">表7</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 7**  keypair字段数据结构说明

<a name="zh-cn_topic_0020212678_table51079899"></a>
<table><thead align="left"><tr id="zh-cn_topic_0020212678_row66208776"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p198331940123814"><a name="p198331940123814"></a><a name="p198331940123814"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p983414014385"><a name="p983414014385"></a><a name="p983414014385"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.3"><p id="p483420400386"><a name="p483420400386"></a><a name="p483420400386"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p483434015389"><a name="p483434015389"></a><a name="p483434015389"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0020212678_row27729526"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p31499108"><a name="zh-cn_topic_0020212678_p31499108"></a><a name="zh-cn_topic_0020212678_p31499108"></a>fingerprint</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p20332135422913"><a name="p20332135422913"></a><a name="p20332135422913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p37455857"><a name="zh-cn_topic_0020212678_p37455857"></a><a name="zh-cn_topic_0020212678_p37455857"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p59121255"><a name="zh-cn_topic_0020212678_p59121255"></a><a name="zh-cn_topic_0020212678_p59121255"></a>SSH密钥对对应的指纹信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212678_row62329248"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p15504345"><a name="zh-cn_topic_0020212678_p15504345"></a><a name="zh-cn_topic_0020212678_p15504345"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1333213546296"><a name="p1333213546296"></a><a name="p1333213546296"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p54079315"><a name="zh-cn_topic_0020212678_p54079315"></a><a name="zh-cn_topic_0020212678_p54079315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p30917775"><a name="zh-cn_topic_0020212678_p30917775"></a><a name="zh-cn_topic_0020212678_p30917775"></a>SSH密钥对的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0020212678_row9824527"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p57589242"><a name="zh-cn_topic_0020212678_p57589242"></a><a name="zh-cn_topic_0020212678_p57589242"></a>public_key</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p83321154152912"><a name="p83321154152912"></a><a name="p83321154152912"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p20116657"><a name="zh-cn_topic_0020212678_p20116657"></a><a name="zh-cn_topic_0020212678_p20116657"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p35311297"><a name="zh-cn_topic_0020212678_p35311297"></a><a name="zh-cn_topic_0020212678_p35311297"></a>SSH密钥对对应的publicKey信息。</p>
</td>
</tr>
<tr id="r6dc39ac44c8c41ab8d79778b4848dc06"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="a753827ce853b445fb144d9046e61e8d2"><a name="a753827ce853b445fb144d9046e61e8d2"></a><a name="a753827ce853b445fb144d9046e61e8d2"></a>private_key</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1533295462918"><a name="p1533295462918"></a><a name="p1533295462918"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="a1691134145724a41a26fd126cb9b3abe"><a name="a1691134145724a41a26fd126cb9b3abe"></a><a name="a1691134145724a41a26fd126cb9b3abe"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="aaf44c1f3cdd64aa989b6086292b68ac5"><a name="aaf44c1f3cdd64aa989b6086292b68ac5"></a><a name="aaf44c1f3cdd64aa989b6086292b68ac5"></a>SSH密钥对对应的privateKey信息。</p>
<a name="ue7736e57e6a9425fb14bfeb35458d607"></a><a name="ue7736e57e6a9425fb14bfeb35458d607"></a><ul id="ue7736e57e6a9425fb14bfeb35458d607"><li>创建SSH密钥对时，响应中包括private_key的信息。</li><li>导入SSH密钥对时，响应中不包括private_key的信息。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0020212678_row49366219"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020212678_p39240784"><a name="zh-cn_topic_0020212678_p39240784"></a><a name="zh-cn_topic_0020212678_p39240784"></a>user_id</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p14332125482916"><a name="p14332125482916"></a><a name="p14332125482916"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020212678_p29185940"><a name="zh-cn_topic_0020212678_p29185940"></a><a name="zh-cn_topic_0020212678_p29185940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020212678_p3041091"><a name="zh-cn_topic_0020212678_p3041091"></a><a name="zh-cn_topic_0020212678_p3041091"></a>SSH密钥对所属的用户ID。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="sa2cfd6b2f5f34f879f1e1a21f8123f29"></a>

-   创建SSH密钥对
    -   创建SSH密钥对请求样例

        ```
        {
            "keypair": {
                "name": "demo1"
            }
        }
        ```

    -   创建SSH密钥对响应样例

        ```
        {
            "keypair": {
                "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCXKzohKbFOqubYNunFNsrEYlk9NEIJIFvbmTe/LTeMzFIPKM53Zu2sYr/uuNcziPkWpFchXdkD+O/Bf2ZzKaR1DYPMWss9TkaqU4RQ7CIBW7ChJF1Qzc1JPRBmKe6e8qs1QBBoS1QvXgSjbuf2Fb1yncSbphmQV8+5KA8xkxz4XdM1/gSAZZ14rJrMjgp7jCdgxWiHNcDuKxaPt+0eO8rEG/gxR7J0b9Uk53ao/xjLoKXYdLLiYUaha0fHdW3t6Lw1NdzUMmKnlLqN9O37Tbg7vM0nN4UJt0XXvM45KfnJiMx0HUKXdWkUj9cE8VBDPw/gBbQzSpJHgQFG7mNDZubN Generated-by-Nova\n",
                "private_key": "-----BEGIN RSA PRIVATE KEY-----\nMIIEowIBAAKCAQEAlys6ISmxTqrm2DbpxTbKxGJZPTRCCSBb25k3vy03jMxSDyjO\nd2btrGK/7rjXM4j5FqRXIV3ZA/jvwX9mcymkdQ2DzFrLPU5GqlOEUOwiAVuwoSRd\nUM3NST0QZinunvKrNUAQaEtUL14Eo27n9hW9cp3Em6YZkFfPuSgPMZMc+F3TNf4E\ngGWdeKyazI4Ke4wnYMVohzXA7isWj7ftHjvKxBv4MUeydG/VJOd2qP8Yy6Cl2HSy\n4mFGoWtHx3Vt7ei8NTXc1DJip5S6jfTt+024O7zNJzeFCbdF17zOOSn5yYjMdB1C\nl3VpFI/XBPFQQz8P4AW0M0qSR4EBRu5jQ2bmzQIDAQABAoIBAFwm1s3Gi7bICec+\nOm2lhCAJUBs2UxcbKcQJd+lL2DQ1jcR9/LbfAP34SMZu2Ykp86Zw0kid3CBGzWko\nj7yeYwmUDocxxfl+USedt+hYujYXvenNsDEE9CK0Xd3ZrAQrLGFOx3G8kfo6FxvG\nDRN/lzhaorK7o5PRY+icWf6/joZ8Q96scHmm0ob5rtBkUYcek+ckf3mLVIpzzdKA\ndkSi57M78zwDA89MpVABEoO1DPVxEqrrMQZy5UnAmeGHh16mPS4qMCokPVz36pSG\nIWSqHnVKzsbxvw5Da9y69NmpSi2E1wqDaU9IzwnLyQpHnE1nXsWmxNqKTHlDBbnb\nXPGFdcECgYEAxf4IMqYBeBiq+7RVwcTcT4gpApJmywigwMFaaX35E3O53ja8hk1/\n5OCRnvK7yrt9wnWY8DIh8GPJptKzuTb/l/14L4kE1MYm7Gpho5SwXV5BqtjgjfZm\nQVNpWruXEugXALcfbHiH+peO+3AmwgIqgkOLPLxY1Duw6/miDB8bOfECgYEAw3VO\nl9edXExJvJvSzAopSNmw+ExpUZTgS3L2Pyn21QhfwNHyxPH8fNNKv0/x9ZzBn25U\nUxXTPPbLFV3cq7kfuYFW0OZkh8QjCPDkIE116E2QvacxqkBuW774xr5msfWdxpcp\nwccgWKci1vEHLtqj3RTNMFKcXtj4QrCES4ZsPp0CgYEAhzYYux4LWszd188r0Yxz\nOA0wlIUOlhFqVri02d4hv1sEz/Bphv5eHRwP1pDGFok8NRTCQSa7bsN27uptuksI\n+e8rqKrWFcjMxB9SVrgwSVMZXWeG0uw2oN4p0MDTRyIgs2hbmWQm2Mev6Z6JmWyJ\nQzSFXhDySN4K0NxGAiksGsECgYAJvZTXGFWtPdgG4DUXGgKIsOCS3yv4dtTerbH7\n39l/MFWlRFE242BT0CvPcOp79P3pNhRZt6K5TQs921md7THZisqKypCD+5BLZ8XW\nnkWb+BGYgfaFp4RYaiH3tZFkmPrt5KaeE5BXGq0vzP8wpJC5+cln+RX13BYzLJzL\nLr3COQKBgDJjY0qop3aSG+1tSkMJtOFdb2+qXiqaE+Wxv03SOkPx8LBz+taNz+DE\nR7THDNXSrS85WVc3ozE8hULBX12iIWpr5kb5lRaw3ZgX6wBnSSpdQu49v3nFoGJk\nUWY95pQ/BWQaX0q4KxzRVxup+7gwT5sKFXU+ktFtsGMYoDoSzbZS\n-----END RSA PRIVATE KEY-----\n",
                "user_id": "e4f380899b1248918f3d37098dc63746",
                "name": "demo123",
                "fingerprint": "49:ef:73:2b:9b:7f:2e:0c:58:d3:e3:42:8e:28:04:3b"
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

-   创建SSH密钥对并托管私钥
    -   创建SSH密钥对并托管私钥请求样例

        ```
        {
            "keypair": {
                "name": "demo2",
                "key_protection": {
                    "encryption": {
                        "type": "kms",
                        "kms_key_name": "demo"
                    }
                }
            }
        }
        ```

    -   创建SSH密钥对并托管私钥响应样例

        ```
        {
            "keypair": {
                "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCXKzohKbFOqubYNunFNsrEYlk9NEIJIFvbmTe/LTeMzFIPKM53Zu2sYr/uuNcziPkWpFchXdkD+O/Bf2ZzKaR1DYPMWss9TkaqU4RQ7CIBW7ChJF1Qzc1JPRBmKe6e8qs1QBBoS1QvXgSjbuf2Fb1yncSbphmQV8+5KA8xkxz4XdM1/gSAZZ14rJrMjgp7jCdgxWiHNcDuKxaPt+0eO8rEG/gxR7J0b9Uk53ao/xjLoKXYdLLiYUaha0fHdW3t6Lw1NdzUMmKnlLqN9O37Tbg7vM0nN4UJt0XXvM45KfnJiMx0HUKXdWkUj9cE8VBDPw/gBbQzSpJHgQFG7mNDZubN Generated-by-Nova\n",
                "private_key": "-----BEGIN RSA PRIVATE KEY-----\nMIIEowIBAAKCAQEAlys6ISmxTqrm2DbpxTbKxGJZPTRCCSBb25k3vy03jMxSDyjO\nd2btrGK/7rjXM4j5FqRXIV3ZA/jvwX9mcymkdQ2DzFrLPU5GqlOEUOwiAVuwoSRd\nUM3NST0QZinunvKrNUAQaEtUL14Eo27n9hW9cp3Em6YZkFfPuSgPMZMc+F3TNf4E\ngGWdeKyazI4Ke4wnYMVohzXA7isWj7ftHjvKxBv4MUeydG/VJOd2qP8Yy6Cl2HSy\n4mFGoWtHx3Vt7ei8NTXc1DJip5S6jfTt+024O7zNJzeFCbdF17zOOSn5yYjMdB1C\nl3VpFI/XBPFQQz8P4AW0M0qSR4EBRu5jQ2bmzQIDAQABAoIBAFwm1s3Gi7bICec+\nOm2lhCAJUBs2UxcbKcQJd+lL2DQ1jcR9/LbfAP34SMZu2Ykp86Zw0kid3CBGzWko\nj7yeYwmUDocxxfl+USedt+hYujYXvenNsDEE9CK0Xd3ZrAQrLGFOx3G8kfo6FxvG\nDRN/lzhaorK7o5PRY+icWf6/joZ8Q96scHmm0ob5rtBkUYcek+ckf3mLVIpzzdKA\ndkSi57M78zwDA89MpVABEoO1DPVxEqrrMQZy5UnAmeGHh16mPS4qMCokPVz36pSG\nIWSqHnVKzsbxvw5Da9y69NmpSi2E1wqDaU9IzwnLyQpHnE1nXsWmxNqKTHlDBbnb\nXPGFdcECgYEAxf4IMqYBeBiq+7RVwcTcT4gpApJmywigwMFaaX35E3O53ja8hk1/\n5OCRnvK7yrt9wnWY8DIh8GPJptKzuTb/l/14L4kE1MYm7Gpho5SwXV5BqtjgjfZm\nQVNpWruXEugXALcfbHiH+peO+3AmwgIqgkOLPLxY1Duw6/miDB8bOfECgYEAw3VO\nl9edXExJvJvSzAopSNmw+ExpUZTgS3L2Pyn21QhfwNHyxPH8fNNKv0/x9ZzBn25U\nUxXTPPbLFV3cq7kfuYFW0OZkh8QjCPDkIE116E2QvacxqkBuW774xr5msfWdxpcp\nwccgWKci1vEHLtqj3RTNMFKcXtj4QrCES4ZsPp0CgYEAhzYYux4LWszd188r0Yxz\nOA0wlIUOlhFqVri02d4hv1sEz/Bphv5eHRwP1pDGFok8NRTCQSa7bsN27uptuksI\n+e8rqKrWFcjMxB9SVrgwSVMZXWeG0uw2oN4p0MDTRyIgs2hbmWQm2Mev6Z6JmWyJ\nQzSFXhDySN4K0NxGAiksGsECgYAJvZTXGFWtPdgG4DUXGgKIsOCS3yv4dtTerbH7\n39l/MFWlRFE242BT0CvPcOp79P3pNhRZt6K5TQs921md7THZisqKypCD+5BLZ8XW\nnkWb+BGYgfaFp4RYaiH3tZFkmPrt5KaeE5BXGq0vzP8wpJC5+cln+RX13BYzLJzL\nLr3COQKBgDJjY0qop3aSG+1tSkMJtOFdb2+qXiqaE+Wxv03SOkPx8LBz+taNz+DE\nR7THDNXSrS85WVc3ozE8hULBX12iIWpr5kb5lRaw3ZgX6wBnSSpdQu49v3nFoGJk\nUWY95pQ/BWQaX0q4KxzRVxup+7gwT5sKFXU+ktFtsGMYoDoSzbZS\n-----END RSA PRIVATE KEY-----\n",
                "user_id": "e4f380899b1248918f3d37098dc63746",
                "name": "demo123",
                "fingerprint": "49:ef:73:2b:9b:7f:2e:0c:58:d3:e3:42:8e:28:04:3b"
            }
        }
        ```

-   导入SSH密钥对公钥
    -   导入SSH密钥对公钥请求样例

        ```
        {
            "keypair": {
                "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCyNtFZM04PFxERvZU5OBKTKr3mtRZABe5/+zX81lTgDFCBfq6OXia47M4qXOa3ciBEKKZF+fMfs8U2UNB9aK1R/uORsoEFtxSgZnWG6p4Ct1vnrqwDD934VaDFPEn+h3JeAfvTB+Ag1YQ9zh9uYyE9Z3qZcC9+Ui93BDGdBtQeav4odxdwXcr2mT2jJV0nsocV0O4UcKM8BaIm8eqbcroZEkyxqT3mUoSbmGx1hrngjBsP1ufgwJ6D85LFGQC1SjIOLvsR9i6v41BaLF8/kygvKOh2HlNVSMx38g52sTqoQ/xb3f8vR1VDXliAuD0frrG2Fy5wK4rOAnjuX9nh0bC9 Generated-by-Nova\n",
                "name": "demo3"
            }
        }
        ```

    -   导入SSH密钥对公钥响应样例

        ```
        {
            "keypair": {
                "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCyNtFZM04PFxERvZU5OBKTKr3mtRZABe5/+zX81lTgDFCBfq6OXia47M4qXOa3ciBEKKZF+fMfs8U2UNB9aK1R/uORsoEFtxSgZnWG6p4Ct1vnrqwDD934VaDFPEn+h3JeAfvTB+Ag1YQ9zh9uYyE9Z3qZcC9+Ui93BDGdBtQeav4odxdwXcr2mT2jJV0nsocV0O4UcKM8BaIm8eqbcroZEkyxqT3mUoSbmGx1hrngjBsP1ufgwJ6D85LFGQC1SjIOLvsR9i6v41BaLF8/kygvKOh2HlNVSMx38g52sTqoQ/xb3f8vR1VDXliAuD0frrG2Fy5wK4rOAnjuX9nh0bC9 Generated-by-Nova\n",
                "user_id": "e4f380899b1248918f3d37098dc63746",
                "name": "demo1",
                "fingerprint": "b4:9a:c3:12:c4:90:bf:8e:7a:e2:70:10:c3:00:55:3f"
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

-   导入SSH密钥对公钥并托管私钥
    -   导入SSH密钥对公钥并托管私钥请求样例

        ```
        {
            "keypair": {
                "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDb26UrW0htRbE/Ygf8EPhzanBCc+5yEhkgmeSb2hTe48YRE5FdJKH6tueyj+vw5guoKjAITLjqZCqffGYXz/7aXpFt244b9tTzh2l43uNtEZC+XZtc6KiBgfWupFI8O2i9YjJqdadsr+4Ad4AtIBbF++qsSJN4YycPX//Gl8ja6AGPy4sdv8DZ40Gr8d+dMQ4pAsnUEtZ3jJ6NLdQU2CE1JhBdg3hbVbeh44gqQtSjhxWaSTlr+NbVxSERtXXpsQWsid6qM1RhqH2+02cqXq5oNs4JLdu56pcTgSO5azTsGYJi6j5qp5BAdjMrFtHjbaeVVWtkO1XQxfpueCJ470lx Generated-by-Nova\n",
                "name": "demo4",
                "key_protection": {
                    "private_key": "-----BEGIN RSA PRIVATE KEY-----\nMIIEpQIBAAKCAQEA29ulK1tIbUWxP2IH/BD4c2pwQnPuchIZIJnkm9oU3uPGEROR\nXSSh+rbnso/r8OYLqCowCEy46mQqn3xmF8/+2l6RbduOG/bU84dpeN7jbRGQvl2b\nXOiogYH1rqRSPDtovWIyanWnbK/uAHeALSAWxfvqrEiTeGMnD1//xpfI2ugBj8uL\nHb/A2eNBq/HfnTEOKQLJ1BLWd4yejS3UFNghNSYQXYN4W1W3oeOIKkLUo4cVmkk5\na/jW1cUhEbV16bEFrIneqjNUYah9vtNnKl6uaDbOCS3bueqXE4EjuWs07BmCYuo+\naqeQQHYzKxbR422nlVVrZDtV0MX6bngieO9JcQIDAQABAoIBAAVSEXM1KFGMqDdy\ndeMBviF85+6Tw6d7DKSfVMr4whyKwpZTNOdeJZVdq8nEdd9Eke+l5bets6PofKeT\naR0WaYJ7W2WfNJc0p/6kvkawjixrimcw+LuM3dcUgA+T5nGStnwuzi2JX13f/BCC\n09VDu4lbCVjWAMufCqjyl8wEjFXP0Amhu8fpDvqHuhGvDkoVWRm9vDEeyz71P25K\n/UUs7kXw5Qv0VRcm15b+2jO6tii3RTo+JaTvkYXoI/qrOjiQhQD88geiOPQVuffa\nzJhDw4/2GdHaCwEN6mzwKCYCfcPTRbM503F1YlceiP9w2qScToao+5B2okN9cIE8\nTV4vmIkCgYEA+vo/TKqFep2D6DPY3dNRu2bHIYikBMtYMCIKJ1bgQ1xS/FjEJfSj\notdDcBEik+0VEV05BCHNduTiMt6rTUD9fpqDduV8PfsskAAZZjndbyUEGP/KrCvS\nJsd2BFa2G7In/3wz3zw+3P77Aegb+zHJfDyqYWReNkYy5tSsaZ9Oz38CgYEA4EH5\nIXQPhJt9683JmK/INiyhW6WqKOAZkvjKpUpdUpGdVHJI/9dfUYI9wxnybgAkOZVL\noErxMTdRCDev8nVAq/OwC/4jI5YnBGkN3ZRxIkCrepzwxIXgWeJiwWqsvdDbosfM\nN0Q6PvUnPTXEly8RGcH9ABTQvQ9Nq4rQyjQvXw8CgYEAuK8hmWb55iq3AE32zfVM\n9ZxB+Jk2KRkBghnqYtx5Fth/cJZZcJy/NXs2cucJDNWvZSG2bSX6rfzrvwdAAw9J\n+rn0968TaADG4AhSqHj4S2tvwn2oRF3SvRqV68drJqJI8KYS/bi1gaZYSyTkQkp2\nu+dgcV6MPWAW4OmrHeZO9j0CgYEAkY8Az4/vipkKkIWP9oUSJOevDDdpTQK4VscZ\ncVPlYvSU8/0CGN2IRvWMdRhgXLnGyYF4BuDd0J4hAH50u6ETiwivGfmogS6ywJAX\nqdzx2dOz+e/n7wceafkhNH2zBbmM9glNKgok7DxfbcF6is7IALoDJ4xbOHu4ZEHD\n55sbrE0CgYEAuOuiISgfbujENFFPW0nvUmNqbkAH5YW1oUIWYA+64z7wcWyvzxRS\nYml2XLWyrJy3JNzHpLoe4mCBxz+HGrftZ0/qfQ/WDZrY/Djp7/xIkPyI9EwsRTYC\nr1PtWvVws3y3hgdo6WVQMaeUqtLSiTugyuuPqidH+/QtwxObunNH6Ns=\n-----END RSA PRIVATE KEY-----\n",
                    "encryption": {
                        "type": "kms",
                        "kms_key_name": "testName"
                    }
                }
            }
        }
        ```

    -   导入SSH密钥对公钥并托管私钥响应样例

        ```
        {
            "keypair": {
                "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCyNtFZM04PFxERvZU5OBKTKr3mtRZABe5/+zX81lTgDFCBfq6OXia47M4qXOa3ciBEKKZF+fMfs8U2UNB9aK1R/uORsoEFtxSgZnWG6p4Ct1vnrqwDD934VaDFPEn+h3JeAfvTB+Ag1YQ9zh9uYyE9Z3qZcC9+Ui93BDGdBtQeav4odxdwXcr2mT2jJV0nsocV0O4UcKM8BaIm8eqbcroZEkyxqT3mUoSbmGx1hrngjBsP1ufgwJ6D85LFGQC1SjIOLvsR9i6v41BaLF8/kygvKOh2HlNVSMx38g52sTqoQ/xb3f8vR1VDXliAuD0frrG2Fy5wK4rOAnjuX9nh0bC9 Generated-by-Nova\n",
                "user_id": "e4f380899b1248918f3d37098dc63746",
                "name": "demo1",
                "fingerprint": "b4:9a:c3:12:c4:90:bf:8e:7a:e2:70:10:c3:00:55:3f"
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

