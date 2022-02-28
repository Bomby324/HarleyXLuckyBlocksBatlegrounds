-- Harley X Created By Anakin Skywalker#4504
game.StarterGui:SetCore("SendNotification", {
    Title = "Harley X";
    Text = "Created By Anakin Skywalker#4504";
    Duration = 15;
})

local MainModule = Instance.new("ScreenGui")
local Top = Instance.new("Frame")
local MainBackground = Instance.new("Frame")
local BlockTypes = Instance.new("ScrollingFrame")
local Block = Instance.new("TextButton")
local UIListLayout = Instance.new("UIListLayout")
local Block1 = Instance.new("TextButton")
local Block2 = Instance.new("TextButton")
local Block3 = Instance.new("TextButton")
local Block4 = Instance.new("TextButton")
local Block5 = Instance.new("TextButton")
local Block6 = Instance.new("TextButton")
local AmountNumber = Instance.new("TextBox")
local BlockTypeHolder = Instance.new("Frame")
local TypeText = Instance.new("TextLabel")
local GearAmountHolder = Instance.new("Frame")
local AmountText = Instance.new("TextLabel")
local AmountText_2 = Instance.new("TextLabel")
local Open = Instance.new("TextButton")
local Type = Instance.new("TextLabel")
local Title = Instance.new("TextLabel")
local Minimize = Instance.new("TextButton")

--Properties:

MainModule.Name = "MainModule"
MainModule.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
MainModule.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Top.Name = "Top"
Top.Parent = MainModule
Top.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Top.BorderColor3 = Color3.fromRGB(0, 0, 0)
Top.BorderSizePixel = 2
Top.Position = UDim2.new(0.189966559, 0, 0.407361925, 0)
Top.Size = UDim2.new(0.315719068, 0, 0.036809817, 0)
local UserInputService = game:GetService("UserInputService")

local gui = Top

local dragging
local dragInput
local dragStart
local startPos

local function update(input)
	local delta = input.Position - dragStart
	gui:TweenPosition(UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y), Enum.EasingDirection.InOut, Enum.EasingStyle.Linear, 0.15, true) -- This is what I changed
end

gui.InputBegan:Connect(function(input)
	if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
		dragging = true
		dragStart = input.Position
		startPos = gui.Position

		input.Changed:Connect(function()
			if input.UserInputState == Enum.UserInputState.End then
				dragging = false
			end
		end)
	end
end)

gui.InputChanged:Connect(function(input)
	if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
		dragInput = input
	end
end)

UserInputService.InputChanged:Connect(function(input)
	if input == dragInput and dragging then
		update(input)
	end
end)

MainBackground.Name = "MainBackground"
MainBackground.Parent = Top
MainBackground.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
MainBackground.BorderColor3 = Color3.fromRGB(0, 0, 0)
MainBackground.BorderSizePixel = 2
MainBackground.ClipsDescendants = true
MainBackground.Position = UDim2.new(0, 0, 0.978952289, 0)
MainBackground.Size = UDim2.new(0.999999881, 0, 8.95503139, 0)

BlockTypes.Name = "BlockTypes"
BlockTypes.Parent = MainBackground
BlockTypes.Active = true
BlockTypes.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
BlockTypes.BorderColor3 = Color3.fromRGB(0, 0, 0)
BlockTypes.BorderSizePixel = 2
BlockTypes.Position = UDim2.new(-5.28900905e-08, 0, 0.145169556, 0)
BlockTypes.Size = UDim2.new(0.313691497, 0, 0.854830325, 0)
BlockTypes.ScrollBarThickness = 0

Block.Name = "Block"
Block.Parent = BlockTypes
Block.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Block.BorderColor3 = Color3.fromRGB(0, 0, 0)
Block.BorderSizePixel = 2
Block.ClipsDescendants = true
Block.Position = UDim2.new(0.0662983581, 0, 0.0186115112, 0)
Block.Size = UDim2.new(0, 157, 0, 44)
Block.Font = Enum.Font.GothamBold
Block.Text = "Lucky Block"
Block.TextColor3 = Color3.fromRGB(255, 255, 0)
Block.TextScaled = true
Block.TextSize = 60.000
Block.TextStrokeTransparency = 0.000
Block.TextWrapped = true
Block.MouseButton1Down:Connect(function()
    Type.Text = "Lucky Block"
    Type.TextColor3 = Color3.fromRGB(255, 255, 0)
end)

UIListLayout.Parent = BlockTypes
UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
UIListLayout.Padding = UDim.new(0, 7)

Block1.Name = "Block1"
Block1.Parent = BlockTypes
Block1.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Block1.BorderColor3 = Color3.fromRGB(0, 0, 0)
Block1.BorderSizePixel = 2
Block1.ClipsDescendants = true
Block1.Position = UDim2.new(0.0662983581, 0, 0.0186115112, 0)
Block1.Size = UDim2.new(0, 157, 0, 44)
Block1.Font = Enum.Font.GothamBold
Block1.Text = "Super Block"
Block1.TextColor3 = Color3.fromRGB(255, 166, 201)
Block1.TextScaled = true
Block1.TextSize = 60.000
Block1.TextStrokeTransparency = 0.000
Block1.TextWrapped = true
Block1.MouseButton1Down:Connect(function()
    Type.Text = "Super Block"
    Type.TextColor3 = Color3.fromRGB(255, 166, 201)
end)

Block2.Name = "Block2"
Block2.Parent = BlockTypes
Block2.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Block2.BorderColor3 = Color3.fromRGB(0, 0, 0)
Block2.BorderSizePixel = 2
Block2.ClipsDescendants = true
Block2.Position = UDim2.new(0.0662983581, 0, 0.0186115112, 0)
Block2.Size = UDim2.new(0, 157, 0, 44)
Block2.Font = Enum.Font.GothamBold
Block2.Text = "Diamond Block"
Block2.TextColor3 = Color3.fromRGB(177, 234, 232)
Block2.TextScaled = true
Block2.TextSize = 60.000
Block2.TextStrokeTransparency = 0.000
Block2.TextWrapped = true
Block2.MouseButton1Down:Connect(function()
    Type.Text = "Diamond Block"
    Type.TextColor3 = Color3.fromRGB(177, 234, 232)
end)

Block3.Name = "Block3"
Block3.Parent = BlockTypes
Block3.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Block3.BorderColor3 = Color3.fromRGB(0, 0, 0)
Block3.BorderSizePixel = 2
Block3.ClipsDescendants = true
Block3.Position = UDim2.new(0.0662983581, 0, 0.0186115112, 0)
Block3.Size = UDim2.new(0, 157, 0, 44)
Block3.Font = Enum.Font.GothamBold
Block3.Text = "Rainbow Block"
Block3.TextColor3 = Color3.fromRGB(255, 255, 255)
Block3.TextScaled = true
Block3.TextSize = 60.000
Block3.TextStrokeTransparency = 0.000
Block3.TextWrapped = true
local t = 5; 
local rainbowloop = coroutine.wrap(function()
	while wait(0.1) do
		local hue = tick() % t / t
		local color = Color3.fromHSV(hue, 1, 1)
		Block3.TextColor3 = color
	end
end)

rainbowloop()

Block3.MouseButton1Down:Connect(function()
    Type.Text = "Rainbow Block"
    Type.TextColor3 = Block3.TextColor3
end)

Block4.Name = "Block4"
Block4.Parent = BlockTypes
Block4.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Block4.BorderColor3 = Color3.fromRGB(0, 0, 0)
Block4.BorderSizePixel = 2
Block4.ClipsDescendants = true
Block4.Position = UDim2.new(0.0662983581, 0, 0.0186115112, 0)
Block4.Size = UDim2.new(0, 157, 0, 44)
Block4.Font = Enum.Font.GothamBold
Block4.Text = "Galaxy Block"
Block4.TextColor3 = Color3.fromRGB(61, 0, 97)
Block4.TextScaled = true
Block4.TextSize = 60.000
Block4.TextStrokeTransparency = 0.000
Block4.TextWrapped = true
Block4.MouseButton1Down:Connect(function()
    Type.Text = "Galaxy Block"
    Type.TextColor3 = Color3.fromRGB(61, 0, 97)
end)

Block5.Name = "Block5"
Block5.Parent = BlockTypes
Block5.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Block5.BorderColor3 = Color3.fromRGB(0, 0, 0)
Block5.BorderSizePixel = 2
Block5.ClipsDescendants = true
Block5.Position = UDim2.new(0.0662983581, 0, 0.0186115112, 0)
Block5.Size = UDim2.new(0, 157, 0, 44)
Block5.Font = Enum.Font.GothamBold
Block5.Text = "Void Block"
Block5.TextColor3 = Color3.fromRGB(221, 221, 221)
Block5.TextScaled = true
Block5.TextSize = 60.000
Block5.TextStrokeTransparency = 0.000
Block5.TextWrapped = true
Block5.MouseButton1Down:Connect(function()
    Type.Text = "Void Block"
    Type.TextColor3 = Color3.fromRGB(221, 221, 221)
end)

Block6.Name = "Block6"
Block6.Parent = BlockTypes
Block6.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
Block6.BorderColor3 = Color3.fromRGB(0, 0, 0)
Block6.BorderSizePixel = 2
Block6.ClipsDescendants = true
Block6.Position = UDim2.new(0.0662983581, 0, 0.0186115112, 0)
Block6.Size = UDim2.new(0, 157, 0, 44)
Block6.Font = Enum.Font.GothamBold
Block6.Text = "Limited  Block"
Block6.TextColor3 = Color3.fromRGB(25, 107, 0)
Block6.TextScaled = true
Block6.TextSize = 60.000
Block6.TextStrokeTransparency = 0.000
Block6.TextWrapped = true
Block6.MouseButton1Down:Connect(function()
    Type.Text = "Limited Block"
    Type.TextColor3 = Color3.fromRGB(25, 107, 0)
end)

AmountNumber.Name = "AmountNumber"
AmountNumber.Parent = MainBackground
AmountNumber.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
AmountNumber.BorderColor3 = Color3.fromRGB(0, 0, 0)
AmountNumber.BorderSizePixel = 2
AmountNumber.ClipsDescendants = true
AmountNumber.Position = UDim2.new(0.424610049, 0, 0.335007191, 0)
AmountNumber.Size = UDim2.new(0.464471459, 0, 0.208448932, 0)
AmountNumber.Font = Enum.Font.GothamBold
AmountNumber.PlaceholderColor3 = Color3.fromRGB(178, 178, 178)
AmountNumber.PlaceholderText = "Please Enter A Number Here."
AmountNumber.Text = ""
AmountNumber.TextColor3 = Color3.fromRGB(255, 255, 0)
AmountNumber.TextScaled = true
AmountNumber.TextSize = 19.000
AmountNumber.TextStrokeTransparency = 0.000
AmountNumber.TextWrapped = true

BlockTypeHolder.Name = "BlockTypeHolder"
BlockTypeHolder.Parent = MainBackground
BlockTypeHolder.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
BlockTypeHolder.BorderColor3 = Color3.fromRGB(0, 0, 0)
BlockTypeHolder.BorderSizePixel = 2
BlockTypeHolder.ClipsDescendants = true
BlockTypeHolder.Position = UDim2.new(-5.28900905e-08, 0, -0.00744471792, 0)
BlockTypeHolder.Size = UDim2.new(0.317157745, 0, 0.148891971, 0)

TypeText.Name = "TypeText"
TypeText.Parent = BlockTypeHolder
TypeText.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TypeText.BackgroundTransparency = 1.000
TypeText.ClipsDescendants = true
TypeText.Position = UDim2.new(0, 0, 0.0657867417, 0)
TypeText.Size = UDim2.new(0.99999994, 0, 0.934212863, 0)
TypeText.Font = Enum.Font.GothamBold
TypeText.Text = "Block Type"
TypeText.TextColor3 = Color3.fromRGB(255, 255, 0)
TypeText.TextSize = 27.000
TypeText.TextStrokeTransparency = 0.000
TypeText.TextWrapped = true

GearAmountHolder.Name = "GearAmountHolder"
GearAmountHolder.Parent = MainBackground
GearAmountHolder.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
GearAmountHolder.BorderColor3 = Color3.fromRGB(0, 0, 0)
GearAmountHolder.BorderSizePixel = 2
GearAmountHolder.ClipsDescendants = true
GearAmountHolder.Position = UDim2.new(0.317157686, 0, -0.00744483154, 0)
GearAmountHolder.Size = UDim2.new(0.682842374, 0, 0.148891866, 0)

AmountText.Name = "AmountText"
AmountText.Parent = GearAmountHolder
AmountText.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
AmountText.BackgroundTransparency = 1.000
AmountText.ClipsDescendants = true
AmountText.Position = UDim2.new(0, 0, 0.0657867417, 0)
AmountText.Size = UDim2.new(1, 0, 0.934212863, 0)
AmountText.Font = Enum.Font.GothamBold
AmountText.Text = "Gear Amount"
AmountText.TextColor3 = Color3.fromRGB(255, 255, 0)
AmountText.TextSize = 37.000
AmountText.TextStrokeTransparency = 0.000
AmountText.TextWrapped = true

AmountText_2.Name = "AmountText"
AmountText_2.Parent = MainBackground
AmountText_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
AmountText_2.BackgroundTransparency = 1.000
AmountText_2.ClipsDescendants = true
AmountText_2.Position = UDim2.new(0.326323092, 0, 0.858637035, 0)
AmountText_2.Size = UDim2.new(0.665255845, 0, 0.137640625, 0)
AmountText_2.Font = Enum.Font.GothamBold
AmountText_2.Text = "TIP: The amount above is the amount of gears that you will open!"
AmountText_2.TextColor3 = Color3.fromRGB(178, 178, 178)
AmountText_2.TextScaled = true
AmountText_2.TextSize = 37.000
AmountText_2.TextStrokeTransparency = 0.000
AmountText_2.TextWrapped = true

Open.Name = "Open"
Open.Parent = MainBackground
Open.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
Open.BorderColor3 = Color3.fromRGB(0, 0, 0)
Open.BorderSizePixel = 2
Open.ClipsDescendants = true
Open.Position = UDim2.new(0.455000013, 0, 0.550000012, 0)
Open.Size = UDim2.new(0.402079761, 0, 0.145169795, 0)
Open.Font = Enum.Font.GothamBold
Open.Text = "Open Block!"
Open.TextColor3 = Color3.fromRGB(255, 255, 0)
Open.TextSize = 40.000
Open.TextStrokeTransparency = 0.000
Open.TextWrapped = true
Open.MouseButton1Down:Connect(function()
    if Type.Text == "Lucky Block" then
        for i=1, AmountNumber.Text do
            game:GetService("ReplicatedStorage").SpawnLuckyBlock:FireServer()
        end
    elseif Type.Text == "Super Block" then
        for i=1, AmountNumber.Text do
            game:GetService("ReplicatedStorage").SpawnSuperBlock:FireServer()
        end
    elseif Type.Text == "Diamond Block" then
        for i=1, AmountNumber.Text do
            game:GetService("ReplicatedStorage").SpawnDiamondBlock:FireServer()
        end
    elseif Type.Text == "Rainbow Block" then
        for i=1, AmountNumber.Text do
            game:GetService("ReplicatedStorage").SpawnRainbowBlock:FireServer()
        end
    elseif Type.Text == "Galaxy Block" then
        for i=1, AmountNumber.Text do
            game:GetService("ReplicatedStorage").SpawnGalaxyBlock:FireServer()
        end
    elseif Type.Text == "Void Block" then
        for i=1, AmountNumber.Text do
            game:GetService("ReplicatedStorage").SpawnSuperBlock:FireServer()
        end
    elseif Type.Text == "Limited Block" then
        for i=1, AmountNumber.Text do
            game:GetService("ReplicatedStorage").SpawnSuperBlock:FireServer()
        end
    end
end)

Type.Name = "Type"
Type.Parent = MainBackground
Type.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
Type.BorderColor3 = Color3.fromRGB(0, 0, 0)
Type.BorderSizePixel = 2
Type.ClipsDescendants = true
Type.Position = UDim2.new(0.503000021, 0, 0.243000001, 0)
Type.Size = UDim2.new(0.311958402, 0, 0.085528411, 0)
Type.Font = Enum.Font.GothamBold
Type.Text = "Lucky Block"
Type.TextColor3 = Color3.fromRGB(255, 255, 0)
Type.TextScaled = true
Type.TextSize = 37.000
Type.TextStrokeTransparency = 0.000
Type.TextWrapped = true

Title.Name = "Title"
Title.Parent = Top
Title.BackgroundColor3 = Color3.fromRGB(247, 0, 255)
Title.BackgroundTransparency = 1.000
Title.Position = UDim2.new(0, 0, -0.100000001, 0)
Title.Size = UDim2.new(0.596187174, 0, 1.01228452, 0)
Title.Font = Enum.Font.GothamBold
Title.Text = "Harley X | Lucky Blocks Battlegrounds"
Title.TextColor3 = Color3.fromRGB(255, 255, 0)
Title.TextScaled = true
Title.TextSize = 14.000
Title.TextStrokeTransparency = 0.000
Title.TextWrapped = true

Minimize.Name = "Minimize"
Minimize.Parent = Top
Minimize.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Minimize.BackgroundTransparency = 1.000
Minimize.Position = UDim2.new(0.937608302, 0, -0.100000001, 0)
Minimize.Size = UDim2.new(0.0623916797, 0, 1.10000002, 0)
Minimize.Font = Enum.Font.GothamSemibold
Minimize.Text = "-"
Minimize.TextColor3 = Color3.fromRGB(255, 255, 0)
Minimize.TextSize = 40.000
Minimize.TextStrokeTransparency = 0.000
Minimize.TextWrapped = true
Minimize.MouseButton1Down:Connect(function()
    if closed == false then
        MainBackground:TweenSize(UDim2.new(1, 0, 0, 0), 'In', 'Linear', '.6')
        wait(1.1)
        closed = true
    else
        MainBackground.Visible = true
        MainBackground:TweenSize(UDim2.new(1, 0, 8.955, 0), 'Out', 'Linear', '.6')
        closed = false
    end
end)

