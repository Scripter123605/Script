local player = game.Players.LocalPlayer
local sound = Instance.new("Sound")
sound.SoundId = "rbxassetid://142376088"
sound.Volume = 5
sound.Looped = true
sound.PlaybackSpeed = 0.75
sound.Parent = workspace

local gui = Instance.new("ScreenGui", game.CoreGui)
gui.ResetOnSpawn = false

local frame = Instance.new("Frame", gui)
frame.Size = UDim2.new(0, 200, 0, 120)
frame.Position = UDim2.new(0.5, -100, 0.4, 0)
frame.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
frame.Active = true
frame.Draggable = true

local playButton = Instance.new("TextButton", frame)
playButton.Size = UDim2.new(1, -20, 0, 40)
playButton.Position = UDim2.new(0, 10, 0, 10)
playButton.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
playButton.TextColor3 = Color3.new(1, 1, 1)
playButton.Text = "Play"

local label = Instance.new("TextLabel", frame)
label.Size = UDim2.new(1, -10, 0, 20)
label.Position = UDim2.new(0, 5, 1, -25)
label.Text = "Made by BaconGodGaming YT"
label.TextColor3 = Color3.new(1, 1, 1)
label.BackgroundTransparency = 1
label.TextScaled = true

local openButton = Instance.new("TextButton", gui)
openButton.Size = UDim2.new(0, 50, 0, 30)
openButton.Position = UDim2.new(1, -60, 0.5, -15)
openButton.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
openButton.TextColor3 = Color3.new(1, 1, 1)
openButton.Text = "Open"
openButton.Visible = false

local playing = false

playButton.MouseButton1Click:Connect(function()
	if not playing then
		sound:Play()
		playButton.Text = "Pause"
	else
		sound:Pause()
		playButton.Text = "Play"
	end
	playing = not playing
end)

local closeBtn = Instance.new("TextButton", frame)
closeBtn.Size = UDim2.new(0, 30, 0, 30)
closeBtn.Position = UDim2.new(1, -35, 0, 5)
closeBtn.BackgroundColor3 = Color3.fromRGB(200, 50, 50)
closeBtn.Text = "X"
closeBtn.TextColor3 = Color3.new(1, 1, 1)

closeBtn.MouseButton1Click:Connect(function()
	frame.Visible = false
	openButton.Visible = true
end)

openButton.MouseButton1Click:Connect(function()
	frame.Visible = true
	openButton.Visible = false
end)
