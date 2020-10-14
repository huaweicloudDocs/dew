# API概览<a name="dew_02_0057"></a>

数据加密服务提供的接口，您可以完整的使用数据加密服务的所有功能。

<a name="table1577981717153"></a>
<table><thead align="left"><tr id="row16810121712155"><th class="cellrowborder" valign="top" width="25.929999999999996%" id="mcps1.1.3.1.1"><p id="p13834717131516"><a name="p13834717131516"></a><a name="p13834717131516"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="74.07000000000001%" id="mcps1.1.3.1.2"><p id="p3883151714159"><a name="p3883151714159"></a><a name="p3883151714159"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2054614267164"><td class="cellrowborder" valign="top" width="25.929999999999996%" headers="mcps1.1.3.1.1 "><p id="p14546162641618"><a name="p14546162641618"></a><a name="p14546162641618"></a><a href="#section13159414572">管理加密密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="74.07000000000001%" headers="mcps1.1.3.1.2 "><p id="p565181993120"><a name="p565181993120"></a><a name="p565181993120"></a>加密密钥管理接口，包括密钥的创建，查询，修改，删除等接口。</p>
</td>
</tr>
<tr id="row1980621151411"><td class="cellrowborder" valign="top" width="25.929999999999996%" headers="mcps1.1.3.1.1 "><p id="p1095493682017"><a name="p1095493682017"></a><a name="p1095493682017"></a><a href="#section3485106141117">管理SSH密钥对</a></p>
</td>
<td class="cellrowborder" valign="top" width="74.07000000000001%" headers="mcps1.1.3.1.2 "><p id="p178077117141"><a name="p178077117141"></a><a name="p178077117141"></a>SSH密钥对管理接口（最新版本），包括SSH密钥对的创建，查询，修改，删除等接口。</p>
</td>
</tr>
<tr id="row17941818161515"><td class="cellrowborder" valign="top" width="25.929999999999996%" headers="mcps1.1.3.1.1 "><p id="p10250132985515"><a name="p10250132985515"></a><a name="p10250132985515"></a><a href="#section1065134812519">历史API</a></p>
</td>
<td class="cellrowborder" valign="top" width="74.07000000000001%" headers="mcps1.1.3.1.2 "><p id="p738610286818"><a name="p738610286818"></a><a name="p738610286818"></a>SSH密钥对管理接口（V2.1和V2版本），包括SSH密钥对的创建，查询，修改，删除等接口。</p>
</td>
</tr>
</tbody>
</table>

## 管理加密密钥<a name="section13159414572"></a>

<a name="table117567013494"></a>
<table><thead align="left"><tr id="row275630194912"><th class="cellrowborder" valign="top" width="23.82%" id="mcps1.1.4.1.1"><p id="p1528427185111"><a name="p1528427185111"></a><a name="p1528427185111"></a>API类别</p>
</th>
<th class="cellrowborder" valign="top" width="30.34%" id="mcps1.1.4.1.2"><p id="p3756190204918"><a name="p3756190204918"></a><a name="p3756190204918"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="45.839999999999996%" id="mcps1.1.4.1.3"><p id="p117561902497"><a name="p117561902497"></a><a name="p117561902497"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17709171717498"><td class="cellrowborder" rowspan="2" valign="top" width="23.82%" headers="mcps1.1.4.1.1 "><p id="p0678336105220"><a name="p0678336105220"></a><a name="p0678336105220"></a>查询API版本信息</p>
</td>
<td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.1.4.1.2 "><p id="p5710717124916"><a name="p5710717124916"></a><a name="p5710717124916"></a><a href="查询版本信息列表.md">查询版本信息列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.1.4.1.3 "><p id="p37103178497"><a name="p37103178497"></a><a name="p37103178497"></a>--</p>
</td>
</tr>
<tr id="row1071014170499"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p97101517174910"><a name="p97101517174910"></a><a name="p97101517174910"></a><a href="查询指定版本信息.md">查询指定版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12710101710492"><a name="p12710101710492"></a><a name="p12710101710492"></a>--</p>
</td>
</tr>
<tr id="row1671011710496"><td class="cellrowborder" rowspan="7" valign="top" width="23.82%" headers="mcps1.1.4.1.1 "><p id="p115798430574"><a name="p115798430574"></a><a name="p115798430574"></a>生命周期管理</p>
</td>
<td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.1.4.1.2 "><p id="p117101317104913"><a name="p117101317104913"></a><a name="p117101317104913"></a><a href="创建密钥.md">创建密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.1.4.1.3 "><p id="p67431122205"><a name="p67431122205"></a><a name="p67431122205"></a>创建一个用户主密钥。</p>
</td>
</tr>
<tr id="row47108178495"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p137100171499"><a name="p137100171499"></a><a name="p137100171499"></a><a href="启用密钥.md">启用密钥</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p974301216201"><a name="p974301216201"></a><a name="p974301216201"></a>启用密钥，密钥启用后才可以使用。</p>
</td>
</tr>
<tr id="row1271061713495"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p67101617104917"><a name="p67101617104917"></a><a name="p67101617104917"></a><a href="禁用密钥.md">禁用密钥</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p574310125206"><a name="p574310125206"></a><a name="p574310125206"></a>禁用密钥，密钥禁用后不可以使用。</p>
</td>
</tr>
<tr id="row67101217204916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1771081764910"><a name="p1771081764910"></a><a name="p1771081764910"></a><a href="计划删除密钥.md">计划删除密钥</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1974331213204"><a name="p1974331213204"></a><a name="p1974331213204"></a>计划删除一个指定密钥，可设置7天～1096天内删除密钥。密钥将被彻底删除后，使用该密钥加密的数据将无法解密。</p>
</td>
</tr>
<tr id="row37101176493"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20710121764911"><a name="p20710121764911"></a><a name="p20710121764911"></a><a href="取消计划删除密钥.md">取消计划删除密钥</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p137437125201"><a name="p137437125201"></a><a name="p137437125201"></a>取消计划删除密钥，取消后，用户可以正常使用该密钥。</p>
</td>
</tr>
<tr id="row1871015172494"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12710141754914"><a name="p12710141754914"></a><a name="p12710141754914"></a><a href="修改密钥别名.md">修改密钥别名</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9744812192010"><a name="p9744812192010"></a><a name="p9744812192010"></a>查询用户所有密钥列表。</p>
</td>
</tr>
<tr id="row1571021713498"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p127101017134913"><a name="p127101017134913"></a><a name="p127101017134913"></a><a href="修改密钥描述.md">修改密钥描述</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17744712122014"><a name="p17744712122014"></a><a name="p17744712122014"></a>查询指定密钥的详细信息。</p>
</td>
</tr>
<tr id="row107119172498"><td class="cellrowborder" rowspan="5" valign="top" width="23.82%" headers="mcps1.1.4.1.1 "><p id="p10261346185916"><a name="p10261346185916"></a><a name="p10261346185916"></a>数据密钥管理</p>
</td>
<td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.1.4.1.2 "><p id="p137113170493"><a name="p137113170493"></a><a name="p137113170493"></a><a href="创建随机数.md">创建随机数</a></p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.1.4.1.3 "><p id="p034013114219"><a name="p034013114219"></a><a name="p034013114219"></a>生成8~8192bit范围内的随机数，且须为8的倍数。</p>
</td>
</tr>
<tr id="row97112178496"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p571191716495"><a name="p571191716495"></a><a name="p571191716495"></a><a href="创建数据密钥.md">创建数据密钥</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p163408113213"><a name="p163408113213"></a><a name="p163408113213"></a>创建数据密钥，返回结果包含明文和密文。</p>
</td>
</tr>
<tr id="row1711117194918"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p103002755114"><a name="p103002755114"></a><a name="p103002755114"></a><a href="创建不含明文数据密钥.md">创建不含明文数据密钥</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1634018192117"><a name="p1634018192117"></a><a name="p1634018192117"></a>创建数据密钥，返回结果只包含密文。</p>
</td>
</tr>
<tr id="row1271151754910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p187116176491"><a name="p187116176491"></a><a name="p187116176491"></a><a href="加密数据密钥.md">加密数据密钥</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p133402132114"><a name="p133402132114"></a><a name="p133402132114"></a>使用指定的用户主密钥加密数据密钥。</p>
</td>
</tr>
<tr id="row17115178499"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9713151712496"><a name="p9713151712496"></a><a name="p9713151712496"></a><a href="解密数据密钥.md">解密数据密钥</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1934031142120"><a name="p1934031142120"></a><a name="p1934031142120"></a>使用指定的用户主密钥解密数据密钥。</p>
</td>
</tr>
<tr id="row18420512124916"><td class="cellrowborder" rowspan="3" valign="top" width="23.82%" headers="mcps1.1.4.1.1 "><p id="p19811555816"><a name="p19811555816"></a><a name="p19811555816"></a>导入密钥管理</p>
</td>
<td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.1.4.1.2 "><p id="p44211512204914"><a name="p44211512204914"></a><a name="p44211512204914"></a><a href="获取密钥导入参数.md">获取密钥导入参数</a></p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.1.4.1.3 "><p id="p17526122412111"><a name="p17526122412111"></a><a name="p17526122412111"></a>获取导入密钥的必要参数，包括密钥导入令牌和密钥加密公钥。</p>
</td>
</tr>
<tr id="row942131254919"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p94218123498"><a name="p94218123498"></a><a name="p94218123498"></a><a href="导入密钥材料.md">导入密钥材料</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5526824162117"><a name="p5526824162117"></a><a name="p5526824162117"></a>导入指定密钥的密钥材料。</p>
</td>
</tr>
<tr id="row11421181254918"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1421812104912"><a name="p1421812104912"></a><a name="p1421812104912"></a><a href="删除密钥材料.md">删除密钥材料</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9526024132120"><a name="p9526024132120"></a><a name="p9526024132120"></a>删除指定密钥的密钥材料。</p>
</td>
</tr>
<tr id="row3421112114914"><td class="cellrowborder" rowspan="5" valign="top" width="23.82%" headers="mcps1.1.4.1.1 "><p id="p143801513821"><a name="p143801513821"></a><a name="p143801513821"></a>授权管理</p>
</td>
<td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.1.4.1.2 "><p id="p54211312204919"><a name="p54211312204919"></a><a name="p54211312204919"></a><a href="创建授权.md">创建授权</a></p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.1.4.1.3 "><p id="p8741114510216"><a name="p8741114510216"></a><a name="p8741114510216"></a>被授权用户可以对授权密钥进行操作。</p>
</td>
</tr>
<tr id="row19421111211498"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p542131224918"><a name="p542131224918"></a><a name="p542131224918"></a><a href="撤销授权.md">撤销授权</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p177412458217"><a name="p177412458217"></a><a name="p177412458217"></a>授权用户撤销被授权用户操作密钥的权限。</p>
</td>
</tr>
<tr id="row842151212495"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p442117121492"><a name="p442117121492"></a><a name="p442117121492"></a><a href="退役授权.md">退役授权</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p774194511219"><a name="p774194511219"></a><a name="p774194511219"></a>被授权用户不再具有授权密钥的操作权。</p>
</td>
</tr>
<tr id="row1742281264917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p742271254912"><a name="p742271254912"></a><a name="p742271254912"></a><a href="查询授权列表.md">查询授权列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14741345152119"><a name="p14741345152119"></a><a name="p14741345152119"></a>查询密钥的授权列表。</p>
</td>
</tr>
<tr id="row187568024914"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p117569015490"><a name="p117569015490"></a><a name="p117569015490"></a><a href="查询可退役授权列表.md">查询可退役授权列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p174174516218"><a name="p174174516218"></a><a name="p174174516218"></a>查询用户可以退役的授权列表。</p>
</td>
</tr>
<tr id="row1375718094916"><td class="cellrowborder" rowspan="2" valign="top" width="23.82%" headers="mcps1.1.4.1.1 "><p id="p19041026821"><a name="p19041026821"></a><a name="p19041026821"></a>小数据加解密</p>
</td>
<td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.1.4.1.2 "><p id="p1075740124915"><a name="p1075740124915"></a><a name="p1075740124915"></a><a href="加密数据.md">加密数据</a></p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.1.4.1.3 "><p id="p15398162815225"><a name="p15398162815225"></a><a name="p15398162815225"></a>使用指定的用户主密钥加密数据。</p>
</td>
</tr>
<tr id="row16757170204910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1975711013499"><a name="p1975711013499"></a><a name="p1975711013499"></a><a href="解密数据.md">解密数据</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12398142812225"><a name="p12398142812225"></a><a name="p12398142812225"></a>解密数据。</p>
</td>
</tr>
<tr id="row451991119312"><td class="cellrowborder" rowspan="4" valign="top" width="23.82%" headers="mcps1.1.4.1.1 "><p id="p837317181319"><a name="p837317181319"></a><a name="p837317181319"></a>轮换管理</p>
</td>
<td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.1.4.1.2 "><p id="p175191711336"><a name="p175191711336"></a><a name="p175191711336"></a><a href="开启密钥轮换.md">开启密钥轮换</a></p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.1.4.1.3 "><p id="p970110506221"><a name="p970110506221"></a><a name="p970110506221"></a>开启用户主密钥轮换，默认主密钥及外部导入密钥不支持轮换操作。</p>
</td>
</tr>
<tr id="row1351919111433"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10519611237"><a name="p10519611237"></a><a name="p10519611237"></a><a href="修改密钥轮换周期.md">修改密钥轮换周期</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5701155014224"><a name="p5701155014224"></a><a name="p5701155014224"></a>修改用户主密钥轮换周期。</p>
</td>
</tr>
<tr id="row75191011232"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p45194111032"><a name="p45194111032"></a><a name="p45194111032"></a><a href="关闭密钥轮换.md">关闭密钥轮换</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7702165002219"><a name="p7702165002219"></a><a name="p7702165002219"></a>关闭用户主密钥轮换。</p>
</td>
</tr>
<tr id="row1519101111315"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1752051113313"><a name="p1752051113313"></a><a name="p1752051113313"></a><a href="查询密钥轮换状态.md">查询密钥轮换状态</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p970225072210"><a name="p970225072210"></a><a name="p970225072210"></a>查询用户主密钥轮换状态。</p>
</td>
</tr>
<tr id="row175201411532"><td class="cellrowborder" rowspan="6" valign="top" width="23.82%" headers="mcps1.1.4.1.1 "><p id="p1827013392032"><a name="p1827013392032"></a><a name="p1827013392032"></a>标签管理</p>
</td>
<td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.1.4.1.2 "><p id="p14520311438"><a name="p14520311438"></a><a name="p14520311438"></a><a href="查询密钥实例.md">查询密钥实例</a></p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.1.4.1.3 "><p id="p11692734162311"><a name="p11692734162311"></a><a name="p11692734162311"></a>通过标签过滤，查询指定用户主密钥的详细信息。</p>
</td>
</tr>
<tr id="row151086714317"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9108571837"><a name="p9108571837"></a><a name="p9108571837"></a><a href="查询密钥标签.md">查询密钥标签</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p169310342232"><a name="p169310342232"></a><a name="p169310342232"></a>查询指定密钥的标签信息。</p>
</td>
</tr>
<tr id="row141081671031"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p141081274319"><a name="p141081274319"></a><a name="p141081274319"></a><a href="查询项目标签.md">查询项目标签</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18693123411235"><a name="p18693123411235"></a><a name="p18693123411235"></a>查询用户在指定项目下的所有标签集合。</p>
</td>
</tr>
<tr id="row51091671132"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p51091272318"><a name="p51091272318"></a><a name="p51091272318"></a><a href="批量添加删除密钥标签.md">批量添加删除密钥标签</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p169353412320"><a name="p169353412320"></a><a name="p169353412320"></a>批量添加或删除密钥标签。</p>
</td>
</tr>
<tr id="row710967636"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9109576314"><a name="p9109576314"></a><a name="p9109576314"></a><a href="添加密钥标签.md">添加密钥标签</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p469323414230"><a name="p469323414230"></a><a name="p469323414230"></a>添加密钥标签。</p>
</td>
</tr>
<tr id="row167577010491"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2075780124911"><a name="p2075780124911"></a><a name="p2075780124911"></a><a href="删除密钥标签.md">删除密钥标签</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19693163492315"><a name="p19693163492315"></a><a name="p19693163492315"></a>删除密钥标签。</p>
</td>
</tr>
<tr id="row23022056437"><td class="cellrowborder" rowspan="4" valign="top" width="23.82%" headers="mcps1.1.4.1.1 "><p id="p6479915410"><a name="p6479915410"></a><a name="p6479915410"></a>查询接口</p>
</td>
<td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.1.4.1.2 "><p id="p030213561131"><a name="p030213561131"></a><a name="p030213561131"></a><a href="查询密钥列表.md">查询密钥列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.1.4.1.3 "><p id="p8717154102410"><a name="p8717154102410"></a><a name="p8717154102410"></a>查询用户所有密钥列表。</p>
</td>
</tr>
<tr id="row127573014919"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p57571200494"><a name="p57571200494"></a><a name="p57571200494"></a><a href="查询密钥信息.md">查询密钥信息</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p97171747247"><a name="p97171747247"></a><a name="p97171747247"></a>查询指定密钥的详细信息。</p>
</td>
</tr>
<tr id="row675713054911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p187572084918"><a name="p187572084918"></a><a name="p187572084918"></a><a href="查询实例数.md">查询实例数</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p140221511248"><a name="p140221511248"></a><a name="p140221511248"></a>获取用户已经创建的用户主密钥数量，不包含默认主密钥。</p>
</td>
</tr>
<tr id="row27571901494"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p575716012496"><a name="p575716012496"></a><a name="p575716012496"></a><a href="查询配额.md">查询配额</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1340312157244"><a name="p1340312157244"></a><a name="p1340312157244"></a>查询用户可以创建的用户主密钥配额总数及当前使用量信息，不包含默认主密钥。</p>
</td>
</tr>
</tbody>
</table>

## 管理SSH密钥对<a name="section3485106141117"></a>

<a name="table246734120109"></a>
<table><thead align="left"><tr id="row164686419109"><th class="cellrowborder" valign="top" width="24.712471247124714%" id="mcps1.1.4.1.1"><p id="p946874110101"><a name="p946874110101"></a><a name="p946874110101"></a>API类别</p>
</th>
<th class="cellrowborder" valign="top" width="29.192919291929194%" id="mcps1.1.4.1.2"><p id="p184687412102"><a name="p184687412102"></a><a name="p184687412102"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="46.094609460946096%" id="mcps1.1.4.1.3"><p id="p74689416108"><a name="p74689416108"></a><a name="p74689416108"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5468204191011"><td class="cellrowborder" rowspan="5" valign="top" width="24.712471247124714%" headers="mcps1.1.4.1.1 "><p id="p1062613141122"><a name="p1062613141122"></a><a name="p1062613141122"></a>密钥对管理</p>
</td>
<td class="cellrowborder" valign="top" width="29.192919291929194%" headers="mcps1.1.4.1.2 "><p id="p12468114115101"><a name="p12468114115101"></a><a name="p12468114115101"></a><a href="查询SSH密钥对列表.md">查询SSH密钥对列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.094609460946096%" headers="mcps1.1.4.1.3 "><p id="p103971129194712"><a name="p103971129194712"></a><a name="p103971129194712"></a>查询SSH密钥对信息列表。</p>
</td>
</tr>
<tr id="row146812418102"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p146814161015"><a name="p146814161015"></a><a name="p146814161015"></a><a href="创建和导入SSH密钥对.md">创建和导入SSH密钥对</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4397929194716"><a name="p4397929194716"></a><a name="p4397929194716"></a>创建SSH密钥对，或把公钥导入华为云中，生成SSH密钥对。</p>
<p id="p28432030134815"><a name="p28432030134815"></a><a name="p28432030134815"></a>创建SSH密钥对成功后，请把响应数据中的私钥内容保存到本地文件，用户使用该私钥登录云服务器。为保证云服务器安全，私钥数据只能下载一次，请妥善保管。</p>
</td>
</tr>
<tr id="row3468134101015"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7468841111020"><a name="p7468841111020"></a><a name="p7468841111020"></a><a href="查询SSH密钥对详细信息.md">查询SSH密钥对详细信息</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p33971429194719"><a name="p33971429194719"></a><a name="p33971429194719"></a>根据SSH密钥对的名称查询指定SSH密钥对。</p>
</td>
</tr>
<tr id="row3468134141010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p184680415100"><a name="p184680415100"></a><a name="p184680415100"></a><a href="删除SSH密钥对.md">删除SSH密钥对</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1739822924714"><a name="p1739822924714"></a><a name="p1739822924714"></a>根据SSH密钥对的名称，删除指定SSH密钥对。</p>
</td>
</tr>
<tr id="row1746834151011"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1446819414101"><a name="p1446819414101"></a><a name="p1446819414101"></a><a href="更新SSH密钥对描述.md">更新SSH密钥对描述</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p123985294473"><a name="p123985294473"></a><a name="p123985294473"></a>更新SSH密钥对描述信息。</p>
</td>
</tr>
<tr id="row1095312941220"><td class="cellrowborder" rowspan="7" valign="top" width="24.712471247124714%" headers="mcps1.1.4.1.1 "><p id="p1495513401215"><a name="p1495513401215"></a><a name="p1495513401215"></a>密钥对任务管理</p>
</td>
<td class="cellrowborder" valign="top" width="29.192919291929194%" headers="mcps1.1.4.1.2 "><p id="p595342911218"><a name="p595342911218"></a><a name="p595342911218"></a><a href="绑定SSH密钥对.md">绑定SSH密钥对</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.094609460946096%" headers="mcps1.1.4.1.3 "><p id="p610017289472"><a name="p610017289472"></a><a name="p610017289472"></a>给指定的虚拟机绑定（替换或重置，替换需提供虚拟机已配置的SSH密钥对私钥；重置不需要提供虚拟机的SSH密钥对私钥）新的SSH密钥对。</p>
</td>
</tr>
<tr id="row129531429171215"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p195311293120"><a name="p195311293120"></a><a name="p195311293120"></a><a href="解绑SSH密钥对.md">解绑SSH密钥对</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11953122921213"><a name="p11953122921213"></a><a name="p11953122921213"></a>给指定的虚拟机解除绑定SSH密钥对并恢复SSH密码登录。</p>
</td>
</tr>
<tr id="row99531729191217"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p49539298126"><a name="p49539298126"></a><a name="p49539298126"></a><a href="查询任务信息.md">查询任务信息</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8953142915127"><a name="p8953142915127"></a><a name="p8953142915127"></a>根据SSH密钥对接口返回的task_id，查询SSH密钥对当前任务的执行状态。</p>
</td>
</tr>
<tr id="row14155521151217"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p131551219125"><a name="p131551219125"></a><a name="p131551219125"></a><a href="查询失败的任务信息.md">查询失败的任务信息</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p151550216127"><a name="p151550216127"></a><a name="p151550216127"></a>查询绑定、解绑等操作失败的任务信息。</p>
</td>
</tr>
<tr id="row71559215122"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p141552021111216"><a name="p141552021111216"></a><a name="p141552021111216"></a><a href="删除所有失败的任务.md">删除所有失败的任务</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1015515212123"><a name="p1015515212123"></a><a name="p1015515212123"></a>删除操作失败的任务信息。</p>
</td>
</tr>
<tr id="row9468174110109"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p114682041121013"><a name="p114682041121013"></a><a name="p114682041121013"></a><a href="删除失败的任务.md">删除失败的任务</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13468741171017"><a name="p13468741171017"></a><a name="p13468741171017"></a>删除失败的任务。</p>
</td>
</tr>
<tr id="row146811412102"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3468104118101"><a name="p3468104118101"></a><a name="p3468104118101"></a><a href="查询正在处理的任务信息.md">查询正在处理的任务信息</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p94581149132017"><a name="p94581149132017"></a><a name="p94581149132017"></a>查询正在处理的任务信息。</p>
</td>
</tr>
</tbody>
</table>

## 历史API<a name="section1065134812519"></a>

<a name="table16207115112432"></a>
<table><thead align="left"><tr id="row320845104310"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.4.1.1"><p id="p1385512448"><a name="p1385512448"></a><a name="p1385512448"></a>API分类</p>
</th>
<th class="cellrowborder" valign="top" width="28.88%" id="mcps1.1.4.1.2"><p id="p122081551124315"><a name="p122081551124315"></a><a name="p122081551124315"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="46.12%" id="mcps1.1.4.1.3"><p id="p1620817514438"><a name="p1620817514438"></a><a name="p1620817514438"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13208105114439"><td class="cellrowborder" rowspan="5" valign="top" width="25%" headers="mcps1.1.4.1.1 "><p id="p1551313407445"><a name="p1551313407445"></a><a name="p1551313407445"></a>管理SSH密钥对(V2.1)</p>
</td>
<td class="cellrowborder" valign="top" width="28.88%" headers="mcps1.1.4.1.2 "><p id="p1978045134519"><a name="p1978045134519"></a><a name="p1978045134519"></a><a href="查询SSH密钥对列表(V2-1).md">查询SSH密钥对列表(V2.1)</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.1.4.1.3 "><p id="p17854574514"><a name="p17854574514"></a><a name="p17854574514"></a>查询SSH密钥对列表。</p>
</td>
</tr>
<tr id="row18208125144312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1578145144510"><a name="p1578145144510"></a><a name="p1578145144510"></a><a href="查询SSH密钥对详情(V2-1).md">查询SSH密钥对详情(V2.1)</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1978174514513"><a name="p1978174514513"></a><a name="p1978174514513"></a>查询SSH密钥对详细信息。</p>
</td>
</tr>
<tr id="row1520875111430"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1796450451"><a name="p1796450451"></a><a name="p1796450451"></a><a href="创建及导入SSH密钥对(V2-1).md">创建及导入SSH密钥对(V2.1)</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p127914510454"><a name="p127914510454"></a><a name="p127914510454"></a>创建SSH密钥对和导入SSH密钥对，同时可选择对私钥进行托管。</p>
</td>
</tr>
<tr id="row3208175184311"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8791445144517"><a name="p8791445144517"></a><a name="p8791445144517"></a><a href="删除SSH密钥对(V2-1).md">删除SSH密钥对(V2.1)</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1879194510459"><a name="p1879194510459"></a><a name="p1879194510459"></a>根据SSH密钥对的名称，删除指定SSH密钥对。</p>
</td>
</tr>
<tr id="row14210115110436"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17944594516"><a name="p17944594516"></a><a name="p17944594516"></a><a href="修改密钥对描述信息(V2-1).md">修改密钥对描述信息(V2.1)</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p97912457456"><a name="p97912457456"></a><a name="p97912457456"></a>根据SSH密钥对的名称，修改指定SSH密钥对的描述信息。</p>
</td>
</tr>
<tr id="row785083313444"><td class="cellrowborder" rowspan="5" valign="top" width="25%" headers="mcps1.1.4.1.1 "><p id="p18241818104515"><a name="p18241818104515"></a><a name="p18241818104515"></a>管理SSH密钥对(V2.0)</p>
</td>
<td class="cellrowborder" valign="top" width="28.88%" headers="mcps1.1.4.1.2 "><p id="p13208165134310"><a name="p13208165134310"></a><a name="p13208165134310"></a><a href="查询SSH密钥对列表(V2).md">查询SSH密钥对列表(V2)</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.1.4.1.3 "><p id="p1120815118435"><a name="p1120815118435"></a><a name="p1120815118435"></a>查询SSH密钥对信息列表。</p>
</td>
</tr>
<tr id="row1850173334411"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15208165124314"><a name="p15208165124314"></a><a name="p15208165124314"></a><a href="查询SSH密钥对详情(V2).md">查询SSH密钥对详情(V2)</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p132081451174312"><a name="p132081451174312"></a><a name="p132081451174312"></a>根据SSH密钥对的名称查询指定SSH密钥对。</p>
</td>
</tr>
<tr id="row1585083311442"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5208125184312"><a name="p5208125184312"></a><a name="p5208125184312"></a><a href="创建及导入SSH密钥对(V2).md">创建及导入SSH密钥对(V2)</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p202081651174312"><a name="p202081651174312"></a><a name="p202081651174312"></a>创建SSH密钥对，或把公钥导入华为云中，生成SSH密钥对。</p>
<p id="p13208145184317"><a name="p13208145184317"></a><a name="p13208145184317"></a>创建SSH密钥对成功后，请把响应数据中的私钥内容保存到本地文件，用户使用该私钥登录云服务器。为保证云服务器安全，私钥数据只能下载一次，请妥善保管。</p>
</td>
</tr>
<tr id="row128509336448"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15209205114315"><a name="p15209205114315"></a><a name="p15209205114315"></a><a href="删除SSH密钥对(V2).md">删除SSH密钥对(V2)</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p32101251174311"><a name="p32101251174311"></a><a name="p32101251174311"></a>根据SSH密钥对的名称，删除指定SSH密钥对。</p>
</td>
</tr>
<tr id="row1362452012465"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18210105124319"><a name="p18210105124319"></a><a name="p18210105124319"></a><a href="复制SSH密钥对（废弃）.md">复制SSH密钥对（废弃）</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1462502017463"><a name="p1462502017463"></a><a name="p1462502017463"></a>在同一个租户下可能包含多个用户帐号，将同一租户下目标用户帐号下的密钥对复制到当前用户帐号下。</p>
</td>
</tr>
</tbody>
</table>

