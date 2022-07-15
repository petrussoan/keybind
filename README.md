--Hotkey close/open
function PopupGui()
	if script.Parent.Visible == true then script.Parent.Visible = false
	else script.Parent.Visible = true
	end
end

game:GetService("UserInputService").InputBegan:Connect(function(key)
	if key.KeyCode == Enum.KeyCode.V then
		PopupGui()
	end
end)
