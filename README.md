# mcp-snippetbox

MCP server template I base new tools on

Built for my own use; public in case it helps someone.

## Usage

```bash
# claude_desktop_config.json
# {
#   "mcpServers": {
#     "notes-box": {"command": "python", "args": ["server.py"]}
#   }
# }
python server.py
```

## Features

- State persisted to a JSON file in the home dir
- Three tools: add / get / list notes
- FastMCP style: decorators, zero boilerplate
- Includes Claude Desktop config snippet

## Getting started

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── Makefile
├── SECURITY.md
├── requirements.txt
└── server.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Changelog

- `0.1.1` - fix edge case in argument parsing
- `0.1.0` - first working version
