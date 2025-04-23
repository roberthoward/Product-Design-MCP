    "chat.agent.enabled": true,
    "mcp": {
        "inputs": [],
        "servers": {
            "figma": {
                "command": "npx",
                "args": [
                    "-y",
                    "figma-developer-mcp",
                    "--stdio"
                ],
                "env": {"FIGMA_API_KEY": ""}
            },  
        },
        
    },
    "files.autoSave": "afterDelay",
    "chat.editing.confirmEditRequestRetry": false
}
