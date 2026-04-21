# Shadowrocket Configuration (sr-rules)

This is my personal Shadowrocket configuration project, primarily used for traffic splitting and rule optimization.

## File Descriptions

| Filename | Description |
| :--- | :--- |
| **`wxy-sr-rules.conf`** | **Final configuration currently in use**. Contains customized splitting rules and policy groups. |
| `Nexitally.conf` | Original configuration file provided by the network service provider, used as a basic reference. |
| `a-nomad.conf` | Reference configuration file copied from [YouTubeResources](https://github.com/wxy8866/YouTubeResources). |

## Key Features

- **Policy Group Design**:
  - `AI专用节点` (AI Dedicated Nodes): Optimized node selection specifically for AI services like Claude (anthropic.com, claude.ai) and OpenAI.
  - `♻️ 自动选择` (Automatic Selection): Automatically switches to the best node based on latency.
  - `📹 油管视频` / `🎥 奈飞视频` / `📺 巴哈姆特`: Independent policy controls for streaming services (YouTube, Netflix, Bahamut).
- **Regional Grouping**: Includes automatic speed-test groups for common regions such as Hong Kong, Japan, Singapore, and the USA.
- **Auto-Update**: The configuration is hosted on GitHub and supports direct remote updates within Shadowrocket.

## Rule Sources
This configuration references and integrates the following rule sets:
- [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR)
- [Loyalsoldier/surge-rules](https://github.com/Loyalsoldier/surge-rules)
- Custom rules (e.g., Claude enhancement rules, local application process filtering, etc.)

## How to Use
1. Download or copy the URL of `wxy-sr-rules.conf`.
2. In Shadowrocket, import it via "Remote Files" -> "Add Remote File".

---
*Note: This project is for personal study and use only.*
