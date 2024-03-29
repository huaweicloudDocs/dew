# API参考

-   [使用前必读](使用前必读.md)
    -   [概述](概述.md)
    -   [调用说明](调用说明.md)
    -   [终端节点](终端节点.md)
    -   [约束与限制](约束与限制.md)
    -   [基本概念](基本概念.md)
    -   [API版本选择建议](API版本选择建议.md)

-   [如何调用API](如何调用API.md)
    -   [构造请求](构造请求.md)
    -   [认证鉴权](认证鉴权.md)
    -   [返回结果](返回结果.md)

-   [API概览](API概览.md)
-   [API说明](API说明.md)
    -   [管理加密密钥](管理加密密钥.md)
        -   [密钥生命周期管理](密钥生命周期管理.md)
            -   [创建密钥](创建密钥.md)
            -   [启用密钥](启用密钥.md)
            -   [禁用密钥](禁用密钥.md)
            -   [计划删除密钥](计划删除密钥.md)
            -   [取消计划删除密钥](取消计划删除密钥.md)
            -   [修改密钥别名](修改密钥别名.md)
            -   [修改密钥描述](修改密钥描述.md)

        -   [数据密钥管理](数据密钥管理.md)
            -   [创建随机数](创建随机数.md)
            -   [创建数据密钥](创建数据密钥.md)
            -   [创建不含明文数据密钥](创建不含明文数据密钥.md)
            -   [加密数据密钥](加密数据密钥.md)
            -   [解密数据密钥](解密数据密钥.md)

        -   [导入密钥管理](导入密钥管理.md)
            -   [获取密钥导入参数](获取密钥导入参数.md)
            -   [导入密钥材料](导入密钥材料.md)
            -   [删除密钥材料](删除密钥材料.md)

        -   [密钥授权管理](密钥授权管理.md)
            -   [创建授权](创建授权.md)
            -   [撤销授权](撤销授权.md)
            -   [退役授权](退役授权.md)
            -   [查询授权列表](查询授权列表.md)
            -   [查询可退役授权列表](查询可退役授权列表.md)

        -   [小数据加解密](小数据加解密.md)
            -   [加密数据](加密数据.md)
            -   [解密数据](解密数据.md)

        -   [签名验签](签名验签.md)
            -   [签名数据](签名数据.md)
            -   [验证签名](验证签名.md)

        -   [密钥轮换管理](密钥轮换管理.md)
            -   [开启密钥轮换](开启密钥轮换.md)
            -   [关闭密钥轮换](关闭密钥轮换.md)
            -   [修改密钥轮换周期](修改密钥轮换周期.md)
            -   [查询密钥轮换状态](查询密钥轮换状态.md)

        -   [密钥标签管理](密钥标签管理.md)
            -   [查询密钥实例](查询密钥实例.md)
            -   [查询密钥标签](查询密钥标签.md)
            -   [添加密钥标签](添加密钥标签.md)
            -   [查询项目标签](查询项目标签.md)
            -   [批量添加删除密钥标签](批量添加删除密钥标签.md)
            -   [删除密钥标签](删除密钥标签.md)

        -   [密钥查询](密钥查询.md)
            -   [查询密钥列表](查询密钥列表.md)
            -   [查询密钥信息](查询密钥信息.md)
            -   [查询公钥信息](查询公钥信息.md)
            -   [查询实例数](查询实例数.md)
            -   [查询配额](查询配额.md)

        -   [查询密钥API版本信息](查询密钥API版本信息.md)
            -   [查询版本信息列表](查询版本信息列表.md)
            -   [查询指定版本信息](查询指定版本信息.md)

        -   [专属密钥库管理](专属密钥库管理.md)
            -   [创建专属密钥库](创建专属密钥库.md)
            -   [查询专属密钥库列表](查询专属密钥库列表.md)
            -   [获取专属密钥库](获取专属密钥库.md)
            -   [删除专属密钥库](删除专属密钥库.md)
            -   [启用专属密钥库](启用专属密钥库.md)
            -   [禁用专属密钥库](禁用专属密钥库.md)

    -   [管理SSH密钥对](管理SSH密钥对.md)
        -   [密钥对管理](密钥对管理.md)
            -   [创建和导入SSH密钥对](创建和导入SSH密钥对.md)
            -   [清除私钥](清除私钥.md)
            -   [查询SSH密钥对列表](查询SSH密钥对列表.md)
            -   [查询SSH密钥对详细信息](查询SSH密钥对详细信息.md)
            -   [删除SSH密钥对](删除SSH密钥对.md)
            -   [更新SSH密钥对描述](更新SSH密钥对描述.md)
            -   [导入私钥](导入私钥.md)
            -   [导出私钥](导出私钥.md)

        -   [密钥对任务管理](密钥对任务管理.md)
            -   [绑定SSH密钥对](绑定SSH密钥对.md)
            -   [解绑SSH密钥对](解绑SSH密钥对.md)
            -   [批量绑定SSH密钥对](批量绑定SSH密钥对.md)
            -   [查询任务信息](查询任务信息.md)
            -   [查询正在处理的任务信息](查询正在处理的任务信息.md)
            -   [查询失败的任务信息](查询失败的任务信息.md)
            -   [删除所有失败的任务](删除所有失败的任务.md)
            -   [删除失败的任务](删除失败的任务.md)

    -   [凭据管理服务](凭据管理服务.md)
        -   [生命周期管理](生命周期管理.md)
            -   [创建凭据](创建凭据.md)
            -   [查询凭据列表](查询凭据列表.md)
            -   [查询凭据](查询凭据.md)
            -   [更新凭据](更新凭据.md)
            -   [立即删除凭据](立即删除凭据.md)
            -   [恢复凭据对象](恢复凭据对象.md)
            -   [下载凭据备份](下载凭据备份.md)
            -   [创建凭据的定时删除任务](创建凭据的定时删除任务.md)
            -   [取消凭据的定时删除任务](取消凭据的定时删除任务.md)
            -   [轮转凭据](轮转凭据.md)

        -   [凭据版本管理](凭据版本管理.md)
            -   [创建凭据版本](创建凭据版本.md)
            -   [查询凭据的版本列表](查询凭据的版本列表.md)
            -   [更新凭据版本](更新凭据版本.md)
            -   [查询凭据的版本与凭据值](查询凭据的版本与凭据值.md)

        -   [凭据版本状态管理](凭据版本状态管理.md)
            -   [更新凭据的版本状态](更新凭据的版本状态.md)
            -   [查询凭据的版本状态](查询凭据的版本状态.md)
            -   [删除凭据的版本状态](删除凭据的版本状态.md)

        -   [凭据标签管理](凭据标签管理.md)
            -   [查询凭据实例](查询凭据实例.md)
            -   [批量添加或删除凭据标签](批量添加或删除凭据标签.md)
            -   [查询凭据标签](查询凭据标签.md)
            -   [添加凭据标签](添加凭据标签.md)
            -   [删除凭据标签](删除凭据标签.md)
            -   [查询项目标签](查询项目标签-0.md)

        -   [事件管理](事件管理.md)
            -   [创建事件](创建事件.md)
            -   [查询事件](查询事件.md)
            -   [查询事件列表](查询事件列表.md)
            -   [更新事件](更新事件.md)
            -   [立即删除事件](立即删除事件.md)
            -   [查询已触发的事件通知记录](查询已触发的事件通知记录.md)

-   [历史API](历史API.md)
    -   [管理SSH密钥对\(V2.1\)](管理SSH密钥对(V2-1).md)
        -   [查询SSH密钥对列表\(V2.1\)](查询SSH密钥对列表(V2-1).md)
        -   [查询SSH密钥对详情\(V2.1\)](查询SSH密钥对详情(V2-1).md)
        -   [创建及导入SSH密钥对\(V2.1\)](创建及导入SSH密钥对(V2-1).md)
        -   [删除SSH密钥对\(V2.1\)](删除SSH密钥对(V2-1).md)
        -   [修改密钥对描述信息\(V2.1\)](修改密钥对描述信息(V2-1).md)

    -   [管理SSH密钥对\(V2\)](管理SSH密钥对(V2).md)
        -   [查询SSH密钥对列表\(V2\)](查询SSH密钥对列表(V2).md)
        -   [查询SSH密钥对详情\(V2\)](查询SSH密钥对详情(V2).md)
        -   [创建及导入SSH密钥对\(V2\)](创建及导入SSH密钥对(V2).md)
        -   [删除SSH密钥对\(V2\)](删除SSH密钥对(V2).md)
        -   [复制SSH密钥对\(V2\)](复制SSH密钥对(V2).md)

-   [应用示例](应用示例.md)
    -   [示例1：加解密小量数据](示例1-加解密小量数据.md)
    -   [示例2：加解密大量数据](示例2-加解密大量数据.md)
    -   [示例3：查询密钥相关信息](示例3-查询密钥相关信息.md)

-   [权限和授权项](权限和授权项.md)
    -   [权限及授权项说明](权限及授权项说明.md)
    -   [加密密钥管理](加密密钥管理.md)
    -   [密钥对管理](权限章节密钥对管理.md)

-   [附录](附录.md)
    -   [状态码](状态码.md)
    -   [错误码](错误码.md)
    -   [获取项目ID](获取项目ID.md)

-   [修订记录](修订记录.md)

