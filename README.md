local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

local jumpPower = 50

local function handleJump()
    if humanoid then
        humanoid.JumpPower = jumpPower
    end
end

game:GetService("UserInputService").InputBegan:Connect(function(input)
    if input.UserInputType == Enum.UserInputType.Keyboard then
        if input.KeyCode == Enum.KeyCode.Space then
            handleJump()
        end
    end
end)local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

local jumpPower = 50

local function handleJump()
    if humanoid then
        humanoid.JumpPower = jumpPower
    end
end

game:GetService("UserInputService").InputBegan:Connect(function(input)
    if input.UserInputType == Enum.UserInputType.Keyboard then
        if input.KeyCode == Enum.KeyCode.Space then
            handleJump()
        end
    end
end)
