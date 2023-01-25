# ASalfinUiBackup-
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
            SoundVolume = 0.5
    
    
        dark theme
    
            MainColor = Color3.fromRGB(35,35,40);
            BrighterMainColor = Color3.fromRGB(40,40,45);
            IconsColor = Color3.fromRGB(100,100,120);
            Accent = Color3.fromRGB(0,100,255);
            DarkText = Color3.fromRGB(170,170,170);
            BrightText = Color3.fromRGB(145,145,145);
            Font = "Gotham";
            SoundVolume = 0.5
    
        
        dark green theme
    
            MainColor = Color3.fromRGB(30,35,30);
            BrighterMainColor = Color3.fromRGB(35,40,35);
            IconsColor = Color3.fromRGB(100,100,120);
            Accent = Color3.fromRGB(0,255,100);
            DarkText = Color3.fromRGB(170,170,170);
            BrightText = Color3.fromRGB(145,145,145);
            Font = "Gotham";
            SoundVolume = 0.5
    
    
        dark red theme
    
            MainColor = Color3.fromRGB(35,30,30);
            BrighterMainColor = Color3.fromRGB(40,35,35);
            IconsColor = Color3.fromRGB(100,100,120);
            Accent = Color3.fromRGB(255,0,100);
            DarkText = Color3.fromRGB(170,170,170);
            BrightText = Color3.fromRGB(145,145,145);
            Font = "Gotham";
            SoundVolume = 0.5
    ]]
    
    
getgenv().LibTheme = {
    MainColor = Color3.fromRGB(35,35,40);
    BrighterMainColor = Color3.fromRGB(40,40,45);
    IconsColor = Color3.fromRGB(100,100,120);
    Accent = Color3.fromRGB(0,100,255);
    DarkText = Color3.fromRGB(170,170,170);
    BrightText = Color3.fromRGB(145,145,145);
    Font = "Gotham";
    SoundVolume = 0.5;
    HideKey = "LeftAlt"
}

local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/JustAP1ayer/ASalfinUiBackup-/main/SalfinUILIBBACKUP.lua"))()

local Main = Library.Main("Ocerium")

local Page = Main.Page("Page","3926305904",Vector2.new(924, 204),Vector2.new(36, 36))

local Section = Page.Section("Section")

local Toggle = Section.Component("Toggle","Toggle Name",function(bool)
  
end,false)

local Dropdown = Section.Component("Dropdown","Dropdown Name",table,false,function(string,bool)

end,false)

local Slider = Section.Component("Slider","Slider Name",0,100,false,function(value)

end,50)

local Button = Section.Component("Button","Button Name",function()

end)

local Paragraph = Section.Component("Card", "Title", "Text here")

local Logs = Main.Logs("Logs name")

local log1 = Logs.LogWithButtons("smh")

local logbutton = log1.Button("something",function()

end)
