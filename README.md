<p align='center'>
 <strong>MidJourney-Web</strong>
<br>
</p>



<p align='center'>
 🍎 Supercharged Experience For  MidJourney On Web UI
<br>
</p>





<div align="center">
	
  🚧 正在施工~进度80% | [查看常见部署问题 🤞](https://github.com/ConnectAI-E/MidJourney-Web/wiki/%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98%E6%B1%87%E6%80%BB)
	
</div>

<div align="center">
	<a href='https://www.connectai-e.com' target="_blank" rel="noopener noreferrer">
	<img width="800" alt="image" src="https://github-production-user-asset-6210df.s3.amazonaws.com/50035229/246644404-d8b30cab-ebae-42dd-8306-4e9904a18b65.png">
	</a>
</div>

## Feature List

- ✅ Support `/imagine`  生图操作
- ✅ Support `/upscale 1-4` 高清图生成
- ✅ Support `/variation 1-4`图片变体
- ✅ Support `/reRoll` 重新生图
- ✅ Support `/describe` 以图生文
- 🛠 Support `/describe imagine` 根据描述画图
- ✅ Support `/blend` 图片融合
- ✅ Progress percentage 绘图进度展示
- ✅ Real-time image display 实时更新绘图结果
- 🛠 Support Cn Prompt 兼容中文提示词
- 🛠 Better Better Prompt 借助GPT一键优化提示词
- 🛠 View historical drawing records 查看所有历史绘图记录
- 🛠 One-click remove picture background 一键去除图片背景
- 🛠 One-click bitmap to vector 一键位图转矢量图
- 🛠 Permission management 界面权限管理
- 🛠 Limit user availability 限制用户可用次数
- 🛠 Mobile adaptation 移动端适配
- 🛠 Account pool mechanism MJ账号池机制增加并发
  

## Quick Start

### 1. Midjourney-Api
```bash
docker run -d --name midjourney-proxy \
 -p 8080:8080 \
 -e mj.discord.guild-id=xxx \
 -e mj.discord.channel-id=xxx \
 -e mj.discord.user-token=xxx \
 -e mj.api-secret=xxx \
 --restart=always \
 novicezk/midjourney-proxy:2.2.3
```
more config info [MidJourney-Api](https://github.com/novicezk/midjourney-proxy/blob/main/docs/discord-params.md)

then check midjourney-api swagger document: http://localhost:8080/mj

<details>
    <summary>其他一键部署方式</summary>

<h3>Railway</h3>

Railway是一个提供弹性部署方案的平台，为MidJourney的调用提供了方便的海外服务。
	
参考：[midjourney-proxy - Railway 部署教程](https://github.com/novicezk/midjourney-proxy/blob/main/docs/railway-start.md)

<h3>Zeabur</h3>

Zeabur 服务器运行在国外，但是其生成的域名 *.zeabur.app 没有被污染,国内可直接访问

[![Deploy on Zeabur](https://zeabur.com/button.svg)](https://dash.zeabur.com/templates/B04F4M)


参考：[midjourney-proxy - Zeabur 部署教程](https://github.com/novicezk/midjourney-proxy/blob/main/docs/zeabur-start.md)
</details>


### 2. Midjourney-Web
```bash
## 填入midjourney-api部署的host地址、访问api的秘钥'mj.api-secret'
mv .env.example .env

pnpm install
pnpm run dev
```

<details>
    <summary>其他一键部署方式</summary>

<h3>Vercel</h3>

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/ConnectAI-E/MidJourney-Web&env=VITE_MIDJOURNEY_PROXY_URL&env=VITE_MIDJOURNEY_PROXY_API_SECRET&project-name=midjourney-web&repository-name=Midjourney-Web)
</details>


## Technology Stack
- [react](https://react.dev/)
- [vite](https://vitejs.dev/)
- [unocss](https://github.com/unocss/unocss)
- [jotai](https://jotai.org/)
- [react query](https://tanstack.com/query/v3/)

## High Resolution Example

https://github.com/ConnectAI-E/MidJourney-Web/assets/50035229/9a21b470-0919-413e-b020-ecd28837c399

<details align='center'>
    <summary> 📹 点击观看更多功能演示</summary>
    <br>
	<video src="https://github.com/ConnectAI-E/MidJourney-Web/assets/50035229/6ad2ffef-0f1a-43b4-a774-8d336511e072" controls ></video>
	<video src="https://github.com/ConnectAI-E/MidJourney-Web/raw/main/assets/50035229/7092a777-d394-445b-9332-3f4d9717c138" controls ></video>
	<video src="https://user-images.githubusercontent.com/50035229/248157796-95e6697c-5f3f-469e-8d36-2ec93d88f1c5.mp4" controls ></video>
<video src="https://github.com/ConnectAI-E/MidJourney-Web/assets/50035229/e03e3e71-e81d-4efa-ac95-bda9c703ddd7.mp4" controls ></video>




</details>

##  ConnectAI-E

| <div style="width:200px">AI</div> |             <img width=120> SDK <img width=120>              |                         Application                          |
| :-------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|              🎒OpenAI              |    [Go-OpenAI](https://github.com/ConnectAI-E/Go-OpenAI)     | [🏅Feishu-OpenAI](https://github.com/ConnectAI-E/Feishu-OpenAI), [🎖Lark-OpenAI](https://github.com/ConnectAI-E/Lark-OpenAI), [Feishu-EX-ChatGPT](https://github.com/ConnectAI-E/Feishu-EX-ChatGPT), [🎖Feishu-OpenAI-Stream-Chatbot](https://github.com/ConnectAI-E/Feishu-OpenAI-Stream-Chatbot), [Feishu-TLDR](https://github.com/ConnectAI-E/Feishu-TLDR),[Feishu-OpenAI-Amazing](https://github.com/ConnectAI-E/Feishu-OpenAI-Amazing), [Feishu-Oral-Friend](https://github.com/ConnectAI-E/Feishu-Oral-Friend), [Feishu-OpenAI-Base-Helper](https://github.com/ConnectAI-E/Feishu-OpenAI-Base-Helper), [Feishu-Vector-Knowledge-Management](https://github.com/ConnectAI-E/Feishu-Vector-Knowledge-Management), [Feishu-OpenAI-PDF-Helper](https://github.com/ConnectAI-E/Feishu-OpenAI-PDF-Helper), [🏅Dingtalk-OpenAI](https://github.com/ConnectAI-E/Dingtalk-OpenAI), [Wework-OpenAI](https://github.com/ConnectAI-E/Wework-OpenAI), [WeWork-OpenAI-Node](https://github.com/ConnectAI-E/WeWork-OpenAI-Node), [llmplugin](https://github.com/ConnectAI-E/llmplugin) |
|             🤖 AutoGPT             |                            ------                            | [🏅AutoGPT-Next-Web](https://github.com/ConnectAI-E/AutoGPT-Next-Web) |
|         🎭 Stablediffusion         |                            ------                            | [🎖Feishu-Stablediffusion](https://github.com/ConnectAI-E/Feishu-Stablediffusion) |
|           🍎 Midjourney            | [Go-Midjourney](https://github.com/ConnectAI-E/Go-Midjourney) | [🏅Feishu-Midjourney](https://github.com/ConnectAI-E/Feishu-Midjourney), [🔥MidJourney-Web](https://github.com/ConnectAI-E/MidJourney-Web), [Dingtalk-Midjourney](https://github.com/ConnectAI-E/Dingtalk-Midjourney) |
|            🍍 文心一言             |    [Go-Wenxin](https://github.com/ConnectAI-E/Go-Wenxin)     | [Feishu-Wenxin](https://github.com/ConnectAI-E/Feishu-Wenxin), [Dingtalk-Wenxin](https://github.com/ConnectAI-E/Dingtalk-Wenxin), [Wework-Wenxin](https://github.com/ConnectAI-E/Wework-Wenxin) |
|             💸 Minimax             |   [Go-Minimax](https://github.com/ConnectAI-E/Go-Minimax)    | [Feishu-Minimax](https://github.com/ConnectAI-E/Feishu-Minimax), [Dingtalk-Minimax](https://github.com/ConnectAI-E/Dingtalk-Minimax), [Wework-Minimax](https://github.com/ConnectAI-E/Wework-Minimax) |
|             ⛳️ CLAUDE              |    [Go-Claude](https://github.com/ConnectAI-E/Go-Claude)     | [Feishu-Claude](https://github.com/ConnectAI-E/Feishu-Claude), [DingTalk-Claude](https://github.com/ConnectAI-E/DingTalk-Claude), [Wework-Claude](https://github.com/ConnectAI-E/Wework-Claude) |
|              🥁 PaLM               |      [Go-PaLM](https://github.com/ConnectAI-E/go-PaLM)       | [Feishu-PaLM](https://github.com/ConnectAI-E/Feishu-PaLM),[DingTalk-PaLM](https://github.com/ConnectAI-E/DingTalk-PaLM),[Wework-PaLM](https://github.com/ConnectAI-E/Wework-PaLM) |
|             🎡 Prompt              |                            ------                            | [📖 Prompt-Engineering-Tutior](https://github.com/ConnectAI-E/Prompt-Engineering-Tutior) |
|             🍋 ChatGLM             |                            ------                            | [Feishu-ChatGLM](https://github.com/ConnectAI-E/Feishu-ChatGLM) |
|            ⛓ LangChain            |                            ------                            | [📖 LangChain-Tutior](https://github.com/ConnectAI-E/LangChain-Tutior) |
|            🪄 One-click            |                            ------                            | [🎖Awesome-One-Click-Deployment](https://github.com/ConnectAI-E/Awesome-One-Click-Deployment) |


## 沟通部署问题

<img width="220" alt="image" src="https://github.com/ConnectAI-E/MidJourney-Web/assets/50035229/f19d3d79-55c4-451a-9691-d90769c43cb4">




