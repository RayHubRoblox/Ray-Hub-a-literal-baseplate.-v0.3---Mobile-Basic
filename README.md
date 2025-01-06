--[[
--WARNING: This script is an official script from Ray Scripts TEAM, and there's no danger at all! (See which are the real Ray Hub and download them safely on the Youtube channel @RayScriptsTEAM)
]]
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()
local SaveManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/SaveManager.lua"))()
local InterfaceManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/InterfaceManager.lua"))()

local Window = Fluent:CreateWindow({
    Title = "Ray Hub | a literal baseplate.",
    SubTitle = "v0.3 - Mobile Basic",
    TabWidth = 160,
    Size = UDim2.fromOffset(460, 250),
    Acrylic = true, 
    Theme = "Dark",
    MinimizeKey = Enum.KeyCode.LeftControl 
})

local Tabs = {
    Main = Window:AddTab({ Title = "Main (FE Scripts)", Icon = "contact" })
}

local Options = Fluent.Options

do
    Fluent:Notify({
        Title = "Loaded",
        Content = "Ray Hub",
        SubContent = "Ray Hub loaded",
        Duration = 5
    })



    Tabs.Main:AddParagraph({
        Title = "Reset when changing to others script",
        Content = ""
    })



    Tabs.Main:AddButton({
        Title = "Da feed",
        Description = "Da feed make ur arm and leg as long leg",
        Callback = function()
             loadstring(game:HttpGet('https://gist.githubusercontent.com/1BlueCat/7291747e9f093555573e027621f08d6e/raw/23b48f2463942befe19d81aa8a06e3222996242c/FE%2520Da%2520Feets'))()
        end
    })
    
    
    Tabs.Main:AddButton({
        Title = "Walk of Element",
        Description = "Walk animation",
        Callback = function()
                      loadstring(game:HttpGet('https://rawscripts.net/raw/Universal-Script-FE-Nameless-Animations-V4-4249'))()
        end
    })
    Tabs.Main:AddButton({
        Title = "Clovr",
        Description = "Turn ur body into vr can be without vr",
        Callback = function()
                            loadstring(game:HttpGet('https://rawscripts.net/raw/Just-a-baseplate.-Fe-Clovr-14102'))()
        end
    })
    
    Tabs.Main:AddButton({
        Title = "Fe winged master",
        Description = "Arm as a wing?",
        Callback = function()
                            loadstring(game:HttpGet('https://pastebin.com/raw/G68Krc4Q'))()
        end
    })
    
    
    

end
    
Window:SelectTab(1)
   
