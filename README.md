local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local under = Instance.new("TextButton")
local Frame_2 = Instance.new("Frame")
local TextLabel_2 = Instance.new("TextLabel")
local got = Instance.new("TextButton")

--Properties:

ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame.Position = UDim2.new(0.222558662, 0, 0.144219309, 0)
Frame.Size = UDim2.new(0, 691, 0, 471)
Frame.Visible = true
Frame.Active = true

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 222.000
TextLabel.Size = UDim2.new(0, 691, 0, 350)
TextLabel.Font = Enum.Font.Nunito
TextLabel.Text = "MADE BY: TheyCallMeRokuro When Using This Script You Must Agree To The Rules                           Rules: DO NOT ABUSE and, DO NOT TAKE CREDIT OVER THIS SCRIPT..  TheyCallMeRokuro IS THE ONLY OWNER"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextScaled = true
TextLabel.TextSize = 10.000
TextLabel.TextWrapped = true

under.Name = "under"
under.Parent = Frame
under.BackgroundColor3 = Color3.fromRGB(175, 175, 175)
under.BorderSizePixel = 0
under.Position = UDim2.new(0.354558617, 0, 0.817409754, 0)
under.Size = UDim2.new(0, 200, 0, 50)
under.Font = Enum.Font.SourceSans
under.Text = "I UnderStand"
under.TextColor3 = Color3.fromRGB(0, 0, 0)
under.TextSize = 40.000
under.MouseButton1Down:connect(function()
	Frame_2.Visible = true
end)

Frame_2.Parent = Frame
Frame_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame_2.Position = UDim2.new(-0.00175392628, 0, -0.000154361129, 0)
Frame_2.Size = UDim2.new(0, 691, 0, 471)
Frame_2.Visible = false

TextLabel_2.Parent = Frame_2
TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.BackgroundTransparency = 222.000
TextLabel_2.Size = UDim2.new(0, 691, 0, 350)
TextLabel_2.Font = Enum.Font.Nunito
TextLabel_2.Text = "New; KeyBinds: [ Q ] --Reset Ur Character [ Z ]--Gives You Force Field [ You Need Admin For Keybinds To Function ] [ Prefix = /] [ Type /cmds in Chat For A List of Commands]"
TextLabel_2.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_2.TextScaled = true
TextLabel_2.TextSize = 10.000
TextLabel_2.TextWrapped = true

got.Name = "got"
got.Parent = Frame_2
got.BackgroundColor3 = Color3.fromRGB(175, 175, 175)
got.BorderSizePixel = 0
got.Position = UDim2.new(0.354558617, 0, 0.817409754, 0)
got.Size = UDim2.new(0, 200, 0, 50)
got.Font = Enum.Font.SourceSans
got.Text = "Got It!"
got.TextColor3 = Color3.fromRGB(0, 0, 0)
got.TextSize = 40.000
got.MouseButton1Down:connect(function()
	Frame.Visible = false
	Frame_2.Visible = false
end)

function zigzag(X) return math.acos(math.cos(X*math.pi))/math.pi end

counter = 0

while wait(0.1)do
	Frame.BackgroundColor3 = Color3.fromHSV(zigzag(counter),1,1)
	Frame_2.BackgroundColor3 = Color3.fromHSV(zigzag(counter),1,1)

	counter = counter + 0.01
end

if Frame.Visible == false and Frame_2.Visible == false  then
	game.Players.LocalPlayer.Chatted:connect(function(msg)
		if string.sub(msg, 1, 5) "/obby" then
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump" then
					v:Destroy()
				end
			end
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump1" then
					v:Destroy()
				end
			end
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump2" then
					v:Destroy()
				end
			end
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump3" then
					v:Destroy()
				end
			end
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump4" then
					v:Destroy()
				end
			end
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump5" then
					v:Destroy()
				end
			end
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump6" then
					v:Destroy()
				end
			end
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump7" then
					v:Destroy()
				end
			end
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump8" then
					v:Destroy()
				end
			end
			for i,v in pairs(game.Workspace.Terrain["_Game"].Workspace.Obby:GetChildren()) do
				if v.Name == "Jump9" then
					v:Destroy()
				end
			end
			
		elseif string.sub(msg, 1, 5) == "/pads" then

			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-44.515686, 8.62999916, 93.947731)
			wait(0.10)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-40.7658501, 8.62999916, 94.2329865)
			wait(0.10)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-36.9654541, 8.62999916, 94.5093765)
			wait(0.10)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-32.928772, 8.62999916, 94.1272049)
			wait(0.10)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-28.7958775, 8.62999916, 94.5988312)
			wait(0.10)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-24.8093014, 8.62999916, 94.3677826)
			wait(0.10)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-20.7154179, 8.62999916, 94.4038391)
			wait(0.10)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-16.9880428, 8.62999916, 94.3027039)
			wait(0.10)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12.7740078, 8.6299963, 93.8409271)
			wait(0.10)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-7.30391502, 8.62999058, 95.0525208)
			wait(0.5)
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-40.9917717, 6.80253983, 57.8530731)
			
		elseif string.sub(msg, 1, 5) == "/cmds" then
			print("( COMMANDS ) [ /obby ]--Deletes Obby [ /pads]--Teliports You To All Pads")
			
		end
	end)
end

game:GetService("UserInputService").InputBegan:connect(function(inputObject, gameProcessedEvent)
	if gameProcessedEvent then return end
	if inputObject.KeyCode == Enum.KeyCode.Q then
		game:GetService'Players':Chat("reset me")
		
	if gameProcessedEvent then return end
	elseif inputObject.KeyCode == Enum.KeyCode.Z then
		game:GetService'Players':Chat("ff me")
		
	end
	end)
