# Criminality UI
This documentation is for Kavo UI Credit To The Owner

## Booting the Criminality UI Library
```lua
local library = loadstring(game:HttpGet('https://raw.githubusercontent.com/cueshut/saves/main/criminality%20paste%20ui%20library'))()
```




## Creating a Criminality UI Window
```lua
local window = library.new('...', 'aye')
```

## Creating a Tab
```lua
local tab = window.new_tab('rbxassetid://4483345998')
local tab1 = window.new_tab('rbxassetid://4483345998')
```

## Creating a Section
```lua
local section = tab.new_section('Bruh XD')
local section1 = tab.new_section(':DDD HI')
```

## Creating a Sector
```lua
local sector = section.new_sector('OK', 'Left')
local sector1 = section.new_sector('BRUHHHH', 'Right')
```

## Creating a Button
```lua
local button = sector.element('Button', 'Button', nil, function()

end)
```

## Creating a toggle
```lua
local toggle = sector.element('Toggle', 'Toggle', false, function(v)
   print(v.Toggle)
end)
```

## Creating a Add Color
```lua
toggle:add_color({Color = Color3.fromRGB(84, 101, 255)}, nil, function(v)
   print(v.Color)    
end)
```

## Creating a Textbox
```lua
Section:NewTextBox("TextboxText", "TextboxInfo", function(txt)
	print(txt)
end)
```

## Creating a Dropdown
```lua
local dropdown = sector.element('Dropdown', 'Dropdown', {options = {'one', 'two', 'three'}}, function(v)
   print(v.Dropdown)
end)
```

## Creating a Slider
```lua
local slider = sector.element('Slider', 'Slider', {default = {min = 1, max = 100, default = 50}}, function(v)
   print(v.Slider)
end)
```

## Creating Combo
```lua
local combo = sector.element('Combo', 'Combo', {options = {'bruh', 'otherbruh'}}, function(v)
   table.foreach(v.Combo, print)
end)
```
