# EVS服务端加密<a name="dew_01_0008"></a>

-   用户购买磁盘时，可以选择“高级配置  \>  现在配置  \>  加密“，使用KMS提供的密钥来加密磁盘上的数据，如[图1](#fig1372118163416)所示。更多信息请参见《云硬盘用户指南》。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >当用户需要使用磁盘加密功能时，需要授权云硬盘访问密钥管理。如果用户有授权资格，则可直接授权。如果权限不足，需先联系Security Administrator权限用户添加Security Administrator权限，然后重新操作。详细信息请参见《云硬盘用户指南》。  

    **图 1**  EVS服务端加密<a name="fig1372118163416"></a>  
    ![](figures/EVS服务端加密.png "EVS服务端加密")

    可供选择的用户主密钥包含以下两种：

    -   KMS为使用EVS（Elastic Volume Service，EVS）的用户创建一个默认主密钥“evs/default“。
    -   用户通过KMS界面创建的非默认主密钥。

-   用户也可以通过调用EVS API接口购买加密磁盘，详情请参考《云硬盘API参考》。

