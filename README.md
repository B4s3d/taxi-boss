local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Taxi Boss RUSH", "BloodTheme")
local Tab = Window:NewTab("Main")
local Section = Tab:NewSection("Halloween")
Section:NewToggle("Candy Farm", ".", function(state)
    if state then
        _G.Autofarm = true
loadstring(game:HttpGet("https://raw.githubusercontent.com/Marco8642/science/main/halloween%20taxi", true))()
    else
        _G.Autofarm = false
loadstring(game:HttpGet("https://raw.githubusercontent.com/Marco8642/science/main/halloween%20taxi", true))()
    end
end)
Section:NewToggle("Auto Spin Halloween Wheel", ".", function(state)
    if state then
        _G.autospin = true
while _G.autospin do
game:GetService("ReplicatedStorage").SpinWheel:InvokeServer()
wait(1)
end
    else
        _G.autospin = false
while _G.autospin do
game:GetService("ReplicatedStorage").SpinWheel:InvokeServer()
wait(1)
end
    end
end)
