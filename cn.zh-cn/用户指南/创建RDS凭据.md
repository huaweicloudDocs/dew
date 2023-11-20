# 创建RDS凭据<a name="dew_01_2003"></a>

该任务指导用户通过凭据管理界面创建通RDS凭据

创建新的凭据，并将凭据值存入凭据的初始版本，初始版本的状态被标记为“SYSCURRENT”。

## 约束条件<a name="section1901mcpsimp"></a>

-   用户最多可创建200个凭据。
-   默认使用凭据管理为您创建的默认密钥“csms/default”作为当前凭据的加密密钥。您也可以前往KMS服务页面创建自定义对称密钥，并使用自定义加密密钥。
-   RDS凭据支持的数据库引擎为：MySQL、PostgreSQL。暂不支持SQL Server数据库。

## 创建通用凭据<a name="section1906mcpsimp"></a>

1.  [登录管理控制台](https://console.huaweicloud.com)。
2.  单击管理控制台左上角![](figures/icon_region-6.png)，选择区域或项目。
3.  单击页面左侧![](figures/icon-servicelist-7.png)，选择“安全与合规  \>  数据加密服务“，默认进入“密钥管理“界面。
4.  在左侧导航树中，选择“凭据管理“，进入“凭据管理“页面。
5.  单击“创建凭据”，选择RDS实例凭据，如[图 RDS实力凭据](#fig105717529331)所示。

    **图 1**  RDS实力凭据<a name="fig105717529331"></a>  
    ![](figures/RDS实力凭据.png "RDS实力凭据")

6.  在弹出的“创建凭据“对话框中，填写参数，参数说明如[表 RDS凭据参数说明](#table1917mcpsimp)所示。

    **表 1**  RDS凭据参数说明

    <a name="table1917mcpsimp"></a>
    <table><thead align="left"><tr id="row1922mcpsimp"><th class="cellrowborder" valign="top" width="21.83%" id="mcps1.2.3.1.1"><p id="p031565710406"><a name="p031565710406"></a><a name="p031565710406"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="78.17%" id="mcps1.2.3.1.2"><p id="p9100175994016"><a name="p9100175994016"></a><a name="p9100175994016"></a>参数说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1927mcpsimp"><td class="cellrowborder" valign="top" width="21.83%" headers="mcps1.2.3.1.1 "><p id="p177811034154115"><a name="p177811034154115"></a><a name="p177811034154115"></a>凭据名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.17%" headers="mcps1.2.3.1.2 "><p id="p2148336194117"><a name="p2148336194117"></a><a name="p2148336194117"></a>待创建凭据的名称</p>
    </td>
    </tr>
    <tr id="row1932mcpsimp"><td class="cellrowborder" valign="top" width="21.83%" headers="mcps1.2.3.1.1 "><p id="p1730153914114"><a name="p1730153914114"></a><a name="p1730153914114"></a>企业项目</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.17%" headers="mcps1.2.3.1.2 "><p id="p10252173774114"><a name="p10252173774114"></a><a name="p10252173774114"></a>该参数针对企业用户使用。如果您是企业用户，且已创建企业项目，则请从下拉列表中为密钥选择需要绑定的企业项目，默认项目为“default”。</p>
    <p id="p77203415412"><a name="p77203415412"></a><a name="p77203415412"></a>未开通企业管理的用户页面则没有“企业项目”参数项，无需进行配置。</p>
    </td>
    </tr>
    <tr id="row1939mcpsimp"><td class="cellrowborder" valign="top" width="21.83%" headers="mcps1.2.3.1.1 "><p id="p1954053174213"><a name="p1954053174213"></a><a name="p1954053174213"></a>RDS实例</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.17%" headers="mcps1.2.3.1.2 "><p id="p4509175712415"><a name="p4509175712415"></a><a name="p4509175712415"></a>选择用户通过RDS控制台创建的实例名称（目前只适用于MySQL数据库）</p>
    </td>
    </tr>
    <tr id="row1944mcpsimp"><td class="cellrowborder" valign="top" width="21.83%" headers="mcps1.2.3.1.1 "><p id="p8764104184216"><a name="p8764104184216"></a><a name="p8764104184216"></a>设置凭据值</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.17%" headers="mcps1.2.3.1.2 "><p id="p315616724213"><a name="p315616724213"></a><a name="p315616724213"></a>待加密的用户凭据键/值和明文凭据。</p>
    <a name="ul122881320173619"></a><a name="ul122881320173619"></a><ul id="ul122881320173619"><li>选择单用户轮转时，需要填入一个可使用的数据库账号。</li><li>选择双用户轮转时，需要填入两个可使用的数据库账号。</li></ul>
    <p id="p149161712104218"><a name="p149161712104218"></a><a name="p149161712104218"></a>具体差异可以参考凭据概述中的<a href="轮转策略.md">轮转策略</a>。</p>
    </td>
    </tr>
    <tr id="row1952mcpsimp"><td class="cellrowborder" valign="top" width="21.83%" headers="mcps1.2.3.1.1 "><p id="p3249181511421"><a name="p3249181511421"></a><a name="p3249181511421"></a>描述信息</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.17%" headers="mcps1.2.3.1.2 "><p id="p11417185428"><a name="p11417185428"></a><a name="p11417185428"></a>凭据的描述信息</p>
    </td>
    </tr>
    <tr id="row1957mcpsimp"><td class="cellrowborder" valign="top" width="21.83%" headers="mcps1.2.3.1.1 "><p id="p113327161422"><a name="p113327161422"></a><a name="p113327161422"></a>KMS加密</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.17%" headers="mcps1.2.3.1.2 "><p id="p1261116192423"><a name="p1261116192423"></a><a name="p1261116192423"></a>选择默认主密钥“csms/default”或用户在KMS已创建的用户密钥。</p>
    <div class="note" id="note95962316372"><a name="note95962316372"></a><a name="note95962316372"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p19597193115379"><a name="p19597193115379"></a><a name="p19597193115379"></a>默认使用凭据管理为您创建的默认密钥“csms/default”作为当前凭据的加密密钥。您也可以前往KMS服务页面创建自定义密钥，使用自定义密钥作为加密密钥，在KMS创建用户密钥的操作，请参见<a href="创建密钥.md">创建密钥</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row67961922135510"><td class="cellrowborder" valign="top" width="21.83%" headers="mcps1.2.3.1.1 "><p id="p8796152219552"><a name="p8796152219552"></a><a name="p8796152219552"></a>关联事件</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.17%" headers="mcps1.2.3.1.2 "><p id="p107961225555"><a name="p107961225555"></a><a name="p107961225555"></a>为凭据选择关联事件，可以查看凭据轮转、版本过期等信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“下一步“，选择轮转周期。

    >![](public_sys-resources/icon-notice.gif) **须知：** 
    >若自动轮转开关未打开，凭据需进行手动轮转。后续若需开启自动轮转，可在凭据详情页面单击“设置轮转策略“，开启自动轮转并设置轮转周期。

1.  打开自动轮转开关，选择轮转周期，可选择已有轮转周期或者自定义设置轮转周期。

    自定义设置轮转周期的取值为6-8760小时，默认选择6小时。

    **图 2**  选择轮转周期<a name="fig977493164211"></a>  
    ![](figures/选择轮转周期.png "选择轮转周期")

2.  单击“下一步“，确认创建的信息。

    **图 3**  凭据信息<a name="fig1565233720428"></a>  
    ![](figures/凭据信息.png "凭据信息")

3.  单击“确定“，凭据创建完成，页面右上角提示创建凭据成功。
4.  用户可在凭据列表查看已完成创建的凭据，如[图 凭据列表](#fig2556193664313)所示，凭据默认状态为“启用”。

    **图 4**  凭据列表<a name="fig2556193664313"></a>  
    ![](figures/凭据列表.png "凭据列表")

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >凭据与CCE服务集成，通过插件将凭据挂载至业务Pod内，将敏感信息与集群环境解耦，有效避免程序硬编码或明文配置等问题导致的敏感信息泄密，具体操作参见[CCE密钥管理](https://support.huaweicloud.com/usermanual-cce/cce_10_0370.html)。

