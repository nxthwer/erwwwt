local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("DarkX Hub (FE)", "GrapeTheme")

-- SCRIPTS 
local Tab = Window:NewTab("Scripts")
local Section = Tab:NewSection("Abuse Scripts")


Section:NewButton("Jetski", "Teleports you to a Jetski", function()
   loadstring(game:HttpGet("https://pastebin.com/raw/rKmydWTS"))()

end)

Section:NewButton("Infinite Yield", "Gives you Infinite Yield Admin", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
end)

Section:NewButton("Pastriez Bypasser GUI", "Opens the Pastriez Bypasser GUI", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/nxthwer/nxthwer/main/README.md"))()
end)

Section:NewButton("Trolling UI","Opens a Trolling UI", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/nxthwer/darkxhub2/main/README.md"))()
end)

local Player = Window:NewTab("Player")
local Section = Player:NewSection("Player Sliders")

Section:NewSlider("Walkspeed", "Changes your walkspeed", 500, 16, function(s) -- Maxium Speed = 500, Minimum Speed = 16
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

Section:NewSlider("Jump Power", "Changes your Jump Power", 500, 50, function(s) -- Maximum Jump = 500, Minimum Jump = 50
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)

