# WindUI Mod

> **WindUI Mod** is a refined fork of the original **WindUI** UI library for Roblox, designed specifically for _Script Hubs_ and _Luau environments_.

This fork maintains full compatibility with the original API and structure while introducing various improvements, bug fixes, optimizations, and visual enhancements.

[![WindUI Mod](https://uibin.orqan.xyz/api/card?id=374c5531-a842-426c-bc90-905eafa936c5&theme=orange)](https://uibin.orqan.xyz/library/374c5531-a842-426c-bc90-905eafa936c5)

---

## Features

* Full compatibility with the original WindUI API and structure
* Bug fixes and improved stability
* Additional elements for Script Hubs and Luau environments

---

## Getting Started

### Installation

Load WindUI Mod into your script using the `loadstring` below:

```luau
local WindUI = loadstring(game:HttpGet("https://raw.githubusercontent.com/orialdev/windui-boreal/refs/heads/main/WindUI-Mod.lua"))()
````

Create a WindUI Mod for your script; you can remove the "--" comments to use the functionality. 

```luau
local Window = WindUI:CreateWindow({
    Title = "My Super Hub",
    Icon = "door-open", -- lucide icon
    Author = "by .ftgs and .ftgs",
    Folder = "MySuperHub",
    
    -- ↓ This all is Optional. You can remove it.
    Size = UDim2.fromOffset(580, 460),
    MinSize = Vector2.new(560, 350),
    MaxSize = Vector2.new(850, 560),
    ToggleKey = Enum.KeyCode.LeftShift,
    Transparent = true,
    Theme = "Dark",
    Resizable = true,
    SideBarWidth = 200,
    BackgroundImageTransparency = 0.42,
    HideSearchBar = true,
    ScrollBarEnabled = false,
    
    -- ↓ Optional. You can remove it.
    --[[ You can set 'rbxassetid://' or video to Background.
        'rbxassetid://':
            Background = "rbxassetid://", -- rbxassetid
        Video:
            Background = "video:YOUR-RAW-LINK-TO-VIDEO.webm", -- video 
    --]]
    
    -- ↓ Optional. You can remove it.
    User = {
        Enabled = true,
        Anonymous = true,
        Callback = function()
            print("clicked")
        end,
    },
    
    --       remove this all, 
    -- !  ↓  if you DON'T need the key system
    KeySystem = { 
        -- ↓ Optional. You can remove it.
        Key = { "1234", "5678" },
        
        Note = "Example Key System.",
        
        -- ↓ Optional. You can remove it.
        Thumbnail = {
            Image = "rbxassetid://",
            Title = "Thumbnail",
        },
        
        -- ↓ Optional. You can remove it.
        URL = "YOUR LINK TO GET KEY (Discord, Linkvertise, Pastebin, etc.)",
        
        -- ↓ Optional. You can remove it.
        SaveKey = false, -- automatically save and load the key.
        
        -- ↓ Optional. You can remove it.
        -- API = {} ← Services. Read about it below ↓
    },
})
```

---

## Credits

| Role | Contributor | Link |
|------|:------------|:-----|
| **Original Author** | Footagesus | [WindUI Repository](https://github.com/Footagesus/WindUI) |
| **Fork Owner** | orialdev | [GitHub Profile](https://github.com/orialdev) |

> This project would not exist without the original work provided by **Footagesus**.
>
>> Full credit for the core framework, architecture, and underlying systems belongs to the original author.

---

## Community

Need help, want updates, or looking for announcements?

👉 **[Join our Discord server](https://discord.gg/B3dEqP2EX6)**
