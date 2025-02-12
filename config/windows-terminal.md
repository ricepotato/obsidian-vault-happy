
windows terminal settings


settings.json

- ctrl + W 누르면 창 닫기
- ctrl + T 누르면 새 열기
- 반투명, 배경효과

```
{
    "$help": "https://aka.ms/terminal-documentation",
    "$schema": "https://aka.ms/terminal-profiles-schema",
    "actions": 
    [
        {
            "command": "find",
            "id": "User.find",
            "keys": "ctrl+shift+f"
        },
        {
            "command": 
            {
                "action": "newTab"
            },
            "id": "User.newTab.5DEADB41",
            "keys": "ctrl+t"
        },
        {
            "command": 
            {
                "action": "splitPane",
                "split": "auto",
                "splitMode": "duplicate"
            },
            "id": "User.splitPane.A6751878",
            "keys": "alt+shift+d"
        },
        {
            "command": "paste",
            "id": "User.paste",
            "keys": "ctrl+v"
        },
        {
            "command": 
            {
                "action": "copy",
                "singleLine": false
            },
            "id": "User.copy.644BA8F2",
            "keys": "ctrl+c"
        },
        {
            "command": 
            {
                "action": "closeTab"
            },
            "id": "User.closeTab.0",
            "keys": "ctrl+w"
        }
    ],
    "copyFormatting": "none",
    "copyOnSelect": false,
    "defaultProfile": "{4dd1e689-b517-5f39-947d-78e8a8bdf958}",
    "newTabMenu": 
    [
        {
            "type": "remainingProfiles"
        }
    ],
    "profiles": 
    {
        "defaults": 
        {
            "backgroundImageOpacity": 0.3,
            "opacity": 90,
            "useAcrylic": true
        },
        "list": 
        [
            {
                "commandline": "%SystemRoot%\\System32\\WindowsPowerShell\\v1.0\\powershell.exe",
                "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
                "hidden": false,
                "name": "Windows PowerShell"
            },
            {
                "commandline": "%SystemRoot%\\System32\\cmd.exe",
                "guid": "{0caa0dad-35be-5f56-a8ff-afceeeaa6101}",
                "hidden": false,
                "name": "\uba85\ub839 \ud504\ub86c\ud504\ud2b8"
            },
            {
                "guid": "{b453ae62-4e3d-5e58-b989-0a998ec441b8}",
                "hidden": false,
                "name": "Azure Cloud Shell",
                "source": "Windows.Terminal.Azure"
            },
            {
                "font": 
                {
                    "face": "MesloLGS NF"
                },
                "guid": "{2ece5bfe-50ed-5f3a-ab87-5cd4baafed2b}",
                "hidden": false,
                "name": "Git Bash",
                "source": "Git"
            },
            {
                "guid": "{07b52e3e-de2c-5db4-bd2d-ba144ed6c273}",
                "hidden": true,
                "name": "WSL2",
                "opacity": 95,
                "source": "Windows.Terminal.Wsl"
            },
            {
                "colorScheme": "One Half Dark",
                "experimental.retroTerminalEffect": false,
                "font": 
                {
                    "face": "MesloLGS NF",
                    "weight": "semi-bold"
                },
                "guid": "{4dd1e689-b517-5f39-947d-78e8a8bdf958}",
                "hidden": false,
                "name": "Ubuntu 20.04.6 LTS",
                "opacity": 95,
                "source": "CanonicalGroupLimited.Ubuntu20.04LTS_79rhkp1fndgsc",
                "useAcrylic": false
            }
        ]
    },
    "schemes": [],
    "themes": []
}
```
