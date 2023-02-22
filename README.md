local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "wan", HidePremium = false,
    IntroText = "DG221", SaveConfig = true, ConfigFolder = "wan"})

OrionLib:MakeNotification({
 Name = "HI!",
 Content = "i'm gay",
 Image = "rbxassetid://4483345998",
 Time = 5
})

local TutTab = Window:MakeTab({
 Name = "Tab 1",
 Icon = "rbxassetid://4483345998",
 PremiumOnly = false
})

local Section = TutTab:AddSection({
 Name = "DG221 Section"
})

TutTab:AddButton({
 Name = "Button!",
 Callback = function()
        print("button pressed")
   end    
})

TutTab:AddToggle({
 Name = "This is a toggle!",
 Default = false,
 Callback = function(Value)
  print("Subscribe")
 end    
})

TutTab:AddColorpicker({
 Name = "Colorpicker",
 Default = Color3.fromRGB(255, 0, 0),
 Callback = function(Value)
  print(Value)
 end   
})

TutTab:AddSlider({
 Name = "Slider",
 Min = 0,
 Max = 20,
 Default = 5,
 Color = Color3.fromRGB(255,255,255),
 Increment = 1,
 ValueName = "bananas",
 Callback = function(Value)
  print(Value)
 end    
})

Tab:AddDropdown({
 Name = "Dropdown",
 Default = "1",
 Options = {"1", "2"},
 Callback = function(Value)
  print(Value)
 end    
})

OrionLib:Init()
