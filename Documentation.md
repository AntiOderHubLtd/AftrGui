# 1. Loading a library.
Paste this in your code:
```lua
loadstring(game:HttpGet('https://antioderhub.lol/AftrUI'))()
--[[
The window creating automatically.
]]
```
# 2. Changing the title of window.
```lua
game.CoreGui.AftrGui.MainFrame.Title.Text = "Your Title"
```
# 3. Add a button.
```lua
local Button = AddContent("TextButton", "Name of the button", [[
print("Button pressed!)
]])
```
# 4. Add an input.
```lua
local Input = AddContent("TextBox","Your Text")
TextBox:GetPropertyChangedSignal("Text"):Connect(function()
print(TextBox.Text)
end)

--[[
Text of input - TextBox.Text
]]
```
# 5. Add a checkbox.
```lua
local Checkbox = AddContent("Checkbox", "Text of checkbox", [[
print("Checkbox value changed!")
wait(100)
]])
```
# 6. Add a toggle.
```lua
local Toggle = AddContent("Toggle", "Text of toggle", [[
print("Value of checkbox: true!")
]],[[
print("Value of checkbox: false!")
]])
```
# 7. Add a label.
```lua
local TextLabel = AddContent("TextLabel")
TextLabel.Text = "Your text here"
```
Enjoy the simple library!
Aftr.


