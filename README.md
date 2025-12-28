local Players = game:GetService("Players")
local UserInputService = game:GetService("UserInputService")
local RunService = game:GetService("RunService")
local player = Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")
local root = character:WaitForChild("HumanoidRootPart")

-- Guardar spawn inicial
local spawnCFrame = root.CFrame

-- Crear GUI
local gui = Instance.new("ScreenGui")
gui.Name = "CASS_HUB"
gui.Parent = player:WaitForChild("PlayerGui")
gui.ResetOnSpawn = false

local frame = Instance.new("Frame", gui)
frame.Size = UDim2.new(0, 300, 0, 330)
frame.Position = UDim2.new(0.5, -150, 0.5, -165)
frame.BackgroundColor3 = Color3.fromRGB(0, 120, 255)
frame.Border
