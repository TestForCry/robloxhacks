	local Keylime = loadstring(game:HttpGet('https://strazos.xyz/files/6f3a77d335f20fc86c2e89ff.txt'))()
	loadstring(game:HttpGet('https://strazos.xyz/files/2f2dc012e71896f1a2313cd7.lua'))()
	wait(10)
	pcall(function()
	loadstring(game:HttpGet('https://strazos.xyz/files/86a645afd7877318a03df885.txt', true))()
	end)
	
	-- Treacherous Tower
	if game.GameId == 1383164929 then
		local Library = Keylime.new("Treacherous Tower")
	Library:Create("Toggle", "God Mode", function(thing)
		godmode = thing
	end, {Default = false})
	Library:Create("Toggle", "Inf Jump", function(thing)
		Jump = thing
	end, {Default = false})
	Library:Create("Slider", "Walkspeed", function(thing)
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = thing
	end, {Default = 16, MinValue = 16, MaxValue = 100})
	Library:Create("Slider", "Jump Height", function(thing)
		game.Players.LocalPlayer.Character.Humanoid.JumpPower = thing
	end, {Default = 50, MinValue = 50, MaxValue = 500})
	spawn(function()
	while wait() do
	if godmode == true then
		game.Workspace[game.Players.LocalPlayer.Name].KillScript.Disabled = true
	elseif godmode == false then
		 game.Workspace[game.Players.LocalPlayer.Name].KillScript.Disabled = false
	end

	end
	end)
	local UserInputService = game:GetService("UserInputService")
	local key = Enum.KeyCode.Space
	local function is()
	return UserInputService:IsKeyDown(key)
	end
	local function Input(input, gameProcessedEvent)
		while is() and Jump do
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
				wait(.1)
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Seated")
		end
	end
	UserInputService.InputBegan:Connect(Input)
	end

	-- Arsenal
	if game.GameId == 111958650 then
	local Library = Keylime.new("Main Functions")
	Library:Create("Toggle", "Inf Jump", function(thing)
		Jump = thing
	end, {Default = false})
	Library:Create("Button", "No Falldamage", function()
				game:GetService("ReplicatedStorage").Events.FallDamage:Destroy()
	end)
	
	Library:Create("Button", "Hitbox Extender", function()
		spawn(function()
			while wait() do
				for i,v in pairs (game.Players:GetChildren()) do
					for i2,v2 in pairs (game.Workspace[v.Name]:GetChildren()) do
						if v2.Name == "LowerTorso" then
							if v.Name ~= game.Players.LocalPlayer.Name and v.Team ~= game.Players.LocalPlayer.Team then
								if v2.CanCollide == true then
									v2.CanCollide = false
									v2.Size = Vector3.new(30,30,30)
									v2.Parent.HumanoidRootPart.Size = Vector3.new(30,30,30)
								end
							elseif v.Team == game.Players.LocalPlayer.Team and v.Name ~= game.Players.LocalPlayer.Name then
								if v2.Parent.HumanoidRootPart.Size ~= Vector3.new(1,2,1) and v2.Size ~= Vector3.new(2,0.4,1) then
									v2.CanCollide = true
									v2.Size = Vector3.new(2,0.4,1)
									v2.Parent.HumanoidRootPart.Size = Vector3.new(1,2,1)
								end
							end
						end
					end
				end
			end
		end)
	end)

	Library:Create("Toggle", "Kill All", function(thing)
		mine = thing
	end, {Default = false})
	
	distance = 5
	Library:Create("Toggle", "Lock Behind", function(thing)
		joe = thing
	end, {Default = false})
	Library:Create("Slider", "Distance", function(thing)
		distance = thing
	end, {Default = 5, MinValue = 2, MaxValue = 15})
	spawn(function()
		while wait() do
			for i,v in pairs(game.Players:GetPlayers()) do
				if v.Name ~= game.Players.LocalPlayer.Name and v.Team ~= game.Players.LocalPlayer.Team and v.Character:FindFirstChild("Spawned") and joe then
					repeat
						game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Character.HumanoidRootPart.CFrame * CFrame.new(0,0,distance)
						wait()
					until not v.Character:FindFirstChild("Spawned") or v.Team == game.Players.LocalPlayer.Team and joe 
				end
			end
		end
	end)
	
	local mt = getrawmetatable(game)
	local oldNamecall = mt.__namecall
	setreadonly(mt, false)

	mt.__namecall = newcclosure(function(self, ...)
    local args = {...}
    if tostring(self) == "HitPart" then
        for i,v in pairs(game.Players.GetPlayers(game.Players)) do
            if v.Character and v ~= game.Players.LocalPlayer and v.TeamColor ~= game.Players.LocalPlayer.TeamColor and mine then
                args[1] = v.Character.Head
                args[2] = v.Character.Head.Position
                for i = 1, 15 do
                    oldNamecall(self, unpack(args))
                end
            end
        end
    end
    return oldNamecall(self, ...)
end)

setreadonly(mt, true)
	
	Library:Create("Button", "Gun Mod", function()
			for i,v in pairs(getgc()) do
			if typeof(v) == "function" and debug.getinfo(v).name == "updateInventory" then
				for i2,v2 in pairs(getupvalues(v)) do
					game:GetService("RunService").Stepped:Connect(function()
						debug.setupvalue(v, 3, 69)
					end)
				end
			end
		end
		for i,v in pairs(getgc()) do
			if type(v) == 'function' and debug.getinfo(v).name == 'firebullet' then
				functionEnv = getfenv(v)
				break
			end
		end

		while wait() do
		functionEnv.recoil = 0 
		functionEnv.currentspread = 0 
		functionEnv.spreadmodifier = 0 
		end
	end)
	local UserInputService = game:GetService("UserInputService")
	local key = Enum.KeyCode.Space
	local function is()
	return UserInputService:IsKeyDown(key  )
	end
	local function Input(input, gameProcessedEvent)
		while is() and Jump do
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
				wait(.1)
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Seated")
		end
	end
	UserInputService.InputBegan:Connect(Input)
	end
	
	-- CBRO
	if game.GameId == 115797356 then
	local Library = Keylime.new("Main Functions")
	Library:Create("Toggle", "Inf Jump", function(thing)
		Jump = thing
	end, {Default = false})
	Library:Create("Button", "No Falldamage", function()
		game:GetService("ReplicatedStorage").Events.FallDamage:Destroy()
	end)
	
	Library:Create("Button", "Gun Mod", function()
	for i,v in pairs(game:GetService("ReplicatedStorage").Weapons:GetDescendants()) do
	if v.Name == "FireRate" then
                v.Value = 0
            end
            if v.Name == "Ammo" then
                v.Value = 9e9
            end
            if v.Name == "StoredAmmo" then
                v.Value = 9e9
            end
            if v.Name == "Auto" then
                v.Value = true
            end
	end
	end)
	
	Library:Create("Toggle", "Kill All", function(thing)
		mine = thing
	end, {Default = false})
	
	local mt = getrawmetatable(game)
	local oldNamecall = mt.__namecall
	setreadonly(mt, false)

	mt.__namecall = newcclosure(function(self, ...)
    local args = {...}
    if tostring(self) == "HitPart" then
        for i,v in pairs(game.Players.GetPlayers(game.Players)) do
            if v.Character and v ~= game.Players.LocalPlayer and v.TeamColor ~= game.Players.LocalPlayer.TeamColor and mine then
                args[1] = v.Character.Head
                args[2] = v.Character.Head.Position
                for i = 1, 15 do
                    oldNamecall(self, unpack(args))
                end
            end
        end
    end
    return oldNamecall(self, ...)
end)

setreadonly(mt, true)
	
	local UserInputService = game:GetService("UserInputService")
	local key = Enum.KeyCode.Space
	local function is()
	return UserInputService:IsKeyDown(key  )
	end
	local function Input(input, gameProcessedEvent)
		while is() and Jump do
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
				wait(.1)
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Seated")
		end
	end
	UserInputService.InputBegan:Connect(Input)
	end
	
	-- Big Paintball
	if game.GameId == 1247975681 then
		local Library = Keylime.new("Main Functions")
	Library:Create("Button", "Hitbox Extender (Buggy)", function()
		while wait() do
spawn(function()
while wait() do
for i,v in pairs (game.Players:GetChildren()) do
for i2,v2 in pairs (game.Workspace:GetChildren()) do
if v.Name == v2.Name then
local tester = v2:WaitForChild("Hitbox")
tester.Size = Vector3.new(100, 100, 100)
tester.Transparency = .6
tester.CanCollide = false
tester.Anchored = false
end
end
end
end
end)

spawn(function()
while wait() do
local play = game.Workspace[game.Players.LocalPlayer.Name]
local player = play:WaitForChild("Hitbox")
player.Size = Vector3.new(3.6, 6, 1.5)
player.Transparency = 1
player.CanCollide = false
player.Anchored = false
end
end)

spawn(function()
while wait() do
for i,v in pairs (game.Players:GetChildren()) do
for i2,v2 in pairs (game.Workspace:GetChildren()) do
if v.Name == v2.Name then
local tester = v2:WaitForChild("Hitbox")
local tester2 = tester:WaitForChild("WeldConstraint")
local tester3 = tester:WaitForChild("OriginalSize")
tester2:Destroy()
tester3:Destroy()
end
end
end
end
end)
end
	end)
Library:Create("Toggle", "Inf Jump", function(thing)
		Jump = thing
end, {Default = false})

Library:Create("Button", "Gun Mod", function()
	for i,v in pairs(getgc(true)) do
    if type(v) == 'table' and rawget(v, "damage") then
        v.firerate = 0.00001
        v.automatic = true
        v.velocity = 1000
    end
end
	end)
	
local UserInputService = game:GetService("UserInputService")
	local key = Enum.KeyCode.Space
	local function is()
	return UserInputService:IsKeyDown(key  )
	end
	local function Input(input, gameProcessedEvent)
		while is() and Jump do
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
				wait(.1)
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Seated")
		end
	end
	UserInputService.InputBegan:Connect(Input)	
end
	
	-- Strucid
if game.GameId == 833423526 then
	local Library = Keylime.new("Main Functions")
	Library:Create("Toggle", "Inf Jump", function(thing)
		Jump = thing
	end, {Default = false})
	
	Library:Create("Button", "God Mode", function()
	local ezpz2 = game.Workspace[game.Players.LocalPlayer.Name].Shield
	ezpz2:Destroy()
	end)
	
	Library:Create("Button", "No Falldamage", function()
	local StrucidNetwork = require(game:GetService("ReplicatedStorage").NetworkModule)
	local old = StrucidNetwork.FireServer
	StrucidNetwork.FireServer = newcclosure(function(self, action, ...)
    if action == "FallDamage" then
    return
    end
    return old(self, action, ...)
end)
end)
	
Library:Create("Button", "Gun Mod", function()
    spawn(function()
        while wait(5) do
            for i,v in pairs(debug.getupvalues(getsenv(game:GetService("Players").LocalPlayer.PlayerGui.MainGui.MainLocal).Reload)) do
                if i == 3 then
                    gunTbl = v
                end
            end
            game:GetService("RunService").Stepped:Connect(function()
                gunTbl.Debounce = 0.01
            end)
                    getsenv(game:GetService("Players").LocalPlayer.PlayerGui.MainGui.MainLocal).CameraRecoil = function()
                end
        end
    end)
end)

	local key = Enum.KeyCode.Space
	local function is()
	return UserInputService:IsKeyDown(key  )
	end
	local function Input(input, gameProcessedEvent)
		while is() and Jump do
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
				wait(.1)
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Seated")
		end
	end
	UserInputService.InputBegan:Connect(Input)	
end

local Keylime = loadstring(game:HttpGet('https://strazos.xyz/files/5f83c2d2ce76f33d75fdb818.txt'))()
local person = game.Players.LocalPlayer.Character.HumanoidRootPart

	-- Flee The Facility
if game.GameId == 372226183 then
    local Library = Keylime.new("Main Functions")
        Library:Create("Slider", "Walkspeed", function(thing)
    		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = thing
    	end, {Default = 16, MinValue = 16, MaxValue = 100})
    
    Library:Create("Button", "Third Person (Beast)", function()
		game:GetService('Players').LocalPlayer.CameraMode = 'Classic'
        game:GetService("Players").LocalPlayer.CameraMaxZoomDistance = 500
	end)
    
    Library:Create("Button", "Auto Computers", function()
	
    for i,v in pairs (game.Workspace:GetDescendants()) do
        spawn(function()
			while wait() do
				game.ReplicatedStorage.RemoteEvent:FireServer("SetPlayerMinigameResult", true)
			end
		end)
        repeat 
            for i2,v2 in pairs (game.Workspace:GetDescendants()) do
                if v2.Name == "ComputerTrigger1" and v2.Parent.Name ~= "PrefabComputerTable" then
                    print("test")
                    person.CFrame = v2.CFrame
                        wait(1)
                    game:GetService("ReplicatedStorage").RemoteEvent:FireServer("Input", "Action", true)
                        wait(1)
                    game:GetService("ReplicatedStorage").RemoteEvent:FireServer("Input", "Action", true)
                    game:GetService("ReplicatedStorage").RemoteEvent:FireServer("Input", "Action", true)
                        wait(1)
                    game:GetService("ReplicatedStorage").RemoteEvent:FireServer("Input", "Action", true)
                    game:GetService("ReplicatedStorage").RemoteEvent:FireServer("Input", "Action", true)
                        wait(8)
                end 
            end
        until game:GetService("ReplicatedStorage").ComputersLeft.Value == 0
    end
    end)
    
    Library:Create("Button", "Win (After Computers)", function()
		
		for i,v in pairs (game.Workspace:GetDescendants()) do
            if v.Name == "ExitArea" then
                person.CFrame = v.CFrame
            end
        end
		
	end)

    Library:Create("Toggle", "Noclip", function(thing)
		noclip = thing
	end, {Default = false})


    game:GetService('RunService').Stepped:connect(function()
        if noclip then
            game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
    	end
    end)
end

-- Lost
	if game.GameId == 597889174 then
	local person = game.Players.LocalPlayer.Character.HumanoidRootPart
	local Library2 = Keylime.new("Main Functions")
	
	Library2:Create("Toggle", "Inf Jump", function(thing)
		Jump = thing
	end, {Default = false})
	
	Library2:Create("Button", "Fullbright", function()
		game.Lighting.FogEnd = 10000
		game.Lighting.GlobalShadows = true
		game.Lighting.Ambient = Color3.new(1,1,1)
		game.Lighting.ClockTime = 13
		game.Lighting.Brightness = 2
	end)
	
	Library2:Create("Button", "Third Person", function()
		game:GetService('Players').LocalPlayer.CameraMode = 'Classic'
        game:GetService("Players").LocalPlayer.CameraMaxZoomDistance = 500
	end)
	
	Library2:Create("Button", "No Drown", function()
		local mt = getrawmetatable(game)
    setreadonly(mt, false)
    local oldNamecall = mt.__namecall

    mt.__namecall = newcclosure(function(self, ...)
    if tostring(self) == "Drown" then
      return
    end
    return oldNamecall(self, ...)
    end)

setreadonly(mt, true)
	end)
	
	local Library = Keylime.new("Raiding Tools")
	Library:Create("Toggle", "Wall", function(thing)
		wall = thing
	end, {Default = false})
	Library:Create("Toggle", "Doorway", function(thing2)
		doorway = thing2
	end, {Default = false})
	Library:Create("Toggle", "Floor", function(thing3)
		Floor = thing3
	end, {Default = false})
	
	Library:Create("Toggle", "Item Esp", function(thing)
		lolok = thing
	end, {Default = false})
	
	local cont = function(hook)
		local core = game:GetService("CoreGui")
		local gamer = Instance.new("BillboardGui")
		local frame = Instance.new("Frame")
		local namey = Instance.new("TextLabel")
		gamer.Parent = core
		gamer.Name = "goneisstupid"
		gamer.AlwaysOnTop = true
		gamer.Size = UDim2.new(2, 0, 2, 0)
		frame.BackgroundTransparency = 0.4
		frame.BorderSizePixel = 0
		frame.Size = UDim2.new(1, 0, 1, 0)
		frame.Parent = gamer
		gamer.Adornee = hook
		spawn(function()
			while wait() do
				if lolok then
					frame.Visible = true
				elseif not lolok then
					frame.Visible = false
				end
			end
		end)
	end
	
	for i,v in pairs(game.Workspace.Containers:GetDescendants()) do
		if v.ClassName == "Part" then
			cont(v)
		end
	end
	
	spawn(function()
	while wait() do
	if wall then
	for i,v in pairs (game:GetService("Workspace").BuiltObjects:GetChildren()) do
		if v.Name == "Wall" then
			v.Wall.Transparency = .7
		end
	end
		elseif not wall then
			for i,v in pairs (game:GetService("Workspace").BuiltObjects:GetChildren()) do
				if v.Name == "Wall" then
					v.Wall.Transparency = 0
				end
			end 
	end
	end
	end)
	spawn(function()
	while wait() do
	if doorway then
	for i,v in pairs (game:GetService("Workspace").BuiltObjects:GetChildren()) do
		if v.Name == "Doorway" then
			v.Doorway.Transparency = .7
		end
	end
		elseif not doorway then
			for i,v in pairs (game:GetService("Workspace").BuiltObjects:GetChildren()) do
				if v.Name == "Doorway" then
					v.Doorway.Transparency = 0
				end
			end
	end
	end
	end)
	spawn(function()
	while wait() do
	if Floor then
	for i,v in pairs (game:GetService("Workspace").BuiltObjects:GetChildren()) do
		if v.Name == "Floor" then
			v.Floor.Transparency = .7
		end
	end
		elseif not doorway then
			for i,v in pairs (game:GetService("Workspace").BuiltObjects:GetChildren()) do
				if v.Name == "Floor" then
					v.Floor.Transparency = 0
				end
			end 
	end
	end
	end)
	
	local UserInputService = game:GetService("UserInputService")
	local key = Enum.KeyCode.Space
	local function is()
	return UserInputService:IsKeyDown(key)
	end
	local function Input(input, gameProcessedEvent)
		while is() and Jump do
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
				wait(2)
				game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Seated")
		end
	end
	UserInputService.InputBegan:Connect(Input)
	end
	
	-- Spider
	if game.GameId == 1776914212 then
	local Library = Keylime.new("Main Functions")

    local esp = function(hook)
    local core = game:GetService("CoreGui")
    local gamer = Instance.new("BillboardGui")
    local frame = Instance.new("Frame")
    local namey = Instance.new("TextLabel")
    gamer.Parent = core
    gamer.Name = "goneisstupid"
    gamer.AlwaysOnTop = true
    gamer.Size = UDim2.new(6, 0, 3, 0)
    frame.BackgroundTransparency = 0.4
    frame.BorderSizePixel = 2
    frame.Size = UDim2.new(1, 0, 1, 0)
    frame.Parent = gamer
    gamer.Adornee = hook
    end
    
    local playeresp = function(hook)
    local core = game:GetService("CoreGui")
    local gamer = Instance.new("BillboardGui")
    local frame = Instance.new("Frame")
    local namey = Instance.new("TextLabel")
    gamer.Parent = core
    gamer.Name = "goneisstupid"
    gamer.AlwaysOnTop = true
    gamer.Size = UDim2.new(4, 0, 5, 0)
    frame.BackgroundTransparency = 0.4
    frame.BorderSizePixel = 2
    frame.Size = UDim2.new(1, 0, 1, 0)
    frame.Parent = gamer
    gamer.Adornee = hook
    end
    
	Library:Create("Textbox", "Player Name", function(thing)
		_G.telename = thing
		person.CFrame = game.Workspace[_G.telename].HumanoidRootPart.CFrame
	end)
	
    local itemesp = function(hook, text, size1, size2)
    local core = game:GetService("CoreGui")
    local gamer = Instance.new("BillboardGui")
    local frame = Instance.new("Frame")
    local textthing = Instance.new("TextLabel")
    gamer.Parent = core
    gamer.Name = "goneisstupid"
    gamer.AlwaysOnTop = true
    gamer.Size = UDim2.new(size1, 0, size2, 0)
    frame.BackgroundTransparency = .4
    frame.Size = UDim2.new(1, 0, 1, 0)
    frame.Parent = gamer
    gamer.Adornee = hook
    textthing.Text = text
    textthing.TextSize = 12
    textthing.Visible = true
    textthing.Size = UDim2.new(0, .8, 0, .5)
    textthing.Parent = frame
    end
    
    Library:Create("Button", "Spider Esp (Use as Player)", function()
    	for i,v in pairs (game.Players:GetPlayers()) do
            for i2,v2 in pairs (game.Workspace[v.Name]:GetChildren()) do
                if v2.Name == "IsSpiderCharacter" then
                    espthing = v2.Parent.HumanoidRootPart
                    esp(espthing, 6, 3)
                end
            end
        end
        print("loaded spider esp")
        warn("loaded spider esp")
    end)
    
    Library:Create("Button", "Player Esp (Use as Spider)", function()
    	for i,v in pairs (game.Players:GetPlayers()) do
            for i2,v2 in pairs (game.Workspace[v.Name]:GetChildren()) do
                if v2.Parent.Name ~= game.Players.LocalPlayer.Name then
                    if v2.Name == "IsSpiderCharacter" then
                        break
                    end
                    if v2.Name == "HumanoidRootPart" then
                        playeresp(v2)
                    end
                end
            end
        end
        print("loaded player esp")
        warn("loaded player esp")
    end)
    
    Library:Create("Button", "Item Esp   (Use as Player)", function()
        for i,v in pairs (game:GetService("Workspace").Items:GetDescendants()) do
            if v.Name == "Hitbox" or v.Name == "Handle" then
                itemesp(v, "test", 1, 1)
            end
        end
end)
    end
