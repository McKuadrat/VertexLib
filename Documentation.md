# VertexUI Library
This guide for using VirtexUI Library!

# Booting The Gui
```lua
local VirtexLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/McKuadrat/VertexLib/refs/heads/main/Source')))()
```

# Creating Window
```lua
local Window = VirtexLib.MakeWindow({Name = "VirtexLib"})

--[[
Name = <String> -- Name Of GUI.
]]
```

# Making Tab
```lua
local Tab = Window.AddTab({Name = "Tab"})

--[[
Name = <String> -- Name Of Tab.
]]
```

# Making Sections
```lua
Tab.AddSection({
	Name = "Local Player"
})

--[[
Name : <String> -- Name Of The Sections
]]
```

# Making Button
```lua
Tab.AddButton({
	Name = "Button",
	OnClick = function()
		print("Hello")
	end
})

--[[
Name = <Sttring> -- Name Of The Button.
OnClick = <Functtion> -- Function for the button.
]]
```

# Making KeyBinds
```lua
Window.Keybinds({
	Key = "E",
	OnClick = function()
		print("Hello")
	end,
})

--[[
Key = <String> -- Key For The Keybinds.
Onclick = <Function> -- Funtion For The Keybinds.
]]
```

# Making DropDown
```lua
local DropDown = Tab.AddDropDown({
	Name = "DropDown",
	Options = {"1", "2},
	Default = "1",
	OnChange = function(Value)
		print(Value)
	end
})

--[[
Name : <String> -- Name Of The DropDown.
Options : <Table> -- The options in the DropDown.
Default : <String> -- The Default Value In DropDown.
OnChange : <Function> -- The Function Of DropDown.
]]
```

## Getting DropDown Value
```lua
DropDown.GetValue()
```

# Making Minimize Key Shortcut
```lua
Window.ShortCut(Enum.KeyCode.V)
```

## Playsound
```lua
Window.Playsound({
	Name = "Playsound1",
	ID = "1848354536"
})

--[[
Name = <String> -- Name Of The Playsound
ID = <String> -- Music ID To Play
]]
```

## Stopsound
```
Window.StopSound("Playsound1")
```

# Making TextBox
```lua
local Textbox = Tab.AddTextbox({
	Name = "Number",
	Text = "0",
	PlaceHolder = "0",
	ClearText = false
})

--[[
Name = <String> -- Name Of The TextBox.
Text = <String> -- Text For TextBox.
PlaceHolder = <String> -- PlaceHolder Text For Textbox.
ClearText = <String> -- Makes the text disappear in the textbox after losing focus.
]]
```

## Getting Textbox Value
```lua
Textbox.GetValue()
```

# Making Toggle
```lua
Tab.AddToggle({
	Name = "Toggle",
	OnClick = function()
		print("Helloo")
	end,
})

--[[
Name = <String> -- Name Of The Toggle.
OnClick = <Function> -- The Function Of The TextBox.
]]
```

# Making Slider
```lua
local Slider = Tab.AddSlider({
	Name = "Tes",
	Min = 1,
	Max = 10,
	Script = function(Value)
		print(Value)
	end
})

--[[
Name : <String> -- Name Of Slider
Min : <Number> -- Minimum Of Slider Value
Max : <Number> -- Maximum Of Sider Value
Script : <Function> -- Function When Slider Changing Value
]]
```

## Getting Slider Value
```lua
Slider.GetValue()
```

## Getting User Image
```lua
VirtexLib.GetUserImage()
```

# Making Paragraph
```lua
Tab.AddParagraph({
	Name = "Paragraph",
	Text = "Hi, this is paragraph, you can write anything in here!"
})

--[[
Name : <String> -- Name Of The Paragraph
Text = <String> -- Content Of The Paragraph
]]
```

# Notifying User
```lua
VirtexLib.Notification({
	Title = "VirtexLib",
	Text = "Hello",
	Time = 5,
	Image = "rbxassetid://123456789"
})

--[[
Title = <String> -- Title Of The Notification.
Text = <String> -- Text Of The Notification.
Time = <Number> -- duration Of The Notification.
Image = <String> -- Image Of The Notification.
]]
```

## Random Number
```lua
VirtexLib.RandomNumber(1, 100)
```

## Player Respawn
```lua
VirtexLib.Respawn()
```

## Destroying Interface
```lua
Window.Delete()
```

# Explanation
This Is Still In Beta Stage, And If I Find Any Bugs I Apologize, And Enjoy!

# Creator
## Programmer : MC Kuadrat
## Designer : MC Kuadrat
