# @zereight/mcp-gitlab

GitLab MCP(Model Context Protocol) Server.

## Installation and Execution

```bash
npx @zereight/mcp-gitlab
```

## Environment Variable Configuration

Before running the server, you need to set the following environment variables:

```bash
GITLAB_PERSONAL_ACCESS_TOKEN=your_gitlab_token
GITLAB_API_URL=your_gitlab_api_url  # Default: https://gitlab.com/api/v4
```

## License

MIT License

## How to use

## Using with Claude App

When using with the Claude App, you need to set up your API key and URLs directly.

```json
{
  "mcpServers": {
    "GitLab communication server": {
      "command": "npx @zereight/mcp-gitlab",
      "args": [],
      "env": {
        "GITLAB_PERSONAL_ACCESS_TOKEN": "your_gitlab_token",
        "GITLAB_API_URL": "your_gitlab_api_url"
      }
    }
  }
}
```

## Using with Cursor

When using with Cursor, you can set up environment variables and run the server as follows:

```bash
env GITLAB_PERSONAL_ACCESS_TOKEN=your_gitlab_token GITLAB_API_URL=your_gitlab_api_url npx @zereight/mcp-gitlab
```

- `GITLAB_PERSONAL_ACCESS_TOKEN`: Your GitLab personal access token.
- `GITLAB_API_URL`: Your GitLab API URL. (Default: `https://gitlab.com/api/v4`)
