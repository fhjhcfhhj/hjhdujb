local WindUI = loadstring(game:HttpGet("https://github.com/Footagesus/WindUI/releases/latest/download/main.lua"))()
 
local Window = WindUI:CreateWindow({
    Title = "款脚本",
    Icon = "sparkle",
    Author = "小款制作必是精品",
    Folder = "GlovSakenScript",
    Size = UDim2.fromOffset(350, 300),
    Transparent = false,
    Theme = "Dark",
    Resizable = false,
    SideBarWidth = 150,
    HideSearchBar = true,
    ScrollBarEnabled = false,
})
 
Window:SetToggleKey(Enum.KeyCode.K)
 
WindUI:SetFont("rbxasset://fonts/families/AccanthisADFStd.json")
 
Window:EditOpenButton({
    Title = "款脚本",
    Icon = "sparkle",
    CornerRadius = UDim.new(0,16),
    StrokeThickness = 0,
    Color = ColorSequence.new(
        Color3.fromHex("000000"), 
        Color3.fromHex("000000")
    ),
    OnlyMobile = true,
    Enabled = true,
    Draggable = true,
})
 
local SentinelTab = Window:Tab({
    Title = "服务器",
    Icon = "shield",
})

local GuestSection = SentinelTab:Section({
    Title = "被遗弃",
    Opened = true,
})  

GuestSection:Button({
    Title = "殺脚本",
    Desc = "被遗弃",
    Callback = function() --被遗弃
loadstring(game:HttpGet("https://raw.githubusercontent.com/FengYu-X/Max/refs/heads/X/fsk.lua"))() end
})
