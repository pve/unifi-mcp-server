# Unifi MCP Server

An MCP server for interacting with your unifi sites.
The API key can be created in the Unifi GUI under Control Plane -> Integrations.

## Usage

Example VSCode MCP Config

```json
"unifi-mcp-server": {
    "command": "uv",
    "args": [
        "--directory",
        "/absolute/path/to/unifi-mcp-server",
        "run",
        "main.py"
    ],
    "env": {
        "UNIFI_HOST": "<your-unifi-host>",
        "UNIFI_API_KEY": "<your-unifi-api-key>"
    }
}
```

## Development

1. Install [uv](https://github.com/astral-sh/uv)
1. `uv venv`
1. `source .venv/bin/activate`
1. `uv sync`
