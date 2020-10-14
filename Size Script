function giant(p, size)	
	local pchar = p.Character
	if pchar then
		local function scale(chr,scl)
		
			for _,v in pairs(pchar:GetChildren()) do
				if v:IsA("Hat") then
					v:Clone()
					v.Parent = game.Lighting
				end
			end
				
		    local Head = chr['Head']
		    local Torso = chr['Torso']
		    local LA = chr['Left Arm']
		    local RA = chr['Right Arm']
		    local LL = chr['Left Leg']
		    local RL = chr['Right Leg']
		    local HRP = chr['HumanoidRootPart']
		
		    wait(0.1)
		   
		    Head.formFactor = 3
		    Torso.formFactor = 3
		    LA.formFactor = 3
		    RA.formFactor = 3
		    LL.formFactor = 3
		    RL.formFactor = 3
		    HRP.formFactor = 3
		    
		    Head.Size = Vector3.new(scl * 2, scl, scl)
		    Torso.Size = Vector3.new(scl * 2, scl * 2, scl)
		    LA.Size = Vector3.new(scl, scl * 2, scl)
		    RA.Size = Vector3.new(scl, scl * 2, scl)
		    LL.Size = Vector3.new(scl, scl * 2, scl)
		    RL.Size = Vector3.new(scl, scl * 2, scl)
		    HRP.Size = Vector3.new(scl * 2, scl * 2, scl)
		    
		    local Motor1 = Instance.new('Motor6D', Torso)
		    Motor1.Part0 = Torso
		    Motor1.Part1 = Head
	    	Motor1.C0 = CFrame.new(0, 1 * scl, 0) * CFrame.Angles(-1.6, 0, 3.1)
	    	Motor1.C1 = CFrame.new(0, -0.5 * scl, 0) * CFrame.Angles(-1.6, 0, 3.1)
	    	Motor1.Name = "Neck"
				    
	    	local Motor2 = Instance.new('Motor6D', Torso)
	    	Motor2.Part0 = Torso
	    	Motor2.Part1 = LA
	    	Motor2.C0 = CFrame.new(-1 * scl, 0.5 * scl, 0) * CFrame.Angles(0, -1.6, 0)
	    	Motor2.C1 = CFrame.new(0.5 * scl, 0.5 * scl, 0) * CFrame.Angles(0, -1.6, 0)
	    	Motor2.Name = "Left Shoulder"
	    	
	    	local Motor3 = Instance.new('Motor6D', Torso)
	   		Motor3.Part0 = Torso
	    	Motor3.Part1 = RA
	    	Motor3.C0 = CFrame.new(1 * scl, 0.5 * scl, 0) * CFrame.Angles(0, 1.6, 0)
	    	Motor3.C1 = CFrame.new(-0.5 * scl, 0.5 * scl, 0) * CFrame.Angles(0, 1.6, 0)
	    	Motor3.Name = "Right Shoulder"
	    	
	    	local Motor4 = Instance.new('Motor6D', Torso)
	    	Motor4.Part0 = Torso
	    	Motor4.Part1 = LL
	    	Motor4.C0 = CFrame.new(-1 * scl, -1 * scl, 0) * CFrame.Angles(0, -1.6, 0)
	    	Motor4.C1 = CFrame.new(-0.5 * scl, 1 * scl, 0) * CFrame.Angles(0, -1.6, 0)
	    	Motor4.Name = "Left Hip"
	    	
	    	local Motor5 = Instance.new('Motor6D', Torso)
	    	Motor5.Part0 = Torso
	    	Motor5.Part1 = RL
	    	Motor5.C0 = CFrame.new(1 * scl, -1 * scl, 0) * CFrame.Angles(0, 1.6, 0)
	    	Motor5.C1 = CFrame.new(0.5 * scl, 1 * scl, 0) * CFrame.Angles(0, 1.6, 0)
	    	Motor5.Name = "Right Hip"
	    	
	    	local Motor6 = Instance.new('Motor6D', HRP)
	    	Motor6.Part0 = HRP
	    	Motor6.Part1 = Torso
	    	Motor6.C0 = CFrame.new(0, 0, 0) * CFrame.Angles(-1.6, 0, -3.1)
	    	Motor6.C1 = CFrame.new(0, 0, 0) * CFrame.Angles(-1.6, 0, -3.1)
	    	    
		end
		
		scale(pchar, size)
		pchar.Humanoid.WalkSpeed = 15 * size
	
		for _,v in pairs(game.Lighting:GetChildren()) do
			if v:IsA("Hat") then
				v.Parent = pchar
			end
		end
	end
end

local plr = game.Players.LocalPlayer
giant(plr,1)


local csize = 1

local sgui = Instance.new("ScreenGui", game.Players.LocalPlayer.PlayerGui)
local base = Instance.new("Frame", sgui)
base.BackgroundTransparency = 1
base.Size = UDim2.new(0, 110, 0, 200)
base.Position = UDim2.new(1, -120, 1, -180)
local indicator = Instance.new("TextLabel", base)
indicator.Size = UDim2.new(1, 0, 0, 25)
indicator.TextColor3 = Color3.new(1, 1, 1)
indicator.BackgroundTransparency = 0
indicator.FontSize = Enum.FontSize.Size18
indicator.Font = Enum.Font.SourceSans
indicator.Text = "Current Size: 3"
local PlusOne = Instance.new("TextButton", base)
PlusOne.BackgroundColor3 = Color3.new(214/255, 214/255, 214/255)
PlusOne.Position = UDim2.new(0, 0, 0, 40)
PlusOne.Size = UDim2.new(1, 0, 0.5, -50)
PlusOne.BorderSizePixel = 2
PlusOne.Font = Enum.Font.SourceSansBold
PlusOne.FontSize = Enum.FontSize.Size24
PlusOne.Text = "+.1 Size"
local MinusOne = Instance.new("TextButton", base)
MinusOne.BackgroundColor3 = Color3.new(214/255, 214/255, 214/255)
MinusOne.Position = UDim2.new(0, 0, 0.5, 10)
MinusOne.Size = UDim2.new(1, 0, 0.5, -50)
MinusOne.Text = "-.1 Size"
MinusOne.BorderSizePixel = 2
MinusOne.Font = Enum.Font.SourceSansBold
MinusOne.FontSize = Enum.FontSize.Size24

PlusOne.MouseButton1Down:connect(function()
	csize = csize + .1
	giant(plr, csize)
	indicator.Text = "Current Size: "..tostring(csize)
end)

MinusOne.MouseButton1Down:connect(function()
	csize = csize - .1
	giant(plr, csize)
	indicator.Text = "Current Size: "..tostring(csize)
end)
