# GameKillerHub
local Mercury = loadstring(game:HttpGet("https://raw.githubusercontent.com/deeeity/mercury-lib/master/src.lua"))()

local GUI = Mercury:Create{
    Name = "Game killer",
    Size = UDim2.fromOffset(600, 400),
    Theme = Mercury.Themes.Dark,
    Link = "https://github.com/deeeity/mercury-lib"
}

local Tab = GUI:Tab{
	Name = "Main",
	Icon = "rbxassetid://8569322835"
}

Tab:Button{
	Name = "Acrylix",
	Description = nil,
	Callback = function()
loadstring(game:HttpGet('https://github.com/3dsonsuce/acrylix/raw/main/Acrylix'))()
 end
}

Tab:Button{
	Name = "Unstability",
	Description = nil,
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/ILOVETHECOFFINOFANDYANDLEYLEY/THE-HACK-/main/script%20omg"))()
 end
}

Tab:Button{
	Name = "No prompt cooldown",
	Description = nil,
	Callback = function()
getgenv().G = true -- change its to false and execute again to disable

while getgenv().G do -- repeats script till getgenv().G = true

for i,d in pairs(game.Workspace:GetDescendants()) do -- iterates throught every object in game workspace.
    if d.ClassName == 'ProximityPrompt' then -- checks if current object is "ProximityPrompt"
        d.HoldDuration = 0 -- changes hold duration to zero. 
    end
end
wait(10) 
end
 end
}

Tab:Button{
	Name = "Infinite Yield",
	Description = nil,
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
 end
}

Tab:Button{
	Name = "Nameless Admin",
	Description = nil,
	Callback = function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/FilteringEnabled/NamelessAdmin/main/Source'))()
 end
}
