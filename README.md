# wmt_ai_coding_study
My AI Coding study

## (No install under Windows) Login deepseek

## (Fast install under Windows) install Trae or CodeBuddy or Qoder, choose CN, choose Windows, choose IDE version (not work version)
* Just free (impossible now, you can choose OpenCode) or just need to pay
* You can choose CN version or International version in different sites, like CodeBuddyCN or TraeCN or QoderCN
* ===
* CN versions IDE: 
* https://www.codebuddy.cn/ide/  
* https://www.trae.cn/ide/download  
* https://qoder.com.cn/download  
* ====
* EN versions IDE:
* https://www.trae.ai  
* https://www.codebuddy.com/product  
* https://qoder.com/en/download  

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

## Aliyun server install claude code CLI version
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

## Install CC-Switch and Desktop version of Cluade Code
* (TODO)


