# Windows cmd 命令行 tab 键 快速补全

1. 打开注册表编辑器：

   快捷键：`Win + R`

   输入：`regedit`

2. 找到 `计算机 > HKEY_LOCAL_MACHINE \ SOFTWARE \ Microsoft \ Command Processor`

   双击打开 `CompletionChar` ，设置：

   数值数据： `9`

   基数： `十进制`

   确定后，打开 cmd 就可以使用 tab 键 快速补全了
