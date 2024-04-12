<p align="center">
  <img src="https://socialify.git.ci/Junyi-99/Shadowrocket-Modules/image?description=1&language=1&name=1&owner=1&stargazers=1&theme=Light" alt="Shadowrocket-Modules" width="640" height="320" />
</p>

# 这是啥

你是不是也烦死了，一不小心就在小红书、淘宝上看短视频看到猪都吃晚饭了？纯靠意志力去戒短视频，那是天方夜谭，多少人盯着你那点可怜的注意力使劲，这个项目就是要帮你从根上切断短视频的诱惑。

# 什么原理

**直接切断流量**：不是屏蔽应用，也不是提醒你。我们直接在网络层面把短视频的流量给切了，简单粗暴。

# 怎么用

1. 在 Shadowrocket 里，设置全局路由为 “配置”
2. 在 Shadowrocket 进入配置选项卡 -> 模块 -> 新建模块 -> 然后粘贴 .module 文件里的内容就好了
3. 开启 Shadowrocket 的 HTTPS 解密功能
   1. Shadowrocket 配置选项卡 -> 右上角加号 -> 从给定的 URL 下载配置 -> URL 输入 `URL`
   2. 点击 “短视频过滤.conf” -> 编辑配置 -> HTTPS 解密 -> 启用 HTTPS 解密（打勾）
   3. 当你勾选 “启用 HTTPS 解密” 之后，会弹出来证书窗口，点击生成新的 CA 证书
   4. **安装** CA 证书到 iPhone
   5. 按照提示，前往 iPhone 设置 -> 通用 -> 关于本机 -> 证书信任设置 -> **信任**刚刚添加的证书
5. 开启 Shadowrocket ，设置结束

# 常见问题

Q: 模块和规则的优先级是怎么样的？模块与模块间规则的优先级是怎样的？

A: 模块规则优先于配置规则。模块列表规则优先级从上到下

# 其他说明

本仓库不提供 Shadowrocket 安装的教程
