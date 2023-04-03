if game.PlaceId == 11103424163 then
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Heist Tycoon💰 / https://discord.gg/6jVRkbARXf", HidePremium = false, IntroText = "Luxorry Hub", SaveConfig = true, ConfigFolder = "LuxFolder"})

--Values
_G.PayIncome = true


--Functions

function PayIncome()
    while _G.PayIncome == true do
    local args = {
        [1] = game:GetService("Players").LocalPlayer
    }
    
    game:GetService("ReplicatedStorage").Knit.Services.TycoonService.RF.PayIncome:InvokeServer(unpack(args))
    end
   end

local Tab = Window:MakeTab({
	Name = "Inf Cash",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddToggle({
	Name = "inf Cash",
	Default = false,
	Callback = function(Value)
        _G.PayIncome = Value
		PayIncome()
	end    
})



end
OrionLib:Init()
