# DEW监控指标说明<a name="dew_01_0236"></a>

## 功能说明<a name="section1295843318168"></a>

本节定义了数据加密服务上报云监控的基础监控指标的命名空间，监控指标列表，各项监控指标的具体含义与使用说明，用户可以通过云监控检索数据加密服务产生的监控指标和告警信息。

## 命名空间<a name="section1191118477174"></a>

密钥管理：SYS.KMS

凭据管理：SYS.CSMS

>![](public_sys-resources/icon-note.gif) **说明：** 
>命名空间是对一组资源和对象的抽象整合。在同一个集群内可创建不同的命名空间，不同命名空间中的数据彼此隔离。使得它们既可以共享同一个集群的服务，也能够互不干扰。

## 数据加密服务监控指标<a name="section847311011196"></a>

**表 1**  密钥管理支持的监控指标

<a name="table1725014565197"></a>
<table><thead align="left"><tr id="row14252175612192"><th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.1"><p id="p5252165631916"><a name="p5252165631916"></a><a name="p5252165631916"></a>指标ID</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.2"><p id="p325225619192"><a name="p325225619192"></a><a name="p325225619192"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.3"><p id="p112521856111919"><a name="p112521856111919"></a><a name="p112521856111919"></a>指标含义</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.4"><p id="p1525225617191"><a name="p1525225617191"></a><a name="p1525225617191"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="16.64667066586683%" id="mcps1.2.7.1.5"><p id="p14252056181916"><a name="p14252056181916"></a><a name="p14252056181916"></a>测量对象</p>
</th>
<th class="cellrowborder" valign="top" width="16.686662667466507%" id="mcps1.2.7.1.6"><p id="p325285691911"><a name="p325285691911"></a><a name="p325285691911"></a>监控周期（原始指标）</p>
</th>
</tr>
</thead>
<tbody><tr id="row1525265619199"><td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.1 "><p id="p87181625202213"><a name="p87181625202213"></a><a name="p87181625202213"></a>delkey_remaing_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.2 "><p id="p177181225122215"><a name="p177181225122215"></a><a name="p177181225122215"></a>密钥剩余时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.3 "><p id="p7718202517227"><a name="p7718202517227"></a><a name="p7718202517227"></a>该指标表示计划删除状态的密钥距离被删除还剩下的时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.4 "><p id="p1019195482210"><a name="p1019195482210"></a><a name="p1019195482210"></a>≥ 0 小时</p>
</td>
<td class="cellrowborder" valign="top" width="16.64667066586683%" headers="mcps1.2.7.1.5 "><p id="p225310560192"><a name="p225310560192"></a><a name="p225310560192"></a>密钥</p>
</td>
<td class="cellrowborder" valign="top" width="16.686662667466507%" headers="mcps1.2.7.1.6 "><p id="p13253125691917"><a name="p13253125691917"></a><a name="p13253125691917"></a>5分钟</p>
</td>
</tr>
<tr id="row182531156101916"><td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.1 "><p id="p95140339223"><a name="p95140339223"></a><a name="p95140339223"></a>matrial_remaing_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.2 "><p id="p1451420330228"><a name="p1451420330228"></a><a name="p1451420330228"></a>密钥材料的剩余有效时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.3 "><p id="p5514033152216"><a name="p5514033152216"></a><a name="p5514033152216"></a>该指标表示外部导入的密钥材料的剩余有效时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.4 "><p id="p10347175511229"><a name="p10347175511229"></a><a name="p10347175511229"></a>≥ 0 小时</p>
</td>
<td class="cellrowborder" valign="top" width="16.64667066586683%" headers="mcps1.2.7.1.5 "><p id="p12253205631912"><a name="p12253205631912"></a><a name="p12253205631912"></a>密钥</p>
</td>
<td class="cellrowborder" valign="top" width="16.686662667466507%" headers="mcps1.2.7.1.6 "><p id="p9253656171914"><a name="p9253656171914"></a><a name="p9253656171914"></a>5分钟</p>
</td>
</tr>
</tbody>
</table>

**表 2**  凭据管理支持的监控指标

<a name="table434281852517"></a>
<table><thead align="left"><tr id="row20343181811253"><th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.1"><p id="p19250112312516"><a name="p19250112312516"></a><a name="p19250112312516"></a>指标ID</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.2"><p id="p172509235257"><a name="p172509235257"></a><a name="p172509235257"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.3"><p id="p182501223142512"><a name="p182501223142512"></a><a name="p182501223142512"></a>指标含义</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.4"><p id="p11250623182516"><a name="p11250623182516"></a><a name="p11250623182516"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.5"><p id="p1625162316257"><a name="p1625162316257"></a><a name="p1625162316257"></a>测量对象</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.6"><p id="p16251923172510"><a name="p16251923172510"></a><a name="p16251923172510"></a>监控周期（原始指标）</p>
</th>
</tr>
</thead>
<tbody><tr id="row6343101812253"><td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.1 "><p id="p168293518251"><a name="p168293518251"></a><a name="p168293518251"></a>del_secret_remaining_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.2 "><p id="p38291151182514"><a name="p38291151182514"></a><a name="p38291151182514"></a>计划删除凭据剩余时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.3 "><p id="p1782975192510"><a name="p1782975192510"></a><a name="p1782975192510"></a>该指标表示计划删除凭据的剩余时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.4 "><p id="p534481802518"><a name="p534481802518"></a><a name="p534481802518"></a>≥ 0 小时</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.5 "><p id="p10344318132515"><a name="p10344318132515"></a><a name="p10344318132515"></a>凭据</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.6 "><p id="p33441018122520"><a name="p33441018122520"></a><a name="p33441018122520"></a>5分钟</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="section62745282261"></a>

<a name="table930414013262"></a>
<table><thead align="left"><tr id="row17304154002619"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="p183041409268"><a name="p183041409268"></a><a name="p183041409268"></a>Key</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="p15304184042610"><a name="p15304184042610"></a><a name="p15304184042610"></a>Value</p>
</th>
</tr>
</thead>
<tbody><tr id="row1630474018263"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p630404052611"><a name="p630404052611"></a><a name="p630404052611"></a>key_id</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p9305124022614"><a name="p9305124022614"></a><a name="p9305124022614"></a>密钥ID</p>
</td>
</tr>
<tr id="row11398194220272"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p13401342172712"><a name="p13401342172712"></a><a name="p13401342172712"></a>secret_id</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p194019422276"><a name="p194019422276"></a><a name="p194019422276"></a>凭据ID</p>
</td>
</tr>
</tbody>
</table>

