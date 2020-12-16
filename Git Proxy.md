# GitHub 设置和取消代理，加速 git clone

## git 设置代理

> git config --global http.proxy `http://127.0.0.1:`**_1087_**

## git 取消代理

> git config --global --unset http.proxy

## 针对 github.com 设置代理

> git config --global http.`https://github.com`.proxy `http://127.0.0.1:`**_1087_**

## 取消 github.com 代理

> git config --global --unset http.`https://github.com`.proxy

### **`注意`**：设置代理需要科(翻)学(墙)上网，后面的`端口号(1087)`要和科(翻)学(墙)上网 `Http 代理监听端口号` 相同
