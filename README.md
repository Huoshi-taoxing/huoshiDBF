# 目录爆破 DBF - 目录爆破工具 (Directory Brute Forcing Tool)

## 简介
目录爆破DBF 是一款基于 Python编写的专业目录爆破工具，旨在辅助授权范围内的渗透测试和网络安全研究。  
通过伪装多种操作系统和浏览器的用户代理及来源 IP，实现较为隐蔽的爆破访问，帮助用户发现网站隐藏目录和文件。

<img src="https://i.ibb.co/NdRyyYVH/DBF.png" alt="DBF工具截图" width="150"> <h3>目录爆破 DBF</h3>

## 主要功能
- **目录爆破**  
  根据用户自定义字典对目标 URL 进行目录或文件爆破，支持自定义爆破扩展名（如 php、html、asp 等），字典文件已经都准备好了，无需额外下载。
  
- **多线程爆破**  
  支持用户设定线程数，提升爆破速度，默认线程数为 10，线程数可调范围为 1 到 50。
  
- **请求伪装**  
  自动随机选择不同的 User-Agent、Referer，模拟不同设备和浏览器访问；  
  随机生成伪造 IP，模拟多来源访问，减少被屏蔽风险。
  
- **响应关键词筛选**  
  支持设置响应关键词，只显示包含指定关键词的结果，提高有效性。
  
- **自定义请求头**  
  支持用户输入自定义 HTTP 请求头，灵活调整请求细节。
  
- **请求结果日志**  
  实时显示请求结果日志，支持筛选只显示 HTTP 200 状态的成功目录。
  
- **已发现目录列表**  
  单独列表展示所有 HTTP 200 响应的目录或文件，方便查看和导出。
  
- **暗黑主题切换**  
  支持界面暗黑模式切换，保护视力，提升用户体验。
  
- **程序界面简洁友好**  
  采用 PyQt5 设计，界面布局合理，操作简单，适合渗透测试初学者和专业人员使用。

## 使用说明
1. 在“目标 URL”输入框填写目标网站地址（例如：http://example.com），请确保以 http:// 或 https:// 开头。  
2. 通过“浏览”按钮加载目录爆破字典文件（文本格式，每行一个目录或文件名）。  
3. 根据需要填写扩展名、响应关键词和自定义请求头（可选）。  
4. 设置线程数，推荐10个以下，防止过快爆破导致被封IP。  
5. 点击“启动”开始爆破，点击“终止”可随时停止。  
6. 通过“精准锁定 ⌖”选项，仅显示 HTTP 200 成功结果。  
7. 查看日志输出，已发现的目录可以通过“已发现的目录”按钮展开列表查看。  
8. 可通过“设置 -> 设置主题”切换暗黑模式。

## 注意事项
- 本工具仅限授权范围内使用，严禁用于非法攻击或未经许可的渗透测试。  
- 爆破频率和线程数过高可能导致目标服务器负载过重或封禁 IP。  
- 仅供网络安全学习、研究和授权测试使用。

## 开发者
- 火狮桃星 HUOSHI  / 影火 Shadow Flame
- B站：https://space.bilibili.com/3546720468207796?spm_id_from=333.337.search-card.all.click

---
## 关键词
目录爆破，huoshidbf，目录爆破DBF，火狮桃星，目录爆破工具，Directory Brute Forcing Tool，渗透测试，Web 安全，渗透测试工具，Python 爆破工具，多线程目录爆破，HTTP 目录扫描，隐蔽访问，网络安全研究，渗透测试字典

感谢使用火狮桃星 的 目录爆破 DBF 工具，祝您测试顺利！

---

English:

# Directory Brute Forcing Tool (DBF)

## Overview
DBF is a professional directory brute forcing tool written in Python for authorized penetration testing and cybersecurity research.  
It uses randomized User-Agent, Referer headers, and spoofed source IPs to perform stealthy brute forcing on target URLs, helping discover hidden directories and files.

## Features
- Directory brute forcing with customizable dictionaries and extensions (php, html, asp, etc.). Dictionaries included.
- Multi-threaded requests with adjustable thread count (default 10, range 1-50).
- Randomized User-Agent, Referer, and spoofed IPs to reduce detection.
- Response keyword filtering to show only relevant results.
- Support for custom HTTP headers.
- Real-time request logs with option to show only HTTP 200 OK responses.
- Separate list for discovered valid directories/files.
- Dark mode UI option.
- Simple, clean PyQt5 GUI for easy operation.

## Usage
1. Enter the target URL (must start with http:// or https://).  
2. Load a directory dictionary file (one directory or filename per line).  
3. Optionally set file extensions, response keywords, custom headers, and thread count.  
4. Click **Start** to begin brute forcing, **Stop** to halt.  
5. Use the “Only HTTP 200” filter to show successful hits.  
6. View discovered directories from the results panel.  
7. Switch UI theme between light and dark in settings.

## Important
- Only use this tool on systems where you have permission.  
- Excessive thread counts or request rates may cause server overload or IP blocking.  
- Intended for learning, research, and authorized security testing only.

## Author
- Huoshi Taoxing (火狮桃星) / Shadow Flame (影火)  
- Bilibili: https://space.bilibili.com/3546720468207796?spm_id_from=333.337.search-card.all.click

---

Thank you for using Huoshi Taoxing’s DBF tool! Wishing you successful tests.