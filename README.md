# wmt_ai_coding_study
My AI Coding study

## (No install under Windows) Login deepseek or bigmodel GLM
* https://chat.deepseek.com  
* https://bigmodel.cn/trialcenter/modeltrial/text  
* But you can't write the files  

## (Fast install under Windows) install Trae or CodeBuddy or Qoder, choose CN, choose Windows, choose IDE version (not work version)
* Just free (impossible now, you can choose OpenCode) or just need to pay
* You can choose CN version or International version in different sites, like CodeBuddyCN or TraeCN or QoderCN
* ===
* CN versions IDE: 
* https://www.trae.cn/ide/download  
* https://www.codebuddy.cn/ide/  
* https://qoder.com.cn/download  
* ====
* EN versions IDE:
* https://www.trae.ai  
* https://www.codebuddy.com/product  
* https://qoder.com/en/download
* ===
* https://www.aliyun.com/benefit/scene/qoder

## Aliyun cloud server install openclaw
* reset system, choose openclaw version, need backup data.
* aliyun panel->app detail->models-choose deepseek->input key
* aliyun panel->app detail->channels-choose wechat->qrcode bind wechat
```
重置系统，选龙虾版本，需要先备份
在aliyun面板-模型-选择deepseek-输入key
在aliyun面板-通道（频道）-下拉选择微信-用微信扫码绑定
```
* CLI usage see: https://github.com/openclaw/openclaw  
https://docs.openclaw.ai/web/tui  
* Full Install: openclaw onboard --install-daemon  
* Small Install: openclaw configure
* (NOT GOOD) CLI Talk: openclaw
* CLI Talk: openclaw chat
* CLI Talk: openclaw tui
* Web Browser Talk: openclaw dashboard

## (For Claude Code CLI Version under Linux) Aliyun server install claude code CLI version
* sudo npm install -g @anthropic-ai/claude-code
```
Sometimes just 'npm install -g @anthropic-ai/claude-code', but server can't do this
```
* https://platform.minimaxi.com/docs/token-plan/claude-code#手动编辑配置文件
```
# Stpe1: 编辑或创建 Claude Code 的配置文件
# MacOS & Linux 为 `~/.claude/settings.json`
# Windows 为`用户目录/.claude/settings.json`
# `MINIMAX_API_KEY` 需替换为您的 MiniMax API Key
# 环境变量 `ANTHROPIC_AUTH_TOKEN` 和 `ANTHROPIC_BASE_URL` 优先级高于配置文件
{
  "env": {
    "ANTHROPIC_BASE_URL": "https://api.minimaxi.com/anthropic",
    "ANTHROPIC_AUTH_TOKEN": "MINIMAX_API_KEY",
    "API_TIMEOUT_MS": "3000000",
    "CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC": "1",
    "ANTHROPIC_MODEL": "MiniMax-M3",
    "ANTHROPIC_DEFAULT_SONNET_MODEL": "MiniMax-M3",
    "ANTHROPIC_DEFAULT_OPUS_MODEL": "MiniMax-M3",
    "ANTHROPIC_DEFAULT_HAIKU_MODEL": "MiniMax-M3"
  }
}
```
```
{
  "env": {
    "ANTHROPIC_BASE_URL": "https://api.minimaxi.com/anthropic",
    "ANTHROPIC_AUTH_TOKEN": "<YOUR_MINIMAX_API_KEY>",
    "API_TIMEOUT_MS": "3000000",
    "CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC": 1,
    "ANTHROPIC_MODEL": "MiniMax-M2.7",
    "ANTHROPIC_SMALL_FAST_MODEL": "MiniMax-M2.7",
    "ANTHROPIC_DEFAULT_SONNET_MODEL": "MiniMax-M2.7",
    "ANTHROPIC_DEFAULT_OPUS_MODEL": "MiniMax-M2.7",
    "ANTHROPIC_DEFAULT_HAIKU_MODEL": "MiniMax-M2.7"
  }
}
```
* 如果执行过claude的话可以新增一行hasCompletedOnboarding(**不是覆盖**)
```
# Step2: 编辑或新增 `.claude.json` 文件
# MacOS & Linux 为 `~/.claude.json`
# Windows 为`用户目录/.claude.json`
# 新增 `hasCompletedOnboarding` 参数
{
  "hasCompletedOnboarding": true
}
```
* https://platform.kimi.com/docs/guide/agent-support#macos-和-linux-2
```
# Linux/macOS 启动高速版 kimi-k2.5 模型
export ANTHROPIC_BASE_URL=https://api.moonshot.cn/anthropic
export ANTHROPIC_AUTH_TOKEN=${YOUR_MOONSHOT_API_KEY}
export ANTHROPIC_MODEL=kimi-k2.5
export ANTHROPIC_DEFAULT_OPUS_MODEL=kimi-k2.5
export ANTHROPIC_DEFAULT_SONNET_MODEL=kimi-k2.5
export ANTHROPIC_DEFAULT_HAIKU_MODEL=kimi-k2.5
export CLAUDE_CODE_SUBAGENT_MODEL=kimi-k2.5
export ENABLE_TOOL_SEARCH=false
claude
```
```
{
  "env": {
    "ANTHROPIC_BASE_URL": "https://api.kimi.com/coding/",
    "ANTHROPIC_AUTH_TOKEN": "<YOUR_KIMI_API_KEY>",
    "API_TIMEOUT_MS": "3000000",
    "CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC": 1,
    "ANTHROPIC_MODEL": "kimi-for-coding",
    "ANTHROPIC_SMALL_FAST_MODEL": "kimi-for-coding",
    "ANTHROPIC_DEFAULT_SONNET_MODEL": "kimi-for-coding",
    "ANTHROPIC_DEFAULT_OPUS_MODEL": "kimi-for-coding",
    "ANTHROPIC_DEFAULT_HAIKU_MODEL": "kimi-for-coding"
  }
}
```
* https://api-docs.deepseek.com/zh-cn/guides/coding_agents  
* https://api-docs.deepseek.com/zh-cn/quick_start/agent_integrations/claude_code  
```
export ANTHROPIC_BASE_URL=https://api.deepseek.com/anthropic
export ANTHROPIC_AUTH_TOKEN=<你的 DeepSeek API Key>
export ANTHROPIC_MODEL=deepseek-v4-pro[1m]
export ANTHROPIC_DEFAULT_OPUS_MODEL=deepseek-v4-pro[1m]
export ANTHROPIC_DEFAULT_SONNET_MODEL=deepseek-v4-pro[1m]
export ANTHROPIC_DEFAULT_HAIKU_MODEL=deepseek-v4-flash
export CLAUDE_CODE_SUBAGENT_MODEL=deepseek-v4-flash
export CLAUDE_CODE_EFFORT_LEVEL=max
```
* 如果你用cc-switch就知道为什么要这样做，因为claude有三个模型需要映射
* 但最好不要用cc-switch，因为有可能会装不上cc-switch，除非windows上用GUI版的claude code就最好用cc-switch
* 而且cc-switch很麻烦，需要照着步骤做，反而不如改配置文件快
* https://docs.bigmodel.cn/cn/coding-plan/tool/claude  

## (TODO) (For Claude Code Desktop Version under Windows) Install CC-Switch and Desktop version of Cluade Code
* (Be careful malware) Install Claude Code Desktop, Claude-xxx.exe and Claude-xxx.msix    
https://claude.com/download  
https://github.com/ProjectAILeap/claude-code-releases/releases  
* (Optional, if you don't do this, You can't use Cowork function in Claude.exe)  
PowerShell：Add-AppxPackage -Path "Claude.msix"  
* Configure Claude Code 3P
```
Open Claude from the start menu. If the window appears blank, it is because Claude has rejected the domestic IP address. Please "turn on VPN" or "computer disconnected" before reopening Claude to see the menu entrance in the upper left corner of the window;
Do not log in to Claude's account;
Firstly, click on the window menu "Help>Troubleshooting>Enable Developer Mode", and then click "Enable" to confirm;
Then click on the window menu "Developer>Configure Third Party Inference..." to open the "Configure Third party Inference" settings window;
To set the "Connection" of the window, usually only the following three items need to be filled in. It is recommended to use it with CC Switch:
Gateway base URL： http://127.0.0.1:15721
Gateway API key: a [any string]
Model list: Add at least one model ID starting with "claude -", such as "claude opus" (because Claude filtered the model ID, it was mapped to the real large model ID through CC Switch)
Then click the "Apply locally" button to confirm, and click "Relaunch now" to immediately rerun and take effect
(Note: After setting up a third-party large model, there is no need to "turn on VPN" or "disconnect computer network")
(Note: If a third-party large model accepts any model ID - similar to the default model ID - then it can directly use the Anthropic protocol address and API Key of this large model without CC Switch)

If prompted to install Git at runtime, go to https://git-scm.com/install/windows Download and install Git, then rerun Claude Desktop

Download and update Claude Code command-line version
From https://github.com/anthropics/claude-code/releases Download the latest Claude Code command-line version, such as claude-win32-x64.zip for v2.1.139（ https://github.com/anthropics/claude-code/releases/download/v2.1.139/claude-win32-x64.zip ）Then extract the file 'claude.exe' (note: the properties of the exe file can be viewed by the version number)

Open the folder "C:\Users\System Account\AppData\Local\Claude 3p\Claude code\2.1.128\" (note: the last folder name may be a different version number, which should be the command line version number associated with the desktop);
Copy the new version file 'claude. exe' to this folder (as it will be called on the desktop);
Additionally, if this folder does not have the file '.verified', you will need to manually create a zero byte file of this size;

Add this folder path to the system environment variable Path, and you can manually call the Claude Code command-line version (open the terminal, cd the working directory, and enter claude);
```
* https://www.luoli.monster/2026/05/08/claude-code-for-vs-codecc-switchdeepseek-v4%e9%85%8d%e7%bd%ae/  
Claude Code for VS Code+cc-switch+deepseek v4配置  

## OpenCode, some free models like deepseek flash
* https://github.com/anomalyco/opencode
* https://opencode.ai/download
* ===
* (Not Recommended) Very old version, but can be upgrade to the newest version
* (Not Recommended) https://opencodeai.cn

## Cursor
* https://cursor.com/cn
* https://cursor.com/cn/docs
* 如果你想用外国的AI, 除了中转站(转发)和Copilot, 可能这是最好的选择, 因为Cursor支持alipay支付
* 当然cursor比较贵, 而且不是最好的, 但能用已经很好了, 我认为至少比中转站(转发)和Copilot好用很多, 中转站容易断开, Copilot很难支付  
