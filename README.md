local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "wan", HidePremium = false,
    IntroText = "DG221", SaveConfig = true, ConfigFolder = "wan"})

OrionLib:MakeNotification({
 Name = "HI!",
 Content = "i'm gay",
 Image = "rbxassetid://4483345998",
 Time = 5
})

local dg1Tab = Window:MakeTab({
 Name = "Tab 1",
 Icon = "rbxassetid://4483345998",
 PremiumOnly = false
})

local Section = dg1Tab:AddSection({
 Name = "DG221 Section"
})

dg1Tab:AddButton({
 Name = "Button!",
 Callback = function()
        print("button pressed")
   end    
})

dg1Tab:AddToggle({
 Name = "This is a toggle!",
 Default = false,
 Callback = function(Value)
  print("Subscribe")
 end    
})

dg1Tab:AddColorpicker({
 Name = "Colorpicker",
 Default = Color3.fromRGB(255, 0, 0),
 Callback = function(Value)
  print(Value)
 end   
})

dg1Tab:AddSlider({
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

dg1Tab:AddDropdown({
 Name = "Dropdown",
 Default = "1",
 Options = {"1", "2"},
 Callback = function(Value)
  print(Value)
 end    
})

---Tap2---

local dg2Tab = Window:MakeTab({
 Name = "Tab 1",
 Icon = "rbxassetid://4483345998",
 PremiumOnly = false
})

local Section = dg2Tab:AddSection({
 Name = "DG221 Section"
})

dg2Tab:AddButton({
 Name = "Button!",
 Callback = function()
        print("button pressed")
   end    
})

dg2Tab:AddToggle({
 Name = "This is a toggle!",
 Default = false,
 Callback = function(Value)
  print("Subscribe")
 end    
})

dg2Tab:AddColorpicker({
 Name = "Colorpicker",
 Default = Color3.fromRGB(255, 0, 0),
 Callback = function(Value)
  print(Value)
 end   
})

dg2Tab:AddSlider({
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

dg2Tab:AddDropdown({
 Name = "Dropdown",
 Default = "1",
 Options = {"1", "2"},
 Callback = function(Value)
  print(Value)
 end    
})

OrionLib:Init()
