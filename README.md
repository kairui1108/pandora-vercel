# 开源项目可以魔改，但请保留原作者信息！！

# Pandora-Vercel
本项目修改了 [Pandora-Cloud](https://github.com/pengzhile/pandora-cloud) 的代码结构，使其能够在 [Vercel](https://vercel.com) 以及 [Zeabur](https://Zeabur.com)、[Railway](https://railway.app) 等平台部署。主要以支持 Vercel 为主，包含 api 反代以及 fakeopen 反代。  

## 一键部署
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fchrysoljq%2Fpandora-vercel&project-name=pandora-vercel&framework=other)
+ 测试网站 [https://pandora-vercel-lovat.vercel.app](https://pandora-vercel-lovat.vercel.app)
+ 本地运行
```bash
npm install -g vercel
vercel dev
```

## 自动更新
若要自动同步本仓库，可参考教程 [保持更新](https://github.com/Yidadaa/ChatGPT-Next-Web/blob/main/README_CN.md#%E4%BF%9D%E6%8C%81%E6%9B%B4%E6%96%B0)。

## **环境变量**
#### `CHATGPT_API_PREFIX`  
对话 api 请求地址，默认为 `https://ai.fakeopen.com`，可以设置为你的部署后的域名（仅限 vercel），如测试网址 `https://pandora-vercel-lovat.vercel.app`，或其他反向代理地址（任意平台）。

#### `LOGIN_LOCAL`  
是否启用账号密码登录。Pandora 现已支持直接登录，故默认为 `True`或 1。
