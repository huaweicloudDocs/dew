# API概览<a name="dew_02_0057"></a>

通过使用数据加密服务提供的接口，您可以完整的使用数据加密服务的所有功能。

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
<tr id="row1980621151411"><td class="cellrowborder" valign="top" width="25.929999999999996%" headers="mcps1.1.3.1.1 "><p id="p1095493682017"><a name="p1095493682017"></a><a name="p1095493682017"></a>管理SSH密钥对(V2)</p>
</td>
<td class="cellrowborder" valign="top" width="74.07000000000001%" headers="mcps1.1.3.1.2 "><p id="p178077117141"><a name="p178077117141"></a><a name="p178077117141"></a>SSH密钥对管理接口（V2版本），包括SSH密钥对的创建，查询，修改，删除等接口。</p>
</td>
</tr>
<tr id="row17941818161515"><td class="cellrowborder" valign="top" width="25.929999999999996%" headers="mcps1.1.3.1.1 "><p id="p10250132985515"><a name="p10250132985515"></a><a name="p10250132985515"></a>管理SSH密钥对(V2.1)</p>
</td>
<td class="cellrowborder" valign="top" width="74.07000000000001%" headers="mcps1.1.3.1.2 "><p id="p738610286818"><a name="p738610286818"></a><a name="p738610286818"></a>SSH密钥对管理接口（V2.1版本），包括SSH密钥对的创建，查询，修改，删除等接口。</p>
</td>
</tr>
</tbody>
</table>

## 管理加密密钥<a name="section13159414572"></a>

<a name="table177341359552"></a>
<table><thead align="left"><tr id="row973425919514"><th class="cellrowborder" valign="top" width="29.631780694621906%" id="mcps1.1.3.1.1"><p id="p87342591555"><a name="p87342591555"></a><a name="p87342591555"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="70.36821930537809%" id="mcps1.1.3.1.2"><p id="p157341859858"><a name="p157341859858"></a><a name="p157341859858"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16734959259"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1373445920518"><a name="p1373445920518"></a><a name="p1373445920518"></a><a href="创建密钥.md">创建密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p79581042143011"><a name="p79581042143011"></a><a name="p79581042143011"></a>创建一个用户主密钥。</p>
</td>
</tr>
<tr id="row3149115214253"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1214945282512"><a name="p1214945282512"></a><a name="p1214945282512"></a><a href="启用密钥.md">启用密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p12149205272519"><a name="p12149205272519"></a><a name="p12149205272519"></a>启用密钥，密钥启用后才可以使用。</p>
</td>
</tr>
<tr id="row155214557258"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1255210550255"><a name="p1255210550255"></a><a name="p1255210550255"></a><a href="禁用密钥.md">禁用密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p20552115502517"><a name="p20552115502517"></a><a name="p20552115502517"></a>禁用密钥，密钥禁用后不可以使用。</p>
</td>
</tr>
<tr id="row11602458112515"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p0602558142513"><a name="p0602558142513"></a><a name="p0602558142513"></a><a href="计划删除密钥.md">计划删除密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p96023581259"><a name="p96023581259"></a><a name="p96023581259"></a>计划删除一个指定密钥，可设置7天～1096天内删除密钥。密钥将被彻底删除后，使用该密钥加密的数据将无法解密。</p>
</td>
</tr>
<tr id="row218953112619"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p518933172613"><a name="p518933172613"></a><a name="p518933172613"></a><a href="取消计划删除密钥.md">取消计划删除密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1318911372613"><a name="p1318911372613"></a><a name="p1318911372613"></a>取消计划删除密钥，取消后，用户可以正常使用该密钥。</p>
</td>
</tr>
<tr id="row3404189192616"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p14059915267"><a name="p14059915267"></a><a name="p14059915267"></a><a href="查询密钥列表.md">查询密钥列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1740529172617"><a name="p1740529172617"></a><a name="p1740529172617"></a>查询用户所有密钥列表。</p>
</td>
</tr>
<tr id="row12054715262"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p32051173263"><a name="p32051173263"></a><a name="p32051173263"></a><a href="查询密钥信息.md">查询密钥信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p102052715263"><a name="p102052715263"></a><a name="p102052715263"></a>查询指定密钥的详细信息。</p>
</td>
</tr>
<tr id="row9823134982516"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p536471910307"><a name="p536471910307"></a><a name="p536471910307"></a><a href="创建随机数.md">创建随机数</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1682374992518"><a name="p1682374992518"></a><a name="p1682374992518"></a>生成512bit的随机数。</p>
</td>
</tr>
<tr id="row119151718237"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p49167710234"><a name="p49167710234"></a><a name="p49167710234"></a><a href="创建数据密钥.md">创建数据密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p129161675236"><a name="p129161675236"></a><a name="p129161675236"></a>创建数据密钥，返回结果包含明文和密文。</p>
</td>
</tr>
<tr id="row2485721289"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p14851827285"><a name="p14851827285"></a><a name="p14851827285"></a><a href="创建不含明文数据密钥.md">创建不含明文数据密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1948517216285"><a name="p1948517216285"></a><a name="p1948517216285"></a>创建数据密钥，返回结果只包含密文。</p>
</td>
</tr>
<tr id="row1451317082810"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p7513140152814"><a name="p7513140152814"></a><a name="p7513140152814"></a><a href="加密数据密钥.md">加密数据密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p3513140142812"><a name="p3513140142812"></a><a name="p3513140142812"></a>使用指定的用户主密钥加密数据密钥。</p>
</td>
</tr>
<tr id="row197618589273"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p4761258202713"><a name="p4761258202713"></a><a name="p4761258202713"></a><a href="解密数据密钥.md">解密数据密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p2761205810273"><a name="p2761205810273"></a><a name="p2761205810273"></a>使用指定的用户主密钥解密数据密钥。</p>
</td>
</tr>
<tr id="row95309213296"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p73628193302"><a name="p73628193302"></a><a name="p73628193302"></a><a href="查询实例数.md">查询实例数</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p141321122298"><a name="p141321122298"></a><a name="p141321122298"></a>获取用户已经创建的用户主密钥数量，不包含默认主密钥。</p>
</td>
</tr>
<tr id="row13528160192911"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p17889915112911"><a name="p17889915112911"></a><a name="p17889915112911"></a><a href="查询配额.md">查询配额</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p588951510294"><a name="p588951510294"></a><a name="p588951510294"></a>查询用户可以创建的用户主密钥配额总数及当前使用量信息，不包含默认主密钥。</p>
</td>
</tr>
<tr id="row9402105820289"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1896422714296"><a name="p1896422714296"></a><a name="p1896422714296"></a><a href="修改密钥别名.md">修改密钥别名</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1892914188298"><a name="p1892914188298"></a><a name="p1892914188298"></a>修改用户主密钥别名。</p>
</td>
</tr>
<tr id="row18681566281"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p16132812192910"><a name="p16132812192910"></a><a name="p16132812192910"></a><a href="修改密钥描述.md">修改密钥描述</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p161289916297"><a name="p161289916297"></a><a name="p161289916297"></a>修改用户主密钥描述信息。</p>
</td>
</tr>
<tr id="row8235125692712"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p5269195653111"><a name="p5269195653111"></a><a name="p5269195653111"></a><a href="创建授权.md">创建授权</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p19959150193219"><a name="p19959150193219"></a><a name="p19959150193219"></a>被授权用户可以对授权密钥进行操作。</p>
</td>
</tr>
<tr id="row7445154215311"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p164451242143120"><a name="p164451242143120"></a><a name="p164451242143120"></a><a href="撤销授权.md">撤销授权</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p11958180113211"><a name="p11958180113211"></a><a name="p11958180113211"></a>授权用户撤销被授权用户操作密钥的权限。</p>
</td>
</tr>
<tr id="row20793124814319"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p2793548103115"><a name="p2793548103115"></a><a name="p2793548103115"></a><a href="退役授权.md">退役授权</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p895611063215"><a name="p895611063215"></a><a name="p895611063215"></a>被授权用户不再具有授权密钥的操作权。</p>
</td>
</tr>
<tr id="row1737134643117"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1273717469314"><a name="p1273717469314"></a><a name="p1273717469314"></a><a href="查询授权列表.md">查询授权列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p10955190153218"><a name="p10955190153218"></a><a name="p10955190153218"></a>查询密钥的授权列表。</p>
</td>
</tr>
<tr id="row37536407310"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p13754114043116"><a name="p13754114043116"></a><a name="p13754114043116"></a><a href="查询可退役授权列表.md">查询可退役授权列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1995460183215"><a name="p1995460183215"></a><a name="p1995460183215"></a>查询用户可以退役的授权列表。</p>
</td>
</tr>
<tr id="row8992646183210"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1270112163316"><a name="p1270112163316"></a><a name="p1270112163316"></a><a href="加密数据.md">加密数据</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p3271142153313"><a name="p3271142153313"></a><a name="p3271142153313"></a>使用指定的用户主密钥加密数据。</p>
</td>
</tr>
<tr id="row12792114233218"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p161021219133313"><a name="p161021219133313"></a><a name="p161021219133313"></a><a href="解密数据.md">解密数据</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1510291933318"><a name="p1510291933318"></a><a name="p1510291933318"></a>解密数据。</p>
</td>
</tr>
<tr id="row273411591512"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p87341059754"><a name="p87341059754"></a><a name="p87341059754"></a><a href="获取密钥导入参数.md">获取密钥导入参数</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p29531010324"><a name="p29531010324"></a><a name="p29531010324"></a>获取导入密钥的必要参数，包括密钥导入令牌和密钥加密公钥。</p>
</td>
</tr>
<tr id="row610942717348"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p5109112763410"><a name="p5109112763410"></a><a name="p5109112763410"></a><a href="导入密钥材料.md">导入密钥材料</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p210982773418"><a name="p210982773418"></a><a name="p210982773418"></a>导入指定密钥的密钥材料。</p>
</td>
</tr>
<tr id="row0193112563117"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p181931325123110"><a name="p181931325123110"></a><a name="p181931325123110"></a><a href="删除密钥材料.md">删除密钥材料</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p17951900321"><a name="p17951900321"></a><a name="p17951900321"></a>删除指定密钥的密钥材料。</p>
</td>
</tr>
<tr id="row12734559159"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1873418591652"><a name="p1873418591652"></a><a name="p1873418591652"></a><a href="开启密钥轮换.md">开启密钥轮换</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1195016063217"><a name="p1195016063217"></a><a name="p1195016063217"></a>开启用户主密钥轮换，默认主密钥及外部导入密钥不支持轮换操作。</p>
</td>
</tr>
<tr id="row1415815481343"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p015974823412"><a name="p015974823412"></a><a name="p015974823412"></a><a href="修改密钥轮换周期.md">修改密钥轮换周期</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p0159648113415"><a name="p0159648113415"></a><a name="p0159648113415"></a>修改用户主密钥轮换周期。</p>
</td>
</tr>
<tr id="row19392541344"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p184017543344"><a name="p184017543344"></a><a name="p184017543344"></a><a href="关闭密钥轮换.md">关闭密钥轮换</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p640115414345"><a name="p640115414345"></a><a name="p640115414345"></a>关闭用户主密钥轮换。</p>
</td>
</tr>
<tr id="row57349591520"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1036317373313"><a name="p1036317373313"></a><a name="p1036317373313"></a><a href="查询密钥轮换状态.md">查询密钥轮换状态</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p194918014328"><a name="p194918014328"></a><a name="p194918014328"></a>查询用户主密钥轮换状态。</p>
</td>
</tr>
<tr id="row9447165213327"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p23312166366"><a name="p23312166366"></a><a name="p23312166366"></a><a href="查询密钥实例.md">查询密钥实例</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1334160363"><a name="p1334160363"></a><a name="p1334160363"></a>通过标签过滤，查询指定用户主密钥的详细信息。</p>
</td>
</tr>
<tr id="row1473418590511"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1873418594515"><a name="p1873418594515"></a><a name="p1873418594515"></a><a href="查询密钥标签.md">查询密钥标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p16948701328"><a name="p16948701328"></a><a name="p16948701328"></a>查询指定密钥的标签信息。</p>
</td>
</tr>
<tr id="row651175619363"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p6511185623618"><a name="p6511185623618"></a><a name="p6511185623618"></a><a href="查询项目标签.md">查询项目标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1051155611364"><a name="p1051155611364"></a><a name="p1051155611364"></a>查询用户在指定项目下的所有标签集合。</p>
</td>
</tr>
<tr id="row1759018541361"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p1759015419365"><a name="p1759015419365"></a><a name="p1759015419365"></a><a href="批量添加删除密钥标签.md">批量添加删除密钥标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p8590175423610"><a name="p8590175423610"></a><a name="p8590175423610"></a>批量添加或删除密钥标签。</p>
</td>
</tr>
<tr id="row1866395833611"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p126631558143614"><a name="p126631558143614"></a><a name="p126631558143614"></a><a href="添加密钥标签.md">添加密钥标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p3663258153617"><a name="p3663258153617"></a><a name="p3663258153617"></a>添加密钥标签。</p>
</td>
</tr>
<tr id="row103767529364"><td class="cellrowborder" valign="top" width="29.631780694621906%" headers="mcps1.1.3.1.1 "><p id="p43761452193616"><a name="p43761452193616"></a><a name="p43761452193616"></a><a href="删除密钥标签.md">删除密钥标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="70.36821930537809%" headers="mcps1.1.3.1.2 "><p id="p1637613523368"><a name="p1637613523368"></a><a name="p1637613523368"></a>删除密钥标签。</p>
</td>
</tr>
</tbody>
</table>

## 管理SSH密钥对\(V2\)<a name="section1320812195617"></a>

<a name="table1520831175617"></a>
<table><thead align="left"><tr id="row120801105619"><th class="cellrowborder" valign="top" width="32.11%" id="mcps1.1.3.1.1"><p id="p20208101145610"><a name="p20208101145610"></a><a name="p20208101145610"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="67.89%" id="mcps1.1.3.1.2"><p id="p1120881135610"><a name="p1120881135610"></a><a name="p1120881135610"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1820813116568"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p1120814175613"><a name="p1120814175613"></a><a name="p1120814175613"></a><a href="查询SSH密钥对列表(V2).md">查询SSH密钥对列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p87765215428"><a name="p87765215428"></a><a name="p87765215428"></a>查询SSH密钥对信息列表。</p>
</td>
</tr>
<tr id="row420914113566"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p13209111165612"><a name="p13209111165612"></a><a name="p13209111165612"></a><a href="查询SSH密钥对详情(V2).md">查询SSH密钥对详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p774195224216"><a name="p774195224216"></a><a name="p774195224216"></a>根据SSH密钥对的名称查询指定SSH密钥对。</p>
</td>
</tr>
<tr id="row72091415569"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p120912135612"><a name="p120912135612"></a><a name="p120912135612"></a><a href="创建及导入SSH密钥对(V2).md">创建及导入SSH密钥对</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p172752144217"><a name="p172752144217"></a><a name="p172752144217"></a>创建SSH密钥对，或把公钥导入华为云中，生成SSH密钥对。</p>
<p id="p88609591718"><a name="p88609591718"></a><a name="p88609591718"></a>创建SSH密钥对成功后，请把响应数据中的私钥内容保存到本地文件，用户使用该私钥登录云服务器。为保证云服务器安全，私钥数据只能下载一次，请妥善保管。</p>
</td>
</tr>
<tr id="row82094135616"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p32091014564"><a name="p32091014564"></a><a name="p32091014564"></a><a href="删除SSH密钥对(V2).md">删除SSH密钥对</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p1369195215427"><a name="p1369195215427"></a><a name="p1369195215427"></a>根据SSH密钥对的名称，删除指定SSH密钥对。</p>
</td>
</tr>
<tr id="row92091145615"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p152097112568"><a name="p152097112568"></a><a name="p152097112568"></a><a href="复制SSH密钥对（旧）.md">复制SSH密钥对（旧）</a></p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p156713523421"><a name="p156713523421"></a><a name="p156713523421"></a>在同一个租户下可能包含多个用户帐号，将同一租户下目标用户帐号下的密钥对复制到当前用户帐号下。</p>
</td>
</tr>
<tr id="row12209121115612"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="p1209614569"><a name="p1209614569"></a><a name="p1209614569"></a><a href="复制SSH密钥对.md">复制SSH密钥对</a></p>
</td>
</tr>
</tbody>
</table>

## 管理SSH密钥对\(V2.1\)<a name="section19254821105614"></a>

<a name="table172541021145620"></a>
<table><thead align="left"><tr id="row1254221175611"><th class="cellrowborder" valign="top" width="32.11%" id="mcps1.1.3.1.1"><p id="p3254132175611"><a name="p3254132175611"></a><a name="p3254132175611"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="67.89%" id="mcps1.1.3.1.2"><p id="p125462119563"><a name="p125462119563"></a><a name="p125462119563"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row122541521155611"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p162541021165616"><a name="p162541021165616"></a><a name="p162541021165616"></a><a href="查询SSH密钥对列表(V2-1).md">查询SSH密钥对列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p778912118456"><a name="p778912118456"></a><a name="p778912118456"></a>查询SSH密钥对列表。</p>
</td>
</tr>
<tr id="row122541921185617"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p19254121155620"><a name="p19254121155620"></a><a name="p19254121155620"></a><a href="查询SSH密钥对详情(V2-1).md">查询SSH密钥对详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p17788611455"><a name="p17788611455"></a><a name="p17788611455"></a>查询SSH密钥对详细信息。</p>
</td>
</tr>
<tr id="row15255182145610"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p9255162115618"><a name="p9255162115618"></a><a name="p9255162115618"></a><a href="创建及导入SSH密钥对(V2-1).md">创建及导入SSH密钥对</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p197873110453"><a name="p197873110453"></a><a name="p197873110453"></a>创建SSH密钥对和导入SSH密钥对，同时可选择对私钥进行托管。</p>
</td>
</tr>
<tr id="row32551021135615"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p1125512216563"><a name="p1125512216563"></a><a name="p1125512216563"></a><a href="删除SSH密钥对(V2-1).md">删除SSH密钥对</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p12787121164512"><a name="p12787121164512"></a><a name="p12787121164512"></a>根据SSH密钥对的名称，删除指定SSH密钥对。</p>
</td>
</tr>
<tr id="row0255821155615"><td class="cellrowborder" valign="top" width="32.11%" headers="mcps1.1.3.1.1 "><p id="p32551021175616"><a name="p32551021175616"></a><a name="p32551021175616"></a><a href="修改密钥对描述信息.md">修改密钥对描述信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.89%" headers="mcps1.1.3.1.2 "><p id="p278614117454"><a name="p278614117454"></a><a name="p278614117454"></a>根据SSH密钥对的名称，修改指定SSH密钥对的描述信息。</p>
</td>
</tr>
</tbody>
</table>

