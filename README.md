# Intent Guardian Wallet

imToken 十周年「AI 共创，生成你想要的钱包」活动作品 Demo。

## 作品简介

Intent Guardian Wallet 是一个安全优先的 AI 意图钱包原型。页面支持在浏览器本地创建测试钱包，输出 BIP39 助记词、Ethereum 地址和加密 Keystore JSON；用户也可以导入测试助记词。用户用自然语言描述转账、兑换、授权管理或安全检查目标，AI 生成签名前草稿；系统在确认页展示资产、金额、地址、网络、手续费和风险解释；用户确认后可用本地测试钱包完成消息签名。

## Token Core 关联说明

本作品基于 Token Core 相关公开材料中的钱包核心能力做交互原型设计：

- 本地助记词生成与 Keystore 加密的安全边界
- 多链账户与资产管理
- 交易签名前的用户确认
- 将签名内容翻译成可理解信息的清晰签名体验

本网页是活动展示 Demo。它会生成真实格式的测试助记词，但不上传、不保存到服务器；不要把页面生成的助记词用于主网资产，也不要输入真实钱包助记词。

## 运行方式

直接打开 `index.html` 即可运行。

如果要用本地服务预览：

```bash
python3 -m http.server 8080
```

然后访问 `http://localhost:8080/imtoken-ai-wallet/`。

## GitHub Pages 发布

1. 在 GitHub 新建仓库，例如 `imtoken-ai-wallet`。
2. 上传本文件夹内的 `index.html`、`README.md` 和 `assets/intent-wallet-map.svg`。
3. 在仓库 Settings -> Pages 中选择 Deploy from a branch，分支选 `main`，目录选 `/root`。
4. 发布后作品链接通常是：

```text
https://你的用户名.github.io/imtoken-ai-wallet/
```

## 活动提交文案

作品名称：Intent Guardian Wallet

简介：一个安全优先的 AI 意图钱包 Demo：支持浏览器本地创建测试钱包、输出助记词、生成地址和 Keystore；用户用自然语言描述转账或授权管理目标，AI 生成草稿；系统在签名前展示资产、地址、网络、手续费和风险解释，最终由用户确认后模拟签名。

Token Core 关联：使用 Token Core 相关材料中的本地 Keystore、私钥不出设备、多链账户与签名确认思路；本 Demo 在浏览器本地生成测试助记词、地址和 Keystore，不上传密钥材料，真实产品形态应由 Token Core 类钱包核心完成密钥生成、Keystore 加密和签名。
