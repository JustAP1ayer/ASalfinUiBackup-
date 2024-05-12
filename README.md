# ASalfinUiBackup-

Slider and Slider2 is different as Slider works after you finish sliding but Slider2 is a calling script, which it would always update when sliding

## Themes
```lua

    --[[
        light theme
    
            MainColor = Color3.fromRGB(200,200,235);
            BrighterMainColor = Color3.fromRGB(215,215,245);
            IconsColor = Color3.fromRGB(100,100,120);
            Accent = Color3.fromRGB(0,100,255);
            DarkText = Color3.fromRGB(75,75,75);
            BrightText = Color3.fromRGB(50,50,50);
            Font = "Gotham";
            SoundVolume = 0.5;
    
    
        dark theme
    
            MainColor = Color3.fromRGB(35,35,40);
            BrighterMainColor = Color3.fromRGB(40,40,45);
            IconsColor = Color3.fromRGB(100,100,120);
            Accent = Color3.fromRGB(0,100,255);
            DarkText = Color3.fromRGB(170,170,170);
            BrightText = Color3.fromRGB(145,145,145);
            Font = "Gotham";
            SoundVolume = 0.5;
    
        
        dark green theme
    
            MainColor = Color3.fromRGB(30,35,30);
            BrighterMainColor = Color3.fromRGB(35,40,35);
            IconsColor = Color3.fromRGB(100,100,120);
            Accent = Color3.fromRGB(0,255,100);
            DarkText = Color3.fromRGB(170,170,170);
            BrightText = Color3.fromRGB(145,145,145);
            Font = "Gotham";
            SoundVolume = 0.5;
    
    
        dark red theme
    
            MainColor = Color3.fromRGB(35,30,30);
            BrighterMainColor = Color3.fromRGB(40,35,35);
            IconsColor = Color3.fromRGB(100,100,120);
            Accent = Color3.fromRGB(255,0,100);
            DarkText = Color3.fromRGB(170,170,170);
            BrightText = Color3.fromRGB(145,145,145);
            Font = "Gotham";
            SoundVolume = 0.5;

Random Color Theme

local rainbowFrequency = 0.75 
local tick = tick()


getgenv().LibTheme = {
    MainColor = Color3.fromRGB(35, 35, 40);
    BrighterMainColor = Color3.fromRGB(40, 40, 45);
    IconsColor = Color3.fromRGB(100, 100, 120);
    Accent = Color3.new(
        math.sin(tick * rainbowFrequency) * 0.5 + 0.5,
        math.sin(tick * rainbowFrequency + 2 * math.pi / 3) * 0.5 + 0.5,
        math.sin(tick * rainbowFrequency + 4 * math.pi / 3) * 0.5 + 0.5
    );
    DarkText = Color3.fromRGB(170, 170, 170);
    BrightText = Color3.fromRGB(145, 145, 145);
    Font = "Gotham";
    SoundVolume = 0.5;
    HideKey = "LeftAlt";
}



    ]]
```
  ## Document
  
 ```lua  

local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/JustAP1ayer/ASalfinUiBackup-/main/ocerlibbackupnopopup.lua"))()

local Main = Library.Main("Ocerlib")
Main.Loader() -- loads,1 arg for how long it is
local Page = Main.Page("Page","3926305904",Vector2.new(924, 204),Vector2.new(36, 36))

local Section = Page.Section("Section")

local Toggle = Section.Component("Toggle","Toggle Name",function(bool)
  -- Code
end,false)

local Dropdown = Section.Component("Dropdown","Dropdown Name",{"choice1","choice2","choice3"},false,function(string,bool)
-- Code
end,false)

local Slider = Section.Component("Slider","Slider Name",0,100,false,function(value)
-- Code
end,50)

local Slider2 = Section.Component("Slider2","Slider Name",0,100,false,function(value)
-- Code
end,50)
Section.Component("TextBox","Title","Text In Box",false,function(value) -- boolean is textdisappear
print(value)
end)
local Button = Section.Component("Button","Button Name",function()
-- Code
end)

local Paragraph = Section.Component("Card", "Title", "Text here")

local Logs = Main.Logs("Logs name")

local log1 = Logs.LogWithButtons("smh")

local logbutton = log1.Button("something",function()
-- Code
end)
```
  ## Example

 ```lua  
getgenv().LibTheme = {
MainColor = Color3.fromRGB(35,30,30);
            BrighterMainColor = Color3.fromRGB(40,35,35);
            IconsColor = Color3.fromRGB(100,100,120);
            Accent = Color3.fromRGB(255,0,100);
            DarkText = Color3.fromRGB(170,170,170);
            BrightText = Color3.fromRGB(145,145,145);
   Font = "FredokaOne";
   SoundVolume = 1;
   HideKey = "LeftAlt"
}
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/JustAP1ayer/ASalfinUiBackup-/main/Ocerlibtest.lua"))()

local Main = Library.Main("Test")
Main.Loader(3) -- seconds
local Page = Main.Page("Page","3926305904",Vector2.new(924, 204),Vector2.new(36, 36))

local Section = Page.Section("Sextion")
local Logs = Main.Logs("Logs name")
 Section.Component("Toggle","Enable / Disable 3d rendering",function(bool)
game:GetService("RunService"):Set3dRenderingEnabled(bool)
end,true)

Section.Component("Dropdown","Dropdown Name",{"choice1","choice2","choice3"},false,function(string,bool)
print(string)
end,false)

 Section.Component("Slider","Walkspeed",0,100,false,function(value)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end,16)

 Section.Component("Slider2","Walkspeed",0,100,false,function(value)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end,16)

Section.Component("Button","Log logs that print yes",function()

Logs.LogWithButtons("smh").Button("something",function()
print("yes")
end)

end)
Section.Component("TextBox","Title","Text In Box",false,function(value)
print(value)
end)
Section.Component("Card", "Hi guys this is a", "Test")

local log1 = Logs.LogWithButtons("nut")

log1.Button("print it lol",function()
print("Came")
end)
Logs.LogWithButtons("no")
```


