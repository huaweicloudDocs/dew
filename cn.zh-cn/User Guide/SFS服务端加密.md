# SFS服务端加密<a name="ZH-CN_TOPIC_0139165811"></a>

-   用户通过弹性文件服务（Scalable File Service，SFS）创建文件系统时，可以选择“KMS加密“，使用KMS提供的密钥来加密文件系统，如[图1](#fig1357418312618)所示。更多信息请参见《弹性文件服务用户指南》。

    **图 1**  SFS服务端加密<a name="fig1357418312618"></a>  
    ![](figures/SFS服务端加密.png "SFS服务端加密")

    可供选择的用户主密钥包含以下两种：

    -   KMS为使用SFS（Scalable File Service，SFS）的用户创建一个默认主密钥“sfs/default“。
    -   用户通过KMS界面创建的非默认主密钥。

-   用户也可以通过调用SFS API接口创建加密的文件系统，详情请参考《弹性文件服务API参考》。

