# 使用私钥获取Windows ECS的登录密码<a name="dew_01_0086"></a>

登录Windows操作系统的弹性云服务器时，需要使用密码方式登录。此时，用户需要先根据购买弹性云服务器时下载的私钥文件，获取该弹性云服务器初始安装时系统生成的管理员密码（Administrator帐户或Cloudbase-init设置的帐户）。该密码为随机密码，安全性高，请放心使用。

用户可以通过管理控制台获取Windows弹性云服务器的登录密码。

## 前提条件<a name="section9399145913169"></a>

已获取登录弹性云服务器的私钥文件（“.pem“格式）。

## 约束条件<a name="section1950021353511"></a>

-   为安全起见，建议用户获取初始密码后，执行清除密码操作，清除系统中记录的初始密码信息。

    该操作不会影响弹性云服务器的正常登录与运行。清除密码后，系统不能恢复获取密码功能，因此，请在执行清除密码操作前，记录弹性云服务器密码信息。详细信息请参见《弹性云服务器用户指南》。

-   用户也可以通过调用API接口的方式获取Windows弹性云服务器的初始密码，请参考《弹性云服务器API参考》。
-   获取的弹性云服务器的私钥文件必须是“.pem“格式。

    若是“.ppk“格式文件，请参考[如何将“.ppk”格式的私钥文件转化为“.pem”格式](https://support.huaweicloud.com/dew_faq/dew_01_0099.html)进行转换。

## 操作步骤<a name="section7349054173814"></a>

1.  [登录管理控制台](https://console.huaweicloud.com)。
2.  单击管理控制台左上角的![](figures/icon_region-14.png)，选择区域或项目。
3.  单击![](figures/icon-servicelist.png)，选择“计算 \> 弹性云服务器“。
4.  在弹性云服务器列表，选择待获取密码的弹性云服务器。
5.  选择“操作 \> 更多“，单击“获取密码“。
6.  通过密钥文件获取密码，有以下两种方式：
    -   单击“选择文件“，从本地上传密钥文件。
    -   将密钥文件内容复制粘贴在空白文本框中。

7.  单击“获取密码“，获取随机密码。

