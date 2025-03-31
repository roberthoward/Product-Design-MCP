
{
    "mcp": {

        "inputs": [{
            "id": "gh-pat",
            "type": "promptString",
            "password": true,
            "description":"Enter your GitHub Personal Access Token"
        },
        {
            "id": "figma-key",
            "type": "promptString",
            "password": true,
            "description": "Enter your Figma API Key"
        }],
        "servers": {
            "github": {
                "command": "npx",
                "args": [
                    "-y",
                    "@modelcontextprotocol/server-github"
                ],
                "env": {
                    "GITHUB_PERSONAL_ACCESS_TOKEN": "--- PAT "
                }
            },
                "azureDevOps": {
                  "command": "npx",
                  "args": ["-y", "@tiberriver256/mcp-server-azure-devops"],
                  "env": {
                    "AZURE_DEVOPS_ORG_URL": "https://dev.azure.com/tr-design",
                    "AZURE_DEVOPS_AUTH_METHOD": "pat",
                    "AZURE_DEVOPS_PAT": “——PERSONAL ACCESS TOKEN —-,
                    "AZURE_DEVOPS_DEFAULT_PROJECT": "Design%20Organization"
                  }
                },
            "figma": {
                "command": "npx",
                "args": [
                    "-y",
                    "figma-developer-mcp",
                    "--stdio"
                ],
                "env": {
                    "FIGMA_API_KEY": "figd_KEY”
                }
            },
        }
    },
    "files.autoSave": "afterDelay",
    "chat.editing.confirmEditRequestRetry": false
}
