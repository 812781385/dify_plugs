# dify_plugs
![cover-v5-optimized](./images/GitHub_README_if.png)
dify离线插件，用于服务器内网完全离线情况安装

### Installing Plugins via Local 通过本地安装插件
Visit the Dify platform's plugin management page, choose Local Package File to complete installation.

### Update Dify platform env  Dify平台放开限制

- your .env configuration file: Change `FORCE_VERIFYING_SIGNATURE` to `false` , the Dify platform will allow the installation of all plugins that are not listed in the Dify Marketplace.

- your .env configuration file: Change `PLUGIN_MAX_PACKAGE_SIZE` to `524288000` , and the Dify platform will allow the installation of plug-ins within 500M.

- your .env configuration file: Change `NGINX_CLIENT_MAX_BODY_SIZE` to `500M` , and the Nginx client will allow uploading content up to 500M in size.



- 在 .env 配置文件将 `FORCE_VERIFYING_SIGNATURE` 改为 `false` ，Dify 平台将允许安装所有未在 Dify Marketplace 上架（审核）的插件。

- 在 .env 配置文件将 `PLUGIN_MAX_PACKAGE_SIZE` 增大为 `524288000`，Dify 平台将允许安装 500M 大小以内的插件。

- 在 .env 配置文件将 `NGINX_CLIENT_MAX_BODY_SIZE` 增大为 `500M`，Nginx客户端将允许上传 500M 大小以内的内容。

访问 Dify 平台的插件管理页，选择通过本地插件完成安装。
![install_plugin_via_local](./images/install_plugin_via_local.png)

## 致谢
- [dify-插件重新打包](https://github.com/junjiem/dify-plugin-repackaging.git)
