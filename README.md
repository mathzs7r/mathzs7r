<img
    align="left"
    alt="HTML"
    title="HTML"
    width="30px"
    style="padding-right: 10px;"
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg"
/>
<img
    align="left"
    alt="CSS"
    title="CSS"
    width="30px"
    style="padding-right: 10px;"
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg"
/>
<img
    align="left"
    alt="JavaScript"
    title="JavaScript"
    width="30px"
    style="padding-right: 10px;"
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg"
/>
<img
    align="left"
    alt="Python"
    title="Python"
    width="30px"
    style="padding-right: 10px;"
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg"
/>
{
    "name": "GitHub Readme Stats Dev",
    "image": "mcr.microsoft.com/devcontainers/base:ubuntu",
    "features": {
        "ghcr.io/devcontainers/features/node:1": { "version": "22" }
    },
    "forwardPorts": [3000],
    "portsAttributes": {
        "3000": { "label": "HTTP" }
    },
    "appPort": [],

    // Use 'postCreateCommand' to run commands after the container is created.
    "postCreateCommand": "npm install -g vercel",

    // Use 'postStartCommand' to run commands after the container is started.
    "postStartCommand": "hostname dev && npm install",

    // Configure tool-specific properties.
    "customizations": {
        "vscode": {
            "extensions": [
                "yzhang.markdown-all-in-one",
                "esbenp.prettier-vscode",
                "dbaeumer.vscode-eslint",
                "github.vscode-github-actions"
            ]
        }
    },

    "remoteUser": "root",
    "privileged": true
}
