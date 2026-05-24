
目前我在编写游戏代码这一块是使用的谷歌的antigravity来编写的代码，但是目前有一个游戏逻辑一直没有编写成功。我是使用的自然语言来告诉AI需要实现的效果，但是这样的结果并不理想。所以需要换一下具体的与AI的沟通方式。




UI构建

```mermaid
flowchart TD
    截图 --> 豆包分析
    豆包分析 --> Obsidian整理
    Obsidian整理 --> Antigravity执行
    Antigravity执行 --> Godot测试
    Godot测试 --> 新截图
```

目前游戏逻辑功能实现的流程是
```mermaid
flowchart TD
A[Antigravity生成代码] --> B[手动测试]
B --> C[问题提取]
C --> D[GPT分析问题]
D --> E[生成修复Prompt]
E --> F[Antigravity修复]
F --> B
```
antigravity自动实现代码->测试一遍，找出问题，提出需求->实现功能的关键代码+需求提交给gpt->gpt给出prompt->antigravity重新修改代码