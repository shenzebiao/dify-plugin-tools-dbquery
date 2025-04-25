## Dify 1.0 Plugin Database Query Tools


**Author:** [Junjie.M](https://github.com/junjiem)   
**Type:** tool  
**Github Repo:** [https://github.com/junjiem/dify-plugin-tools-dbquery](https://github.com/junjiem/dify-plugin-tools-dbquery)  
**Github Issues:** [issues](https://github.com/junjiem/dify-plugin-tools-dbquery/issues)


---


### Demonstration

Database Query Tools

数据库查询工具

Currently supported database types: mysql, oracle, postgresql, or mssql.

目前支持的数据库类型：mysql、oracle、postgresql、mssql。

![db_query](_assets/db_query.png)

![db_query_sql_query](_assets/db_query_sql_query.png)

![db_query_chatflow](_assets/db_query_chatflow.png)



---



### Examples 示例

- [完蛋！我被LLM包围了！（Dify1.0战绩排行版）](https://github.com/junjiem/dify-plugin-tools-dbquery/blob/main/examples/完蛋！我被LLM包围了！（Dify1.0战绩排行版）.yml)

- [完蛋！我被LLM包围了！（Dify1.0战绩排行+留言版）](https://github.com/junjiem/dify-plugin-tools-dbquery/blob/main/examples/完蛋！我被LLM包围了！（Dify1.0战绩排行+留言版）.yml)


![](_assets/llm_riddles1.png)

![](_assets/llm_riddles2.png)

![](_assets/llm_riddles3.png)



---



### FAQ

#### 1. How to Handle Errors When Installing Plugins? 安装插件时遇到异常应如何处理？

**Issue**: If you encounter the error message: plugin verification has been enabled, and the plugin you want to install has a bad signature, how to handle the issue?

**Solution**: Add the following line to the end of your .env configuration file: FORCE_VERIFYING_SIGNATURE=false
Once this field is added, the Dify platform will allow the installation of all plugins that are not listed (and thus not verified) in the Dify Marketplace.

**问题描述**：安装插件时遇到异常信息：plugin verification has been enabled, and the plugin you want to install has a bad signature，应该如何处理？

**解决办法**：在 .env 配置文件的末尾添加 FORCE_VERIFYING_SIGNATURE=false 字段即可解决该问题。
添加该字段后，Dify 平台将允许安装所有未在 Dify Marketplace 上架（审核）的插件，可能存在安全隐患。


#### 2. How to install the offline version 如何安装离线版本

Scripting tool for downloading Dify plugin package from Dify Marketplace and Github and repackaging [true] offline package (contains dependencies, no need to be connected to the Internet).

从Dify市场和Github下载Dify插件包并重新打【真】离线包（包含依赖，不需要再联网）的脚本工具。

Github Repo: https://github.com/junjiem/dify-plugin-repackaging

