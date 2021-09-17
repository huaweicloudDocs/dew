# API概览<a name="dew_02_0057"></a>

数据加密服务提供的接口，您可以完整的使用数据加密服务的所有功能。

<a name="table1577981717153"></a>
<table><thead align="left"><tr id="row16810121712155"><th class="cellrowborder" valign="top" width="25.929999999999996%" id="mcps1.1.3.1.1"><p id="p13834717131516"><a name="p13834717131516"></a><a name="p13834717131516"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="74.07000000000001%" id="mcps1.1.3.1.2"><p id="p3883151714159"><a name="p3883151714159"></a><a name="p3883151714159"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2054614267164"><td class="cellrowborder" valign="top" width="25.929999999999996%" headers="mcps1.1.3.1.1 "><p id="p14546162641618"><a name="p14546162641618"></a><a name="p14546162641618"></a>管理加密密钥</p>
</td>
<td class="cellrowborder" valign="top" width="74.07000000000001%" headers="mcps1.1.3.1.2 "><p id="p565181993120"><a name="p565181993120"></a><a name="p565181993120"></a>加密密钥管理接口，包括密钥的创建，查询，修改，删除等接口。</p>
</td>
</tr>
<tr id="row519911471288"><td class="cellrowborder" valign="top" width="25.929999999999996%" headers="mcps1.1.3.1.1 "><p id="p819910471786"><a name="p819910471786"></a><a name="p819910471786"></a>凭据管理服务</p>
</td>
<td class="cellrowborder" valign="top" width="74.07000000000001%" headers="mcps1.1.3.1.2 "><p id="p61993479815"><a name="p61993479815"></a><a name="p61993479815"></a>凭据管理接口，包括凭据的创建，查询，修改，删除等接口。</p>
</td>
</tr>
<tr id="row1980621151411"><td class="cellrowborder" valign="top" width="25.929999999999996%" headers="mcps1.1.3.1.1 "><p id="p1095493682017"><a name="p1095493682017"></a><a name="p1095493682017"></a>管理SSH密钥对</p>
</td>
<td class="cellrowborder" valign="top" width="74.07000000000001%" headers="mcps1.1.3.1.2 "><p id="p178077117141"><a name="p178077117141"></a><a name="p178077117141"></a>SSH密钥对管理接口（最新版本），包括SSH密钥对的创建，查询，修改，删除等接口。</p>
</td>
</tr>
<tr id="row17941818161515"><td class="cellrowborder" valign="top" width="25.929999999999996%" headers="mcps1.1.3.1.1 "><p id="p10250132985515"><a name="p10250132985515"></a><a name="p10250132985515"></a>历史API</p>
</td>
<td class="cellrowborder" valign="top" width="74.07000000000001%" headers="mcps1.1.3.1.2 "><p id="p738610286818"><a name="p738610286818"></a><a name="p738610286818"></a>SSH密钥对管理接口（V2.1和V2版本），包括SSH密钥对的创建，查询，修改，删除等接口。</p>
</td>
</tr>
</tbody>
</table>

## 历史API<a name="section1065134812519"></a>

<a name="table16207115112432"></a>
<table><thead align="left"><tr id="row320845104310"><th class="cellrowborder" valign="top" width="35.15%" id="mcps1.1.3.1.1"><p id="p1385512448"><a name="p1385512448"></a><a name="p1385512448"></a>API分类</p>
</th>
<th class="cellrowborder" valign="top" width="64.85%" id="mcps1.1.3.1.2"><p id="p1620817514438"><a name="p1620817514438"></a><a name="p1620817514438"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13208105114439"><td class="cellrowborder" rowspan="5" valign="top" width="35.15%" headers="mcps1.1.3.1.1 "><p id="p1551313407445"><a name="p1551313407445"></a><a name="p1551313407445"></a>管理SSH密钥对(V2.1)</p>
</td>
<td class="cellrowborder" valign="top" width="64.85%" headers="mcps1.1.3.1.2 "><p id="p17854574514"><a name="p17854574514"></a><a name="p17854574514"></a>查询SSH密钥对列表。</p>
</td>
</tr>
<tr id="row18208125144312"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="p1978174514513"><a name="p1978174514513"></a><a name="p1978174514513"></a>查询SSH密钥对详细信息。</p>
</td>
</tr>
<tr id="row1520875111430"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="p127914510454"><a name="p127914510454"></a><a name="p127914510454"></a>创建SSH密钥对和导入SSH密钥对，同时可选择对私钥进行托管。</p>
</td>
</tr>
<tr id="row3208175184311"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="p1879194510459"><a name="p1879194510459"></a><a name="p1879194510459"></a>根据SSH密钥对的名称，删除指定SSH密钥对。</p>
</td>
</tr>
<tr id="row14210115110436"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="p97912457456"><a name="p97912457456"></a><a name="p97912457456"></a>根据SSH密钥对的名称，修改指定SSH密钥对的描述信息。</p>
</td>
</tr>
<tr id="row785083313444"><td class="cellrowborder" rowspan="5" valign="top" width="35.15%" headers="mcps1.1.3.1.1 "><p id="p18241818104515"><a name="p18241818104515"></a><a name="p18241818104515"></a>管理SSH密钥对(V2.0)</p>
</td>
<td class="cellrowborder" valign="top" width="64.85%" headers="mcps1.1.3.1.2 "><p id="p1120815118435"><a name="p1120815118435"></a><a name="p1120815118435"></a>查询SSH密钥对信息列表。</p>
</td>
</tr>
<tr id="row1850173334411"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="p132081451174312"><a name="p132081451174312"></a><a name="p132081451174312"></a>根据SSH密钥对的名称查询指定SSH密钥对。</p>
</td>
</tr>
<tr id="row1585083311442"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="p202081651174312"><a name="p202081651174312"></a><a name="p202081651174312"></a>创建SSH密钥对，或把公钥导入华为云中，生成SSH密钥对。</p>
<p id="p13208145184317"><a name="p13208145184317"></a><a name="p13208145184317"></a>创建SSH密钥对成功后，请把响应数据中的私钥内容保存到本地文件，用户使用该私钥登录云服务器。为保证云服务器安全，私钥数据只能下载一次，请妥善保管。</p>
</td>
</tr>
<tr id="row128509336448"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="p32101251174311"><a name="p32101251174311"></a><a name="p32101251174311"></a>根据SSH密钥对的名称，删除指定SSH密钥对。</p>
</td>
</tr>
<tr id="row1362452012465"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="p1462502017463"><a name="p1462502017463"></a><a name="p1462502017463"></a>在同一个租户下可能包含多个用户帐号，将同一租户下目标用户帐号下的密钥对复制到当前用户帐号下。</p>
</td>
</tr>
</tbody>
</table>

