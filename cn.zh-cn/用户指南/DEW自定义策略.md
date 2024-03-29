# DEW自定义策略<a name="dew_01_0161"></a>

如果系统预置的DEW权限，不满足您的授权要求，可以创建自定义策略。自定义策略中可以添加的授权项（Action）请参见[权限及授权项说明](https://support.huaweicloud.com/api-dew/dew_02_0308.html)。

目前华为云支持以下两种方式创建自定义策略：

-   可视化视图创建自定义策略：无需了解策略语法，按可视化视图导航栏选择策略内容，可自动生成策略。

    创建KMS自定义策略时：

    -   “云服务“：数据加密服务（KMS）。
    -   “操作“：根据您的需求进行选择。
    -   “选择资源（可选）“：“资源“选择“特定资源“，“KeyId“选择“通过资源路径指定“时，“路径“为创建密钥时生成的ID，可参考“查看密钥“章节获取ID。

-   JSON视图创建自定义策略：可以在选择策略模板后，根据具体需求编辑策略内容；也可以直接在编辑框内编写JSON格式的策略内容。具体创建步骤请参见：[创建自定义策略](https://support.huaweicloud.com/usermanual-iam/iam_01_0605.html)。本章为您介绍常用的DEW自定义策略样例。

## DEW自定义策略样例<a name="zh-cn_topic_0195548199_section1435112710517"></a>

-   示例：授权用户创建密钥

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Allow",
                "Action": [
                    "kms:cmk:create",
                    "kms:cmk:getMaterial",
                    "kms:cmkTag:create",
                    "kms:cmkTag:batch",
                    "kms:cmk:importMaterial"
                ]
            }
        ]
    }
    ```

-   示例：拒绝用户删除密钥标签

    拒绝策略需要同时配合其他策略使用，否则没有实际作用。用户被授予的策略中，一个授权项的作用如果同时存在Allow和Deny，则遵循Deny优先。

    如果您给用户授予“KMS Administrator“的系统策略，但不希望用户拥有“KMS Administrator“中删除密钥标签权限（kms:cmkTag:delete），您可以创建一条相同Action的自定义策略，并将自定义策略的Effect设置为Deny，然后同时将“KMS Administrator“和拒绝策略授予用户，根据Deny优先原则用户可以对密钥对执行除了删除密钥标签的所有操作。以下策略样例表示：拒绝用户删除密钥标签。

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Deny",
                "Action": [
                    "kms:cmkTag:delete"
                ]
            }
        ]
    }
    ```

-   示例：授权用户使用密钥

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Allow",
                "Action": [
                    "kms:dek:crypto",
                    "kms:cmk:get",
                    "kms:cmk:crypto",
                    "kms:cmk:generate",
                    "kms:cmk:list"
                ]
            }
        ]
    }
    ```

-   示例：多个授权项策略

    一个自定义策略中可以包含多个授权项，且除了可以包含本服务的授权项外，还可以包含其他服务的授权项，可以包含的其他服务必须跟本服务同属性，即都是项目级服务。多个授权语句策略描述如下：

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Allow",
                "Action": [
                    "rds:task:list"
                ]
            },
            {
                "Effect": "Allow",
                "Action": [
                    "kms:dek:crypto",
                    "kms:cmk:get",
                    "kms:cmk:crypto",
                    "kms:cmk:generate",
                    "kms:cmk:list"
                ]
            }
        ]
    }
    ```

