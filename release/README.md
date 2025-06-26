# MotaV1.0 - URL Search Tool

```
███╗   ███╗ ██████╗ ████████╗ █████╗
████╗ ████║██╔═══██╗╚══██╔══╝██╔══██╗
██╔████╔██║██║   ██║   ██║   ███████║
██║╚██╔╝██║██║   ██║   ██║   ██╔══██║
██║ ╚═╝ ██║╚██████╔╝   ██║   ██║  ██║
╚═╝     ╚═╝ ╚═════╝    ╚═╝   ╚═╝  ╚═╝
                V1.0 - URL Search Tool
                   Author: Mon2on
```

## 简介

MotaV1.0 是一个高效的URL搜索和提取工具，支持根据关键词搜索特定域名后缀的URL数据。

## 功能特点

- 🔍 **智能搜索**: 根据关键词搜索包含特定域名后缀的URL
- 🌐 **远程连接**: 客户端通过API连接到远程服务器获取数据
- 🔐 **认证机制**: 首次使用生成唯一认证码，认证后可无限制使用
- 📊 **数据提取**: 自动提取文件中的URL并保存到本地
- 🎨 **美观界面**: 彩色3D Logo和友好的用户界面
- 🖥️ **跨平台**: 支持Windows、Linux、macOS、FreeBSD等多个平台

## 支持平台

- **Windows**: 64位 (amd64) / 32位 (386)
- **Linux**: 64位 (amd64) / 32位 (386) / ARM64
- **macOS**: Intel (amd64) / Apple Silicon (arm64)
- **FreeBSD**: 64位 (amd64)

## 使用方法

### 1. 下载对应平台的客户端

从 `release/` 目录下载适合您系统的客户端：

- Windows 64位: `MotaV1.0_windows_amd64.exe`
- Windows 32位: `MotaV1.0_windows_386.exe`
- Linux 64位: `MotaV1.0_linux_amd64`
- Linux 32位: `MotaV1.0_linux_386`
- Linux ARM64: `MotaV1.0_linux_arm64`
- macOS Intel: `MotaV1.0_macos_amd64`
- macOS Apple Silicon: `MotaV1.0_macos_arm64`
- FreeBSD 64位: `MotaV1.0_freebsd_amd64`

### 2. 运行客户端

**简化使用方法（推荐）**：
```bash
# Linux/macOS/FreeBSD
./MotaV1.0_linux_amd64 .tw

# Windows
MotaV1.0_windows_amd64.exe .tw
```

**传统使用方法**：
```bash
# Linux/macOS/FreeBSD
./MotaV1.0_linux_amd64 -keyword=.tw

# Windows
MotaV1.0_windows_amd64.exe -keyword=.tw
```

### 3. 认证流程

**首次使用时**：
1. 程序会自动生成一个唯一的认证码
2. 将认证码发送给管理员
3. 管理员批准后，您就可以无限制使用

**认证前限制**：
- 未认证用户限制下载10000条URL
- 认证后可无限制下载

## 命令行参数

- **直接参数**（推荐）: 直接输入关键词
- `-h` 或 `--help`: 显示帮助信息

## 使用示例

**简化命令（推荐）**：
```bash
# 搜索包含 .br 域名的URL
./MotaV1.0_linux_amd64 .tw

# 搜索包含 .com 域名的URL
./MotaV1.0_linux_amd64 .com

# 搜索包含 .edu 域名的URL
./MotaV1.0_linux_amd64 .edu
```

**传统命令**：
```bash
# 搜索包含 .br 域名的URL
./MotaV1.0_linux_amd64 -keyword=.tw

# 搜索包含 .com 域名的URL
./MotaV1.0_linux_amd64 -keyword=.com
```

**获取帮助**：
```bash
./MotaV1.0_linux_amd64 -h
```

## 输出文件

搜索结果会保存到 `MotaUrl.txt` 文件中，每行一个URL。

## 服务器信息

- 客户端会自动连接到服务器获取数据
- 无需本地安装任何数据文件

## 技术特点

- 使用Go语言开发，性能优异
- 支持正则表达式匹配域名和完整URL
- 实现了CORS支持和详细的日志记录
- 客户端本地保存认证信息，避免重复生成认证码

## 注意事项

1. 首次使用需要网络连接到服务器
2. 认证码具有唯一性，请妥善保管
3. 如需技术支持，请联系管理员

## 更新日志

### V1.0
- 初始版本发布
- 支持多平台编译
- 实现认证机制
- 添加彩色3D Logo
- 优化用户体验

---

**Author**: Mon2on  
**Version**: 1.0  
**License**: All Rights Reserved 