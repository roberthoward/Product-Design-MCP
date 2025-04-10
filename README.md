    "chat.agent.enabled": true,
    "mcp": {

        "inputs": [],
        "servers": {
            "github": {
                "command": "npx",
                "args": [
                    "-y",
                    "@modelcontextprotocol/server-github"
                ],
                "env": {"GITHUB_PERSONAL_ACCESS_TOKEN": "--- PAT "}
            },
            "figma": {
                "command": "npx",
                "args": [
                    "-y",
                    "figma-developer-mcp",
                    "--stdio"
                ],
                "env": {"FIGMA_API_KEY": ""}
            },  
             "azureDevOps": {
                "command": "npx",
                "args": ["-y", "@tiberriver256/mcp-server-azure-devops"],
                "env": {
                    "AZURE_DEVOPS_ORG_URL": "https://dev.azure.com/tr-design",
                    "AZURE_DEVOPS_AUTH_METHOD": "pat",
                    "AZURE_DEVOPS_PAT": "——PERSONAL ACCESS TOKEN —-",
                    "AZURE_DEVOPS_DEFAULT_PROJECT": "Design%20Organization"
                }
            },
        
        },
        
    },
    "files.autoSave": "afterDelay",
    "chat.editing.confirmEditRequestRetry": false
}
