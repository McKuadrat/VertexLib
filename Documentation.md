# VirtexUI Library
This guide for using VirtexUI Library!

# Booting The Gui
```lua
local VirtexLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/McKuadrat/VirtexLib/refs/heads/main/Source')))()
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

# Making Button
```lua
Tab2.AddButton({
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


## Getting User Image
```lua
VirtexLib.GetUserImage()
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
Programmer : MC Kuadrat\n
Designer : MC Kuadrat
