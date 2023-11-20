# 创建用户并授权使用DEW<a name="dew_01_0135"></a>

如果您需要对您所拥有的DEW进行精细的权限管理，您可以使用[统一身份认证服务](https://support.huaweicloud.com/usermanual-iam/iam_01_0001.html)（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为帐号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用DEW资源。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将DEW资源委托给更专业、高效的其他华为帐号或者云服务，这些帐号或者云服务可以根据权限进行代运维。

如果华为帐号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用DEW服务的其它功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#fig23111471897)所示。

## 前提条件<a name="section121325115513"></a>

给用户组授权之前，请您了解用户组可以添加的DEW权限，并结合实际需求进行选择，DEW支持的系统权限如[表1](#table194381648115212)所示。

若您需要对除DEW之外的其它服务授权，IAM支持服务的所有权限请参见[系统权限](https://support.huaweicloud.com/permissions/policy_list.html?product=dew)。

**表 1**  DEW系统权限

<a name="table194381648115212"></a>
<table><thead align="left"><tr id="zh-cn_topic_0169425412_row1346222921318"><th class="cellrowborder" valign="top" width="28.67%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0169425412_p246217292138"><a name="zh-cn_topic_0169425412_p246217292138"></a><a name="zh-cn_topic_0169425412_p246217292138"></a>系统角色/策略名称</p>
</th>
<th class="cellrowborder" valign="top" width="45.839999999999996%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0169425412_p146292918139"><a name="zh-cn_topic_0169425412_p146292918139"></a><a name="zh-cn_topic_0169425412_p146292918139"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="16.55%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0169425412_p3459112418415"><a name="zh-cn_topic_0169425412_p3459112418415"></a><a name="zh-cn_topic_0169425412_p3459112418415"></a>类别</p>
</th>
<th class="cellrowborder" valign="top" width="8.94%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0169425412_p161282127415"><a name="zh-cn_topic_0169425412_p161282127415"></a><a name="zh-cn_topic_0169425412_p161282127415"></a>依赖关系</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0169425412_row1462142915137"><td class="cellrowborder" valign="top" width="28.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p25241140125910"><a name="zh-cn_topic_0169425412_p25241140125910"></a><a name="zh-cn_topic_0169425412_p25241140125910"></a>KMS Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p162039144415"><a name="zh-cn_topic_0169425412_p162039144415"></a><a name="zh-cn_topic_0169425412_p162039144415"></a>密钥管理服务(KMS)管理员，拥有该服务下的所有权限。</p>
</td>
<td class="cellrowborder" valign="top" width="16.55%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p134591224104113"><a name="zh-cn_topic_0169425412_p134591224104113"></a><a name="zh-cn_topic_0169425412_p134591224104113"></a>系统角色</p>
</td>
<td class="cellrowborder" valign="top" width="8.94%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p14128201274112"><a name="zh-cn_topic_0169425412_p14128201274112"></a><a name="zh-cn_topic_0169425412_p14128201274112"></a>无</p>
</td>
</tr>
<tr id="zh-cn_topic_0169425412_row4708123532810"><td class="cellrowborder" valign="top" width="28.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p07090356289"><a name="zh-cn_topic_0169425412_p07090356289"></a><a name="zh-cn_topic_0169425412_p07090356289"></a>KMS CMKFullAccess</p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p12709103592818"><a name="zh-cn_topic_0169425412_p12709103592818"></a><a name="zh-cn_topic_0169425412_p12709103592818"></a>密钥管理服务(KMS)的加密密钥所有权限。拥有该权限的用户可以完成基于策略授权的所有操作。</p>
</td>
<td class="cellrowborder" valign="top" width="16.55%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p1170963517284"><a name="zh-cn_topic_0169425412_p1170963517284"></a><a name="zh-cn_topic_0169425412_p1170963517284"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="8.94%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p1012851254117"><a name="zh-cn_topic_0169425412_p1012851254117"></a><a name="zh-cn_topic_0169425412_p1012851254117"></a>无</p>
</td>
</tr>
<tr id="zh-cn_topic_0169425412_row87771645614"><td class="cellrowborder" valign="top" width="28.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p167791343617"><a name="zh-cn_topic_0169425412_p167791343617"></a><a name="zh-cn_topic_0169425412_p167791343617"></a>KMS CMKReadOnlyAccess</p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p13779104567"><a name="zh-cn_topic_0169425412_p13779104567"></a><a name="zh-cn_topic_0169425412_p13779104567"></a>密钥管理服务(KMS)的加密密钥只读权限。拥有该权限的用户可以完成基于策略授权的所有操作。</p>
</td>
<td class="cellrowborder" valign="top" width="16.55%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p6853174013616"><a name="zh-cn_topic_0169425412_p6853174013616"></a><a name="zh-cn_topic_0169425412_p6853174013616"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="8.94%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p188539401964"><a name="zh-cn_topic_0169425412_p188539401964"></a><a name="zh-cn_topic_0169425412_p188539401964"></a>无</p>
</td>
</tr>
<tr id="zh-cn_topic_0169425412_row13720637112819"><td class="cellrowborder" valign="top" width="28.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p13864438161415"><a name="zh-cn_topic_0169425412_p13864438161415"></a><a name="zh-cn_topic_0169425412_p13864438161415"></a>DEW KeypairFullAccess</p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p1872023712815"><a name="zh-cn_topic_0169425412_p1872023712815"></a><a name="zh-cn_topic_0169425412_p1872023712815"></a>数据加密服务中密钥对管理服务(KPS)的所有权限。拥有该权限的用户可以完成基于策略授权的所有操作。</p>
</td>
<td class="cellrowborder" valign="top" width="16.55%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p772133712819"><a name="zh-cn_topic_0169425412_p772133712819"></a><a name="zh-cn_topic_0169425412_p772133712819"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="8.94%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p1128151213419"><a name="zh-cn_topic_0169425412_p1128151213419"></a><a name="zh-cn_topic_0169425412_p1128151213419"></a>无</p>
</td>
</tr>
<tr id="zh-cn_topic_0169425412_row43641644115114"><td class="cellrowborder" valign="top" width="28.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p4365104445120"><a name="zh-cn_topic_0169425412_p4365104445120"></a><a name="zh-cn_topic_0169425412_p4365104445120"></a>DEW KeypairReadOnlyAccess</p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p19365194475114"><a name="zh-cn_topic_0169425412_p19365194475114"></a><a name="zh-cn_topic_0169425412_p19365194475114"></a>数据加密服务中密钥对管理服务(KPS)的查看权限。拥有该权限的用户仅能查看密钥对管理服务(KPS)数据。</p>
</td>
<td class="cellrowborder" valign="top" width="16.55%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p6776131716526"><a name="zh-cn_topic_0169425412_p6776131716526"></a><a name="zh-cn_topic_0169425412_p6776131716526"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="8.94%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p212818123411"><a name="zh-cn_topic_0169425412_p212818123411"></a><a name="zh-cn_topic_0169425412_p212818123411"></a>无</p>
</td>
</tr>
<tr id="zh-cn_topic_0169425412_row46093321416"><td class="cellrowborder" valign="top" width="28.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p5610173219110"><a name="zh-cn_topic_0169425412_p5610173219110"></a><a name="zh-cn_topic_0169425412_p5610173219110"></a>CSMS FullAccess</p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p46108320119"><a name="zh-cn_topic_0169425412_p46108320119"></a><a name="zh-cn_topic_0169425412_p46108320119"></a>数据加密服务中凭据管理服务(CSMS)的所有权限。拥有该权限的用户可以完成基于策略授权的所有操作。</p>
</td>
<td class="cellrowborder" valign="top" width="16.55%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p150620501628"><a name="zh-cn_topic_0169425412_p150620501628"></a><a name="zh-cn_topic_0169425412_p150620501628"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="8.94%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p125063501026"><a name="zh-cn_topic_0169425412_p125063501026"></a><a name="zh-cn_topic_0169425412_p125063501026"></a>无</p>
</td>
</tr>
<tr id="zh-cn_topic_0169425412_row760254111120"><td class="cellrowborder" valign="top" width="28.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p96021411618"><a name="zh-cn_topic_0169425412_p96021411618"></a><a name="zh-cn_topic_0169425412_p96021411618"></a>CSMS ReadOnlyAccess</p>
</td>
<td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p1360215411011"><a name="zh-cn_topic_0169425412_p1360215411011"></a><a name="zh-cn_topic_0169425412_p1360215411011"></a>数据加密服务中凭据管理服务(CSMS)的只读权限。拥有该权限的用户可以完成基于策略授权的所有操作。</p>
</td>
<td class="cellrowborder" valign="top" width="16.55%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p123341451028"><a name="zh-cn_topic_0169425412_p123341451028"></a><a name="zh-cn_topic_0169425412_p123341451028"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="8.94%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p153349517216"><a name="zh-cn_topic_0169425412_p153349517216"></a><a name="zh-cn_topic_0169425412_p153349517216"></a>无</p>
</td>
</tr>
</tbody>
</table>

[表2](#table18421457162111)列出了DEW常用操作与系统权限的授权关系，您可以参照该表选择合适的系统权限。

**表 2**  常用操作与系统权限的关系

<a name="table18421457162111"></a>
<table><thead align="left"><tr id="row9421857202116"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.1"><p id="p19227182034219"><a name="p19227182034219"></a><a name="p19227182034219"></a>操作</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.2"><p id="p11227132054211"><a name="p11227132054211"></a><a name="p11227132054211"></a>KMS Administrator</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.3"><p id="p8227122074219"><a name="p8227122074219"></a><a name="p8227122074219"></a>KMS CMKFullAccess</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.4"><p id="p922710201425"><a name="p922710201425"></a><a name="p922710201425"></a>DEW KeypairFullAccess</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.5"><p id="p1422782024218"><a name="p1422782024218"></a><a name="p1422782024218"></a>DEW KeypairReadOnlyAccess</p>
</th>
</tr>
</thead>
<tbody><tr id="row9431057102113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1522710203425"><a name="p1522710203425"></a><a name="p1522710203425"></a>创建密钥</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p1422714207425"><a name="p1422714207425"></a><a name="p1422714207425"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p922742018420"><a name="p922742018420"></a><a name="p922742018420"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p4227420114212"><a name="p4227420114212"></a><a name="p4227420114212"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p1165181904318"><a name="p1165181904318"></a><a name="p1165181904318"></a>x</p>
</td>
</tr>
<tr id="row104717142213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1822772014219"><a name="p1822772014219"></a><a name="p1822772014219"></a>启用密钥</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p322702034220"><a name="p322702034220"></a><a name="p322702034220"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p0227132012420"><a name="p0227132012420"></a><a name="p0227132012420"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1622762017427"><a name="p1622762017427"></a><a name="p1622762017427"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p1565519134318"><a name="p1565519134318"></a><a name="p1565519134318"></a>x</p>
</td>
</tr>
<tr id="row7655111902217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p422762014420"><a name="p422762014420"></a><a name="p422762014420"></a>禁用密钥</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p3227020174215"><a name="p3227020174215"></a><a name="p3227020174215"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p172271420164217"><a name="p172271420164217"></a><a name="p172271420164217"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p197691054114213"><a name="p197691054114213"></a><a name="p197691054114213"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p136516196439"><a name="p136516196439"></a><a name="p136516196439"></a>x</p>
</td>
</tr>
<tr id="row145418553404"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p32281320134219"><a name="p32281320134219"></a><a name="p32281320134219"></a>计划删除密钥</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p17228122094217"><a name="p17228122094217"></a><a name="p17228122094217"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p102289206423"><a name="p102289206423"></a><a name="p102289206423"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1776915543429"><a name="p1776915543429"></a><a name="p1776915543429"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p46541911438"><a name="p46541911438"></a><a name="p46541911438"></a>x</p>
</td>
</tr>
<tr id="row12454125515401"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p3228120184213"><a name="p3228120184213"></a><a name="p3228120184213"></a>取消计划删除密钥</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p622892034218"><a name="p622892034218"></a><a name="p622892034218"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p522892011423"><a name="p522892011423"></a><a name="p522892011423"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p873825914211"><a name="p873825914211"></a><a name="p873825914211"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p10275120104311"><a name="p10275120104311"></a><a name="p10275120104311"></a>x</p>
</td>
</tr>
<tr id="row11453155512403"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p622812208429"><a name="p622812208429"></a><a name="p622812208429"></a>修改密钥别名</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p122862018421"><a name="p122862018421"></a><a name="p122862018421"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1228320154219"><a name="p1228320154219"></a><a name="p1228320154219"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p197381959184219"><a name="p197381959184219"></a><a name="p197381959184219"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p14275132019438"><a name="p14275132019438"></a><a name="p14275132019438"></a>x</p>
</td>
</tr>
<tr id="row12565165714014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p3228820174215"><a name="p3228820174215"></a><a name="p3228820174215"></a>修改密钥描述</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p13228520184220"><a name="p13228520184220"></a><a name="p13228520184220"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p022819206427"><a name="p022819206427"></a><a name="p022819206427"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p10738659124211"><a name="p10738659124211"></a><a name="p10738659124211"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p14275152013436"><a name="p14275152013436"></a><a name="p14275152013436"></a>x</p>
</td>
</tr>
<tr id="row105651957124019"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p12228162054211"><a name="p12228162054211"></a><a name="p12228162054211"></a>创建随机数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p192281420134215"><a name="p192281420134215"></a><a name="p192281420134215"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p92281320124215"><a name="p92281320124215"></a><a name="p92281320124215"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p6738175954217"><a name="p6738175954217"></a><a name="p6738175954217"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p172757203433"><a name="p172757203433"></a><a name="p172757203433"></a>x</p>
</td>
</tr>
<tr id="row1856455794013"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p11228920184216"><a name="p11228920184216"></a><a name="p11228920184216"></a>创建数据密钥</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p1022819202421"><a name="p1022819202421"></a><a name="p1022819202421"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p522852094218"><a name="p522852094218"></a><a name="p522852094218"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p27185115438"><a name="p27185115438"></a><a name="p27185115438"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p10842202215433"><a name="p10842202215433"></a><a name="p10842202215433"></a>x</p>
</td>
</tr>
<tr id="row287871014111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p6228172012429"><a name="p6228172012429"></a><a name="p6228172012429"></a>创建不含明文数据密钥</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p1228152064213"><a name="p1228152064213"></a><a name="p1228152064213"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p922815200423"><a name="p922815200423"></a><a name="p922815200423"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p207184110438"><a name="p207184110438"></a><a name="p207184110438"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p0843192220438"><a name="p0843192220438"></a><a name="p0843192220438"></a>x</p>
</td>
</tr>
<tr id="row9878191084111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p5228720144213"><a name="p5228720144213"></a><a name="p5228720144213"></a>加密数据密钥</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p15228182013425"><a name="p15228182013425"></a><a name="p15228182013425"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p9229192014214"><a name="p9229192014214"></a><a name="p9229192014214"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p57181117431"><a name="p57181117431"></a><a name="p57181117431"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p148431922154316"><a name="p148431922154316"></a><a name="p148431922154316"></a>x</p>
</td>
</tr>
<tr id="row13877710204117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p162291120154212"><a name="p162291120154212"></a><a name="p162291120154212"></a>解密数据密钥</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p15229220164213"><a name="p15229220164213"></a><a name="p15229220164213"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p102292020204218"><a name="p102292020204218"></a><a name="p102292020204218"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p187189112437"><a name="p187189112437"></a><a name="p187189112437"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p148431022114318"><a name="p148431022114318"></a><a name="p148431022114318"></a>x</p>
</td>
</tr>
<tr id="row13591912144118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p3229192011422"><a name="p3229192011422"></a><a name="p3229192011422"></a>获取密钥导入参数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p202298204425"><a name="p202298204425"></a><a name="p202298204425"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1522922034212"><a name="p1522922034212"></a><a name="p1522922034212"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p7837154204315"><a name="p7837154204315"></a><a name="p7837154204315"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p139461424144319"><a name="p139461424144319"></a><a name="p139461424144319"></a>x</p>
</td>
</tr>
<tr id="row13590312164115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p922912202429"><a name="p922912202429"></a><a name="p922912202429"></a>导入密钥材料</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p13230132014218"><a name="p13230132014218"></a><a name="p13230132014218"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1123014207422"><a name="p1123014207422"></a><a name="p1123014207422"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p883734154310"><a name="p883734154310"></a><a name="p883734154310"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p19946112424313"><a name="p19946112424313"></a><a name="p19946112424313"></a>x</p>
</td>
</tr>
<tr id="row9590412184114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p172301220184217"><a name="p172301220184217"></a><a name="p172301220184217"></a>删除密钥材料</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p823022024216"><a name="p823022024216"></a><a name="p823022024216"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p523018203421"><a name="p523018203421"></a><a name="p523018203421"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p68381454311"><a name="p68381454311"></a><a name="p68381454311"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p99461724104310"><a name="p99461724104310"></a><a name="p99461724104310"></a>x</p>
</td>
</tr>
<tr id="row38611719174116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p2230172044214"><a name="p2230172044214"></a><a name="p2230172044214"></a>创建授权</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p7230120194211"><a name="p7230120194211"></a><a name="p7230120194211"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p4230142010420"><a name="p4230142010420"></a><a name="p4230142010420"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p148385474314"><a name="p148385474314"></a><a name="p148385474314"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p11946162434312"><a name="p11946162434312"></a><a name="p11946162434312"></a>x</p>
</td>
</tr>
<tr id="row20861111924111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p5230142034214"><a name="p5230142034214"></a><a name="p5230142034214"></a>撤销授权</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p17230120164214"><a name="p17230120164214"></a><a name="p17230120164214"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p42301320114219"><a name="p42301320114219"></a><a name="p42301320114219"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p136601462437"><a name="p136601462437"></a><a name="p136601462437"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p1630227194310"><a name="p1630227194310"></a><a name="p1630227194310"></a>x</p>
</td>
</tr>
<tr id="row19860181934111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p323022024212"><a name="p323022024212"></a><a name="p323022024212"></a>退役授权</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p9230172019427"><a name="p9230172019427"></a><a name="p9230172019427"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p92307209426"><a name="p92307209426"></a><a name="p92307209426"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p16601063435"><a name="p16601063435"></a><a name="p16601063435"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p33042744319"><a name="p33042744319"></a><a name="p33042744319"></a>x</p>
</td>
</tr>
<tr id="row18859119164111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p112311420154220"><a name="p112311420154220"></a><a name="p112311420154220"></a>查询授权列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p5231182004213"><a name="p5231182004213"></a><a name="p5231182004213"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1523162054220"><a name="p1523162054220"></a><a name="p1523162054220"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p666019624317"><a name="p666019624317"></a><a name="p666019624317"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p83002744318"><a name="p83002744318"></a><a name="p83002744318"></a>x</p>
</td>
</tr>
<tr id="row28581219184117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1223116202426"><a name="p1223116202426"></a><a name="p1223116202426"></a>查询可退役授权列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p123162084215"><a name="p123162084215"></a><a name="p123162084215"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p6231420164217"><a name="p6231420164217"></a><a name="p6231420164217"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p116601762435"><a name="p116601762435"></a><a name="p116601762435"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p1330827174317"><a name="p1330827174317"></a><a name="p1330827174317"></a>x</p>
</td>
</tr>
<tr id="row685761974111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p823142012428"><a name="p823142012428"></a><a name="p823142012428"></a>加密数据</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p923102084216"><a name="p923102084216"></a><a name="p923102084216"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p32311520104213"><a name="p32311520104213"></a><a name="p32311520104213"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p17198812434"><a name="p17198812434"></a><a name="p17198812434"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p8544528174318"><a name="p8544528174318"></a><a name="p8544528174318"></a>x</p>
</td>
</tr>
<tr id="row085613190411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p923132024218"><a name="p923132024218"></a><a name="p923132024218"></a>解密数据</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p323118207425"><a name="p323118207425"></a><a name="p323118207425"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p162312205426"><a name="p162312205426"></a><a name="p162312205426"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1871919812431"><a name="p1871919812431"></a><a name="p1871919812431"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p1354402810435"><a name="p1354402810435"></a><a name="p1354402810435"></a>x</p>
</td>
</tr>
<tr id="row1066737433"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p19671938439"><a name="p19671938439"></a><a name="p19671938439"></a>签名消息</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p86719314439"><a name="p86719314439"></a><a name="p86719314439"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p36718354318"><a name="p36718354318"></a><a name="p36718354318"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p66733104314"><a name="p66733104314"></a><a name="p66733104314"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p15671935430"><a name="p15671935430"></a><a name="p15671935430"></a>x</p>
</td>
</tr>
<tr id="row11541105914318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p45414591434"><a name="p45414591434"></a><a name="p45414591434"></a>验证签名</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p854216594436"><a name="p854216594436"></a><a name="p854216594436"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1654275918436"><a name="p1654275918436"></a><a name="p1654275918436"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p154235964316"><a name="p154235964316"></a><a name="p154235964316"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p16542559144315"><a name="p16542559144315"></a><a name="p16542559144315"></a>x</p>
</td>
</tr>
<tr id="row18560192419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p142311120124216"><a name="p142311120124216"></a><a name="p142311120124216"></a>开启密钥轮换</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p92311920134214"><a name="p92311920134214"></a><a name="p92311920134214"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p52311520134215"><a name="p52311520134215"></a><a name="p52311520134215"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p177197854315"><a name="p177197854315"></a><a name="p177197854315"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p3544202864317"><a name="p3544202864317"></a><a name="p3544202864317"></a>x</p>
</td>
</tr>
<tr id="row285561916416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p122314209426"><a name="p122314209426"></a><a name="p122314209426"></a>修改密钥轮换周期</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p6231122017425"><a name="p6231122017425"></a><a name="p6231122017425"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p15231142044213"><a name="p15231142044213"></a><a name="p15231142044213"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p20719118134318"><a name="p20719118134318"></a><a name="p20719118134318"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p2544928134315"><a name="p2544928134315"></a><a name="p2544928134315"></a>x</p>
</td>
</tr>
<tr id="row9855191954114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p623182014426"><a name="p623182014426"></a><a name="p623182014426"></a>关闭密钥轮换</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p123132024213"><a name="p123132024213"></a><a name="p123132024213"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p202314206424"><a name="p202314206424"></a><a name="p202314206424"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p6263191064310"><a name="p6263191064310"></a><a name="p6263191064310"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p2030493164311"><a name="p2030493164311"></a><a name="p2030493164311"></a>x</p>
</td>
</tr>
<tr id="row19854101904111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p923272004218"><a name="p923272004218"></a><a name="p923272004218"></a>查询密钥轮换状态</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p5232102024212"><a name="p5232102024212"></a><a name="p5232102024212"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p112321820194213"><a name="p112321820194213"></a><a name="p112321820194213"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p326313104439"><a name="p326313104439"></a><a name="p326313104439"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p16304163154310"><a name="p16304163154310"></a><a name="p16304163154310"></a>x</p>
</td>
</tr>
<tr id="row285381913413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p152322020194217"><a name="p152322020194217"></a><a name="p152322020194217"></a>查询密钥实例</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p142324209429"><a name="p142324209429"></a><a name="p142324209429"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1823262024211"><a name="p1823262024211"></a><a name="p1823262024211"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1726310106431"><a name="p1726310106431"></a><a name="p1726310106431"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p19304331184315"><a name="p19304331184315"></a><a name="p19304331184315"></a>x</p>
</td>
</tr>
<tr id="row1285361919419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p3232182024211"><a name="p3232182024211"></a><a name="p3232182024211"></a>查询密钥标签</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p123215207424"><a name="p123215207424"></a><a name="p123215207424"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1123218209425"><a name="p1123218209425"></a><a name="p1123218209425"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p17263191016431"><a name="p17263191016431"></a><a name="p17263191016431"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p12305831184316"><a name="p12305831184316"></a><a name="p12305831184316"></a>x</p>
</td>
</tr>
<tr id="row12852161917412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p42321820104210"><a name="p42321820104210"></a><a name="p42321820104210"></a>查询项目标签</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p11232102020425"><a name="p11232102020425"></a><a name="p11232102020425"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p132321020114217"><a name="p132321020114217"></a><a name="p132321020114217"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p5791212124319"><a name="p5791212124319"></a><a name="p5791212124319"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p17826163214319"><a name="p17826163214319"></a><a name="p17826163214319"></a>x</p>
</td>
</tr>
<tr id="row11851319164119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p4233220114215"><a name="p4233220114215"></a><a name="p4233220114215"></a>批量添加删除密钥标签</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p1623362019427"><a name="p1623362019427"></a><a name="p1623362019427"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p10233192074216"><a name="p10233192074216"></a><a name="p10233192074216"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p3791912184316"><a name="p3791912184316"></a><a name="p3791912184316"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p148269323432"><a name="p148269323432"></a><a name="p148269323432"></a>x</p>
</td>
</tr>
<tr id="row9933192212419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p723314202422"><a name="p723314202422"></a><a name="p723314202422"></a>添加密钥标签</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p423342016422"><a name="p423342016422"></a><a name="p423342016422"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p2233182012429"><a name="p2233182012429"></a><a name="p2233182012429"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1079121215433"><a name="p1079121215433"></a><a name="p1079121215433"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p19826193254318"><a name="p19826193254318"></a><a name="p19826193254318"></a>x</p>
</td>
</tr>
<tr id="row159321226415"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1823312013421"><a name="p1823312013421"></a><a name="p1823312013421"></a>删除密钥标签</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p3233720184218"><a name="p3233720184218"></a><a name="p3233720184218"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p10233172084216"><a name="p10233172084216"></a><a name="p10233172084216"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p279271234315"><a name="p279271234315"></a><a name="p279271234315"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p082693213437"><a name="p082693213437"></a><a name="p082693213437"></a>x</p>
</td>
</tr>
<tr id="row1932112218413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p6233172012421"><a name="p6233172012421"></a><a name="p6233172012421"></a>查询密钥列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p1233122044210"><a name="p1233122044210"></a><a name="p1233122044210"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p823332044217"><a name="p823332044217"></a><a name="p823332044217"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1339041414311"><a name="p1339041414311"></a><a name="p1339041414311"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p1329263418433"><a name="p1329263418433"></a><a name="p1329263418433"></a>x</p>
</td>
</tr>
<tr id="row893142224112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1023315205424"><a name="p1023315205424"></a><a name="p1023315205424"></a>查询密钥信息</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p723352013420"><a name="p723352013420"></a><a name="p723352013420"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p9233820144212"><a name="p9233820144212"></a><a name="p9233820144212"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p93901914124313"><a name="p93901914124313"></a><a name="p93901914124313"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p122923342431"><a name="p122923342431"></a><a name="p122923342431"></a>x</p>
</td>
</tr>
<tr id="row311813714443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1111911375448"><a name="p1111911375448"></a><a name="p1111911375448"></a>查询公钥信息</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p31190379449"><a name="p31190379449"></a><a name="p31190379449"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p411915370445"><a name="p411915370445"></a><a name="p411915370445"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1011933717443"><a name="p1011933717443"></a><a name="p1011933717443"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p18119143774416"><a name="p18119143774416"></a><a name="p18119143774416"></a>x</p>
</td>
</tr>
<tr id="row893042284113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p16233220164219"><a name="p16233220164219"></a><a name="p16233220164219"></a>查询实例数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p3233132019425"><a name="p3233132019425"></a><a name="p3233132019425"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p9233520144216"><a name="p9233520144216"></a><a name="p9233520144216"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p5390181474316"><a name="p5390181474316"></a><a name="p5390181474316"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p15292334144311"><a name="p15292334144311"></a><a name="p15292334144311"></a>x</p>
</td>
</tr>
<tr id="row293016229419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p9233320144218"><a name="p9233320144218"></a><a name="p9233320144218"></a>查询配额</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p142331820114215"><a name="p142331820114215"></a><a name="p142331820114215"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p8233192054213"><a name="p8233192054213"></a><a name="p8233192054213"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p2039051484317"><a name="p2039051484317"></a><a name="p2039051484317"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p829223417430"><a name="p829223417430"></a><a name="p829223417430"></a>x</p>
</td>
</tr>
<tr id="row5929422154111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1923415209422"><a name="p1923415209422"></a><a name="p1923415209422"></a>查询密钥对列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p19799123974314"><a name="p19799123974314"></a><a name="p19799123974314"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p81470417439"><a name="p81470417439"></a><a name="p81470417439"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1234920184212"><a name="p1234920184212"></a><a name="p1234920184212"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p2023462012423"><a name="p2023462012423"></a><a name="p2023462012423"></a>√</p>
</td>
</tr>
<tr id="row199288228416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1723410202429"><a name="p1723410202429"></a><a name="p1723410202429"></a>创建或导入密钥对</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p279923919438"><a name="p279923919438"></a><a name="p279923919438"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p21478413439"><a name="p21478413439"></a><a name="p21478413439"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p02341920114213"><a name="p02341920114213"></a><a name="p02341920114213"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p2234192015424"><a name="p2234192015424"></a><a name="p2234192015424"></a>x</p>
</td>
</tr>
<tr id="row592732274112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p11234172017428"><a name="p11234172017428"></a><a name="p11234172017428"></a>查询密钥对</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p67998396435"><a name="p67998396435"></a><a name="p67998396435"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p201471541144314"><a name="p201471541144314"></a><a name="p201471541144314"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p923532024211"><a name="p923532024211"></a><a name="p923532024211"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p162361620114219"><a name="p162361620114219"></a><a name="p162361620114219"></a>√</p>
</td>
</tr>
<tr id="row1592712229418"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p11236122034213"><a name="p11236122034213"></a><a name="p11236122034213"></a>删除密钥对</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p579913390439"><a name="p579913390439"></a><a name="p579913390439"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p151472041144316"><a name="p151472041144316"></a><a name="p151472041144316"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p182363205420"><a name="p182363205420"></a><a name="p182363205420"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p141311251194317"><a name="p141311251194317"></a><a name="p141311251194317"></a>x</p>
</td>
</tr>
<tr id="row18926622134120"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1236520154210"><a name="p1236520154210"></a><a name="p1236520154210"></a>更新密钥对描述</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p199741642164313"><a name="p199741642164313"></a><a name="p199741642164313"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p3779444174316"><a name="p3779444174316"></a><a name="p3779444174316"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1923613208429"><a name="p1923613208429"></a><a name="p1923613208429"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p16131155174310"><a name="p16131155174310"></a><a name="p16131155174310"></a>x</p>
</td>
</tr>
<tr id="row209256220415"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p623632094217"><a name="p623632094217"></a><a name="p623632094217"></a>绑定密钥对</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p139741342184316"><a name="p139741342184316"></a><a name="p139741342184316"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p87791944134312"><a name="p87791944134312"></a><a name="p87791944134312"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p323742024219"><a name="p323742024219"></a><a name="p323742024219"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p1213119519434"><a name="p1213119519434"></a><a name="p1213119519434"></a>x</p>
</td>
</tr>
<tr id="row6925122164117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1723732019428"><a name="p1723732019428"></a><a name="p1723732019428"></a>解绑密钥对</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p199741842134315"><a name="p199741842134315"></a><a name="p199741842134315"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p107791544124320"><a name="p107791544124320"></a><a name="p107791544124320"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p52375209428"><a name="p52375209428"></a><a name="p52375209428"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p10131185111431"><a name="p10131185111431"></a><a name="p10131185111431"></a>x</p>
</td>
</tr>
<tr id="row492472211413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1323713202422"><a name="p1323713202422"></a><a name="p1323713202422"></a>查询绑定任务信息</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p197414274317"><a name="p197414274317"></a><a name="p197414274317"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p877915444439"><a name="p877915444439"></a><a name="p877915444439"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p12237102019429"><a name="p12237102019429"></a><a name="p12237102019429"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p122371120184211"><a name="p122371120184211"></a><a name="p122371120184211"></a>√</p>
</td>
</tr>
<tr id="row16923162214416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p20237132011424"><a name="p20237132011424"></a><a name="p20237132011424"></a>查询失败的任务</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p10827144664313"><a name="p10827144664313"></a><a name="p10827144664313"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p18158114811432"><a name="p18158114811432"></a><a name="p18158114811432"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p11237182015423"><a name="p11237182015423"></a><a name="p11237182015423"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p172371420184216"><a name="p172371420184216"></a><a name="p172371420184216"></a>√</p>
</td>
</tr>
<tr id="row1016342994110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p112371220104212"><a name="p112371220104212"></a><a name="p112371220104212"></a>删除所有失败的任务</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p178276461438"><a name="p178276461438"></a><a name="p178276461438"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p18158184874319"><a name="p18158184874319"></a><a name="p18158184874319"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p14237112034214"><a name="p14237112034214"></a><a name="p14237112034214"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p92745610436"><a name="p92745610436"></a><a name="p92745610436"></a>x</p>
</td>
</tr>
<tr id="row91621029164119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p17237102084218"><a name="p17237102084218"></a><a name="p17237102084218"></a>删除失败的任务</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p158271546144316"><a name="p158271546144316"></a><a name="p158271546144316"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p161586488439"><a name="p161586488439"></a><a name="p161586488439"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p10237820134220"><a name="p10237820134220"></a><a name="p10237820134220"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p12279569433"><a name="p12279569433"></a><a name="p12279569433"></a>x</p>
</td>
</tr>
<tr id="row1716102924110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p62371020134210"><a name="p62371020134210"></a><a name="p62371020134210"></a>查询正在处理的任务</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p10827194616434"><a name="p10827194616434"></a><a name="p10827194616434"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1115884874316"><a name="p1115884874316"></a><a name="p1115884874316"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p14237182012428"><a name="p14237182012428"></a><a name="p14237182012428"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p123710201424"><a name="p123710201424"></a><a name="p123710201424"></a>√</p>
</td>
</tr>
</tbody>
</table>

## 示例流程<a name="section882111167912"></a>

**图 1**  给用户授权DEW权限流程<a name="fig23111471897"></a>  
![](figures/给用户授权DEW权限流程.png "给用户授权DEW权限流程")

1.  <a name="li960014441019"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/iam_03_0001.html)

    在IAM控制台创建用户组，并授予加密密钥所有权限“KMS CMKFullAccess“。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/iam_02_0001.html)

    在IAM控制台创建用户，并将其加入[1](#li960014441019)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，切换至授权区域，验证权限。

    -   在“服务列表“中选择数据加密服务，进入DEW主界面，选择“密钥对管理“，若提示权限不足，表示“KMS CMKFullAccess“已生效。
    -   在“服务列表“中选择除数据加密服务外的任一服务，若提示权限不足，表示“KMS CMKFullAccess“已生效。

