# calcgrid

A command line for spreadsheets, made for AI agents (Claude Code and others) and scripts.
It reads, edits, checks and renders CalcGrid documents (`.numb`) and Excel files (`.xlsx`) —
Excel files are edited in place, and what calcgrid does not understand in them is left as it was.

Free. One binary, no network access, JSON on stdout.

## Install

```bash
brew install sunfmin/tap/calcgrid
```

Apple silicon, macOS 14 or later. Update with `brew upgrade calcgrid`.

## Start

```bash
calcgrid help            # every command
calcgrid help <command>  # one command and the shape of its output
calcgrid skill           # the guide for an AI agent
```

To teach Claude Code when to use it:

```bash
mkdir -p ~/.claude/skills/calcgrid && calcgrid skill > ~/.claude/skills/calcgrid/SKILL.md
```

## The CalcGrid app

CalcGrid is also a Mac spreadsheet app, sold separately on the Mac App Store (coming soon).
calcgrid works without it. Two commands need the app: `calcgrid open FILE` shows a file in
its window, and `calcgrid selection` answers what the user has selected there.

## 中文

`calcgrid` 是给 AI Agent 和脚本用的表格命令行：读、改、验算、渲染 CalcGrid 文档（`.numb`）和 Excel 文件
（`.xlsx`）。免费，单个二进制，不联网，输出是 JSON。用 `brew install sunfmin/tap/calcgrid` 安装（Apple 芯片，
macOS 14 起）。CalcGrid（算格）App 在 Mac App Store 另售（即将上架）；命令行不装 App 也能用，只有 `open` 和
`selection` 两条命令要 App。

## Feedback

Open an issue in this repository.

## License

Free to use; see [LICENSE](LICENSE). The source code is not published.
