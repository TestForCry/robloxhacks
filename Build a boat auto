local LocalPlayer = game:GetService("Players").LocalPlayer
local ui = loadstring(game:GetObjects("rbxassetid://4133667265")[1].Source)("Library by wally")
local w = ui:CreateWindow('Automated')
w:Section('Autofarms')
local b = w:Button("Autofarm (Forever)", function()
    print("Autofarm Activated (Forever)")
    vu = game:GetService("VirtualUser")
    game:GetService("Players").LocalPlayer.Idled:connect(function()
        vu:Button2Down(Vector2.new(0, 0), workspace.CurrentCamera.CFrame)
        wait(1)
        vu:Button2Up(Vector2.new(0, 0), workspace.CurrentCamera.CFrame)
    end)
    print("Anti-Afk Succes!")
    while true do
        spawn(function()
        game:getService("RunService"):BindToRenderStep("NoClip",0,function()
        pcall(function()
        if not game.Players.LocalPlayer.Character:findFirstChildOfClass("Humanoid") then return end
        if not running == true then return end
        game.Players.LocalPlayer.Character:findFirstChildOfClass("Humanoid"):ChangeState(11)
        end)
        end)
        end)
        
        local checks = workspace.BoatTerrains:getDescendants()
        for i=1,#checks do
        running = true
        if checks[i].Name == "DarknessPart" or checks[i].Name == "GatePart" then
        checks[i].Transparency = 0
        if game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = checks[i].CFrame
        end
        wait(0.42)
        end
        end
        
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = workspace.GoldenChest.Collider.CFrame
        repeat
        if game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") then
        game.Players.LocalPlayer.Character.Humanoid.Jump = true
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = workspace.GoldenChest.Collider.CFrame
        end
        wait()
        until not game.Players.LocalPlayer.Character:FindFirstChild("Humanoid")
        running = false
        wait()
        end
    end)
    local b = w:Button("Autofarm (Once)", function()
        print("Autofarm Activated (Once)")
        spawn(function()
            game:getService("RunService"):BindToRenderStep("NoClip",0,function()
            pcall(function()
            if not game.Players.LocalPlayer.Character:findFirstChildOfClass("Humanoid") then return end
            if not running == true then return end
            game.Players.LocalPlayer.Character:findFirstChildOfClass("Humanoid"):ChangeState(11)
            end)
            end)
            end)
            
            local checks = workspace.BoatTerrains:getDescendants()
            for i=1,#checks do
            running = true
            if checks[i].Name == "DarknessPart" or checks[i].Name == "GatePart" then
            checks[i].Transparency = 0
            if game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = checks[i].CFrame
            end
            wait(0.42)
            end
            end
            
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = workspace.GoldenChest.Collider.CFrame
            repeat
            if game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") then
            game.Players.LocalPlayer.Character.Humanoid.Jump = true
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = workspace.GoldenChest.Collider.CFrame
            end
            wait()
            until not game.Players.LocalPlayer.Character:FindFirstChild("Humanoid")
            running = false
        end)
        local b = w:Button("Autofarm Treasure (Forever)", function()
            print("Autofarm Treasure Activated (Forever)")
            vu = game:GetService("VirtualUser")
    game:GetService("Players").LocalPlayer.Idled:connect(function()
        vu:Button2Down(Vector2.new(0, 0), workspace.CurrentCamera.CFrame)
        wait(1)
        vu:Button2Up(Vector2.new(0, 0), workspace.CurrentCamera.CFrame)
    end)
    print("Anti-Afk Succes!")
            while true do
                spawn(function()
                game:getService("RunService"):BindToRenderStep("NoClip",0,function()
                pcall(function()
                if not game.Players.LocalPlayer.Character:findFirstChildOfClass("Humanoid") then return end
                if not running == true then return end
                game.Players.LocalPlayer.Character:findFirstChildOfClass("Humanoid"):ChangeState(11)
                end)
                end)
                end)
                
                local checks = workspace.BoatTerrains:getDescendants()
                for i=1,#checks do
                running = true
                if checks[i].Name == "LockHolePart1" or checks[i].Name == "LockHolePart2" then
                checks[i].Transparency = 0
                if game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = checks[i].CFrame
                end
                wait(0.42)
                end
                end
                
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = workspace.GoldenChest.Collider.CFrame
                repeat
                if game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") then
                game.Players.LocalPlayer.Character.Humanoid.Jump = true
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = workspace.GoldenChest.Collider.CFrame
                end
                wait()
                until not game.Players.LocalPlayer.Character:FindFirstChild("Humanoid")
                running = false
                wait()
                end
            end)
            local b = w:Button("Autofarm Treasure (Once)", function()
                print("Autofarm Treasure Activated (Once)")
                spawn(function()
                    game:getService("RunService"):BindToRenderStep("NoClip",0,function()
                    pcall(function()
                    if not game.Players.LocalPlayer.Character:findFirstChildOfClass("Humanoid") then return end
                    if not running == true then return end
                    game.Players.LocalPlayer.Character:findFirstChildOfClass("Humanoid"):ChangeState(11)
                    end)
                    end)
                    end)
                    
                    local checks = workspace.BoatTerrains:getDescendants()
                    for i=1,#checks do
                    running = true
                    if checks[i].Name == "LockHolePart1" or checks[i].Name == "LockHolePart2" then
                    checks[i].Transparency = 0
                    if game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") then
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = checks[i].CFrame
                    end
                    wait(0.42)
                    end
                    end
                    
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = workspace.GoldenChest.Collider.CFrame
                    repeat
                    if game.Players.LocalPlayer.Character:FindFirstChild("Humanoid") then
                    game.Players.LocalPlayer.Character.Humanoid.Jump = true
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = workspace.GoldenChest.Collider.CFrame
                    end
                    wait()
                    until not game.Players.LocalPlayer.Character:FindFirstChild("Humanoid")
                    running = false
                end)
                w:Section('Open Chests')
local IBFS = workspace:WaitForChild("ItemBoughtFromShop", 1)
    w:Dropdown("Chest Type", {
        list = {
            "Common Chest",
            "Uncommon Chest",
            "Rare Chest",
            "Epic Chest",
            "Legendary Chest"
        },
        location = shared,
        flag = "chesttype"
    })
    w:Button("Open Chest", function()
            IBFS:FireServer(shared.chesttype or "Common Chest")
            print("Chest Successfully Opened")
        end)
local qm = workspace:WaitForChild("QuestMakerEvent", 1)
if qm then
    w:Section("Open Quests")
    w:Dropdown("Quest Name", {
        list = {
            "Cloud Quest",
            "Target Quest",
            "Ramp Quest",
            "Find Me Quest",
            "Dragon Quest",
            "The Box Quest",
            "Rings Quest",
            "Soccor Quest"
        },
        location = shared,
        flag = "questtype"
    })
    w:Button("Open Quest", function()
        qm:FireServer(({
            ["Cloud Quest"] = 1,
            ["Target Quest"] = 2,
            ["Ramp Quest"] = 3,
            ["Find Me Quest"] = 4,
            ["Dragon Quest"] = 5,
            ["The Box Quest"] = 6,
            ["Rings Quest"] = 7,
            ["Soccor Quest"] = 8
        })[shared.questtype or "Cloud Quest"])
        print("Quest Successfully Made")
    end)
end
w:Section("Codes")
local b = w:Button("Redeem Codes", function()
    RedeemCode = game:GetService("Workspace").CheckCodeFunction
    RedeemCode:InvokeServer("=D")
    RedeemCode:InvokeServer("=p")
    RedeemCode:InvokeServer("hi")
    RedeemCode:InvokeServer("squid army")
    RedeemCode:InvokeServer("chillthrill709 was here")
    RedeemCode:InvokeServer("TTTRRREEEAAASSSUUURRREEE")
print("Codes Activated")
end)
local b = w:Button("Share Codes", function()
    print("This Can Take Up To 15 Seconds")
    SMR = game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest
    SMR:FireServer("Here Are Some Codes For All Of You!", "All")
    SMR:FireServer("Currently There Are 6 Codes.", "All")
    wait(2.5)
    SMR:FireServer("Code1: =D", "All")
    wait(2.5)
    SMR:FireServer("Code2: =p", "All")
    wait(2.5)
    SMR:FireServer("Code3: hi", "All")
    wait(2.5)
    SMR:FireServer("Code4: squid army", "All")
    wait(2.5)
    SMR:FireServer("Code5: chillthrill709 was here", "All")
    wait(2.5)
    SMR:FireServer("Code6: TTTRRREEEAAASSSUUURRREEE", "All")
    print("Codes Shared")
end)
local w = ui:CreateWindow('Character Cheats')
local b = w:Button("Water Godmode", function()
    LocalPlayerName = game:GetService("Players").LocalPlayer.Name
    LocalPlayerWorkspace = game:GetService("Workspace")[LocalPlayerName]
    LocalPlayerWorkspace.WaterDetector:Destroy()
    print("Water Godmode Enabled")
end)
local b = w:Button("Noclip (n)", function()
   noclip = false
game:GetService('RunService').Stepped:connect(function()
if noclip then
game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
end
end)
end)
plr = game.Players.LocalPlayer
mouse = plr:GetMouse()
mouse.KeyDown:connect(function(key)

if key == "n" then
noclip = not noclip
game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
end
end)
print("Noclip Loaded! Press 'n' To Toggle On/Off")
local box = w:Box('WalkSpeed', {
    flag = "ws";
    type = 'number';
 }, function(box, new, old, enter)
    print(new, old, enter)
    LocalPlayer.Character.Humanoid.WalkSpeed = tonumber(new)
    print("WalkSpeed Changed")
 end)
 local b2 = w:Button('Reset WalkSpeed', function()
    LocalPlayer.Character.Humanoid.WalkSpeed = 16
    print("WalkSpeed Reset")
 end)
 local box = w:Box('JumpPower', {
    flag = "jp";
    type = 'number';
 }, function(box, new, old, enter)
    print(new, old, enter)
    LocalPlayer.Character.Humanoid.JumpPower = tonumber(new)
    print("JumpPower Changed")
 end)
 local b2 = w:Button('Reset JumpPower', function()
    LocalPlayer.Character.Humanoid.JumpPower = 50
    print("JumpPower Reset")
 end)
 local box = w:Box('HipHeight', {
    flag = "hh";
    type = 'number';
 }, function(box, new, old, enter)
    print(new, old, enter)
    LocalPlayer.Character.Humanoid.HipHeight = tonumber(new)
    print("HipHeight Changed")
 end)
 local b2 = w:Button('Reset HipHeight', function()
    LocalPlayer.Character.Humanoid.HipHeight = 2
    print("HipHeight Reset")
 end)
 local s = w:Slider("Gravity", {
    min = 0;
    max = 196.2;
    flag = 'g'
 }, function(v)
    game:GetService("Workspace").Gravity = v;
 end)
 local b2 = w:Button('Reset Gravity', function()
    game:GetService("Workspace").Gravity = 196.2
    print("Gravity Reset")
 end)
 local old = workspace.CurrentCamera.FieldOfView
local s = w:Slider("FOV", {
   min = math.floor(workspace.CurrentCamera.FieldOfView);
   max = 120;
   flag = 'fov'
}, function(v)
   workspace.CurrentCamera.FieldOfView = v;
end)
local b2 = w:Button('Reset FOV', function()
   s:Set(old)
   print("Reset")
end)
w:Section('Kill Yourself')
w:Bind("Kill Player", {
   flag = "killbind";
   kbonly = true;
   default = Enum.KeyCode.RightAlt;
}, function()
   game.Players.LocalPlayer.Character:BreakJoints()
   print("Killed Yourslef")
end)
 w:Section('Characters')
 local b = w:Button("Fox Character", function()
    CC = game:GetService("Workspace").ChangeCharacter
    CC:FireServer("FoxCharacter")
    print("Successfully Changed To Fox Character")
 end)
 local b = w:Button("Chicken Character", function()
    CC = game:GetService("Workspace").ChangeCharacter
    CC:FireServer("ChickenCharacter")
    print("Successfully Changed To Chicken Character")
 end)
 local b = w:Button("Penguin Character", function()
    CC = game:GetService("Workspace").ChangeCharacter
    CC:FireServer("PenguinCharacter")
    print("Successfully Changed To Penguin Character")
 end)
 local w = ui:CreateWindow('Teleports')
 local b = w:Button("Teleport Random Player", function()
    local randomPlayer = game.Players:GetPlayers()
[math.random(1,#game.Players:GetPlayers())]
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(Vector3.new(randomPlayer.Character.Head.Position.X, randomPlayer.Character.Head.Position.Y, randomPlayer.Character.Head.Position.Z))
print("Teleported To ???")
end)
local box = w:Box('Player', {
    flag = "p";
    type = 'string';
 }, function(box, new, old, enter)
    print(new, old, enter)
    _G.PlayerSelected = new
 end)
 local b2 = w:Button('Teleport', function()
    PlayerName = game:GetService("Players")[_G.PlayerSelected]
    LocalPlayer.Character.HumanoidRootPart.CFrame = PlayerName.Character.HumanoidRootPart.CFrame
    print("Teleported To Player")
 end)
 local b = w:Button("Teleport Tool", function()
   local plr = game:GetService("Players").LocalPlayer
local mouse = plr:GetMouse()

local tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Teleport Tool"

tool.Activated:Connect(function()
local root = plr.Character.HumanoidRootPart
local pos = mouse.Hit.Position+Vector3.new(0,2.5,0)
local offset = pos-root.Position
root.CFrame = root.CFrame+offset
end)

tool.Parent = plr.Backpack
print("Tool Received")
end)
 w:Section('Team Teleports')
 local b = w:Button("BlackZone", function()
   LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-328.943665, -9.89999294, -72.1218643, -0.000303131208, -3.68797224e-08, 0.99999994, 3.53605003e-08, 1, 3.68904445e-08, -0.99999994, 3.53716807e-08, -0.000303131208)
   print("Teleported To BlackZone")
 end)
 local b = w:Button("Really blueZone", function()
   LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(221.835587, -9.89999294, 289.496735, 3.00895917e-05, 1.89661886e-08, -1, -1.8994708e-08, 1, 1.89656184e-08, 1, 1.89941378e-08, 3.00895917e-05)
   print("Teleported To Really blueZone")
 end)
 local b = w:Button("CamoZone", function()
   LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-328.966553, -9.89999294, 285.890778, 2.32723869e-05, 4.81436508e-08, 1, -8.0430631e-08, 1, -4.81417786e-08, -1, -8.04295084e-08, 2.32723869e-05)
   print("Teleported To CamoZone")
 end)
 local b = w:Button("MagentaZone", function()
   LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(221.835083, -9.89999294, 647.695251, -2.21245518e-05, -1.27197168e-08, -1, -7.80432288e-08, 1, -1.27179902e-08, 1, 7.80429446e-08, -2.21245518e-05)
   print("Teleported To MagentaZone")
 end)
 local b = w:Button("Really redZone", function()
   LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(221.835068, -9.89999294, -68.7047195, -2.20595903e-05, -1.15739818e-08, -1, -8.31205469e-08, 1, -1.15721486e-08, 1, 8.31202911e-08, -2.20595903e-05)
   print("Teleported To Really redZone")
 end)
 local b = w:Button("WhiteZone", function()
   LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-53.5637512, -9.89999294, -345.507538, 1, 4.29280682e-08, -2.15271102e-05, -4.29279226e-08, 1, 6.71854927e-09, 2.15271102e-05, -6.71762512e-09, 1)
   print("Teleported To WhiteZone")
 end)
 local b = w:Button("New YellerZone", function()
   LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-328.942108, -9.89999294, 643.876709, -0.00115210481, -5.0259036e-08, 0.999999344, 4.44386856e-08, 1, 5.03102662e-08, -0.999999344, 4.44966162e-08, -0.00115210481)
   print("Teleported To New YellerZone")
 end)
 w:Section('TheEnd')
 local b = w:Button("WaterSand", function()
   LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-53.5905228, -360.700012, 9499.88184, 0.99999994, 5.23848342e-09, 0.000277680316, -5.23909627e-09, 1, 2.20502683e-09, -0.000277680316, -2.20648144e-09, 0.99999994)
   print("Teleported To WaterSand")
 end)
 local w = ui:CreateWindow('Miscellaneous')
 w:Section('New')
 local b = w:Button("Kill All", function()
    print("[WARNING] Only Works If Players Have Pvp Mode Enabled")
    LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-53.5655861, -360.700012, 9391.29199, 0.999978304, 8.00575783e-09, -0.00659008743, -8.00250088e-09, 1, 5.20489041e-10, 0.00659008743, -4.67740568e-10, 0.999978304)
    print("Successfully Teleported Players")
    game:GetService("RunService").Stepped:connect(function()
        for i,v in pairs (game:GetService("Players"):GetChildren()) do
            if v.TeamColor ~= LocalPlayer.TeamColor and v.Name ~= LocalPlayer.Name then
                v.Character.HumanoidRootPart.Anchored = true
                v.Character.HumanoidRootPart.CFrame = CFrame.new(-53.5905228, -360.700012, 9499.88184, 0.99999994, 5.23848342e-09, 0.000277680316, -5.23909627e-09, 1, 2.20502683e-09, -0.000277680316, -2.20648144e-09, 0.99999994)
            end
        end
    end)
end)
local b = w:Button("Big Head Player", function()
   LocalPlayerName = game:GetService("Players").LocalPlayer.Name
   LocalPlayerWorkspace = game:GetService("Workspace")[LocalPlayerName]
   LocalPlayerWorkspace.Head.Size = Vector3.new(4, 2, 2)
   print("Head Enlarged")
end)
 w:Section('Launch Teams')
 local b = w:Button("Launch BlackZone", function()
    game:GetService("Workspace").BlackZone.RE:FireServer()
    print("Launched BlackZone")
 end)
 local b = w:Button("Launch Really blueZone", function()
    game:GetService("Workspace")["Really blueZone"].RE:FireServer()
    print("Launched Really blueZone")
 end)
 local b = w:Button("Launch CamoZone", function()
    game:GetService("Workspace").CamoZone.RE:FireServer()
    print("Launched CamoZone")
 end)
 local b = w:Button("Launch MagentaZone", function()
    game:GetService("Workspace")["MagentaZone"].RE:FireServer()
    print("Launched MagentaZone")
 end)
 local b = w:Button("Launch Really redZone", function()
    game:GetService("Workspace")["Really redZone"].RE:FireServer()
    print("Launched Really redZone")
 end)
 local b = w:Button("Launch WhiteZone", function()
    game:GetService("Workspace")["WhiteZone"].RE:FireServer()
    print("Launched WhiteZone")
 end)
 local b = w:Button("Launch New YellerZone", function()
    game:GetService("Workspace")["New YellerZone"].RE:FireServer()
    print("Launched New YellerZone")
 end)
 local w = ui:CreateWindow('Fun')
 w:Section('Flings')
 local b = w:Button("Spin Fling (R6)", function()
   power = 500 -- change this to make it more or less powerful

game:GetService('RunService').Stepped:connect(function()
game.Players.LocalPlayer.Character.Head.CanCollide = false
game.Players.LocalPlayer.Character.Torso.CanCollide = false
game.Players.LocalPlayer.Character["Left Leg"].CanCollide = false
game.Players.LocalPlayer.Character["Right Leg"].CanCollide = false
end)

wait(.1)
local bambam = Instance.new("BodyThrust")
bambam.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
bambam.Force = Vector3.new(power,0,power)
bambam.Location = game.Players.LocalPlayer.Character.HumanoidRootPart.Position
print("Spin Fling (R6) Enabled")
end)
local b = w:Button("Spin Fling (R15)", function()
   power = 500 -- change this to make it more or less powerful

game:GetService('RunService').Stepped:connect(function()
game.Players.LocalPlayer.Character.Head.CanCollide = false
game.Players.LocalPlayer.Character.UpperTorso.CanCollide = false
game.Players.LocalPlayer.Character.LowerTorso.CanCollide = false
game.Players.LocalPlayer.Character.HumanoidRootPart.CanCollide = false
end)
wait(.1)
local bambam = Instance.new("BodyThrust")
bambam.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
bambam.Force = Vector3.new(power,0,power)
bambam.Location = game.Players.LocalPlayer.Character.HumanoidRootPart.Position
print("Spin Fling (R15) Enabled")
end)
local b = w:Button("Invisible Fling", function()
   


spawn(function()
   local message = Instance.new("Message",workspace)
   message.Text = "Loaded Press 'z' To Execute Invisibility , Press 'x' To Respawn)"
   wait(0.5)
   message:Destroy()
   end)
   
   
   
   
   
   
   
   
   local mouse = game.Players.LocalPlayer:GetMouse()
   
   local groot = nil
   
   mouse.KeyDown:connect(function(k)
      
      if k == "z" then
         
         
         
   spawn(function()
   local message = Instance.new("Message",workspace)
   message.Text = "Fe Invisible Fling By Loaded (Wait 11 Seconds To Load)"
   wait(11)
   message:Destroy()
   end)
   
   
   local ch = game.Players.LocalPlayer.Character
   local prt=Instance.new("Model", workspace)
   local z1 =  Instance.new("Part", prt)
   z1.Name="Torso"
   z1.CanCollide = false
   z1.Anchored = true
   local z2  =Instance.new("Part", prt)
   z2.Name="Head"
   z2.Anchored = true
   z2.CanCollide = false
   local z3 =Instance.new("Humanoid", prt)
   z3.Name="Humanoid"
   z1.Position = Vector3.new(0,9999,0)
   z2.Position = Vector3.new(0,9991,0)
    game.Players.LocalPlayer.Character=prt
   wait(5)
   game.Players.LocalPlayer.Character=ch
   wait(6)
   
   
   local plr = game.Players.LocalPlayer
   mouse = plr:GetMouse()
   
   local Hum = Instance.new("Humanoid")
   Hum.Parent = game.Players.LocalPlayer.Character
   
   
   local root =  game.Players.LocalPlayer.Character.HumanoidRootPart
   
   
   for i,v in pairs(plr.Character:GetChildren()) do
      
      if v ~= root and  v.Name ~= "Humanoid" then
         
         v:Destroy()
         
      end
      
      
   end
              
   workspace.CurrentCamera.CameraSubject = root
   
   local se = Instance.new("SelectionBox",root)
   se.Adornee = root
   
   
   game:GetService('RunService').Stepped:connect(function()
   game.Players.LocalPlayer.Character.HumanoidRootPart.CanCollide = false
   end)
   game:GetService('RunService').RenderStepped:connect(function()
   game.Players.LocalPlayer.Character.HumanoidRootPart.CanCollide = false
   end)
   
   
   power = 999999 -- change this to make it more or less powerful
   
   power = power*10
   
   ---
   wait(.1)
   local bambam = Instance.new("BodyThrust")
   bambam.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
   bambam.Force = Vector3.new(power,0,power)
   bambam.Location = game.Players.LocalPlayer.Character.HumanoidRootPart.Position 
   
   
   
   
   
   local plr = game.Players.LocalPlayer
   local torso = root
   local flying = true
   local deb = true
   local ctrl = {f = 0, b = 0, l = 0, r = 0}
   local lastctrl = {f = 0, b = 0, l = 0, r = 0}
   local maxspeed = 120
   local speed = 15
   
   
   ---local bambam = Instance.new("BodyThrust")
   ---bambam.Parent = torso
   --bambam.Force = Vector3.new(9999999,0,9999999)
   --bambam.Location = torso.Position
   
   
   ---
   groot = root
    
   function Fly()
   local bg = Instance.new("BodyGyro", torso)
   bg.P = 9e4
   bg.maxTorque = Vector3.new(0, 0, 0)
   bg.cframe = torso.CFrame
   local bv = Instance.new("BodyVelocity", torso)
   bv.velocity = Vector3.new(0,0,0)
   bv.maxForce = Vector3.new(9e9, 9e9, 9e9)
   repeat wait()
   
   if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then
   speed = speed+.2
   if speed > maxspeed then
   speed = maxspeed
   end
   elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then
   speed = speed-1
   if speed < 0 then
   speed = 0
   end
   end
   if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then
   bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
   lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r}
   elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then
   bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
   else
   bv.velocity = Vector3.new(0,0.1,0)
   end
   
   until not flying
   ctrl = {f = 0, b = 0, l = 0, r = 0}
   lastctrl = {f = 0, b = 0, l = 0, r = 0}
   speed = 0
   bg:Destroy()
   bv:Destroy()
   
   end
   mouse.KeyDown:connect(function(key)
   if key:lower() == "e" then
   if flying then flying = false
   else
   flying = true
   Fly()
   end
   elseif key:lower() == "w" then
   ctrl.f = 1
   elseif key:lower() == "s" then
   ctrl.b = -1
   elseif key:lower() == "a" then
   ctrl.l = -1
   elseif key:lower() == "d" then
   ctrl.r = 1
   end
   end)
   mouse.KeyUp:connect(function(key)
   if key:lower() == "w" then
   ctrl.f = 0
   elseif key:lower() == "s" then
   ctrl.b = 0
   elseif key:lower() == "a" then
   ctrl.l = 0
   elseif key:lower() == "d" then
   ctrl.r = 0
   elseif key:lower() == "r" then
   
   end
   end)
   Fly()
   
         
         
      elseif k == "x" then
         
         
         spawn(function()
   local message = Instance.new("Message",workspace)
   message.Text = "Respawning Don't Spam"
   wait(1)
   message:Destroy()
   end)
         
         local saved = groot.Position
         
   local ch = game.Players.LocalPlayer.Character
   local prt=Instance.new("Model", workspace)
   local z1 =  Instance.new("Part", prt)
   z1.Name="Torso"
   z1.CanCollide = false
   z1.Anchored = true
   local z2  =Instance.new("Part", prt)
   z2.Name="Head"
   z2.Anchored = true
   z2.CanCollide = false
   local z3 =Instance.new("Humanoid", prt)
   z3.Name="Humanoid"
   z1.Position = Vector3.new(0,9999,0)
   z2.Position = Vector3.new(0,9991,0)
    game.Players.LocalPlayer.Character=prt
   wait(5)
    game.Players.LocalPlayer.Character=ch
   local poop = nil
         repeat wait() poop = game.Players.LocalPlayer.Character:FindFirstChild("Head") until poop ~= nil
         wait(1)
         game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(saved)
         print("Invisible Fling Enabled")
         
      end
      
      
   end)
end)
w:Section('Fly')
w:Button("Fly (f)", function()
   repeat wait()
   until game.Players.LocalPlayer and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:findFirstChild("UpperTorso") and game.Players.LocalPlayer.Character:findFirstChild("Humanoid")
 local mouse = game.Players.LocalPlayer:GetMouse()
 repeat wait() until mouse
 local plr = game.Players.LocalPlayer
 local UpperTorso = plr.Character.UpperTorso
 local flying = true
 local deb = true
 local ctrl = {f = 0, b = 0, l = 0, r = 0}
 local lastctrl = {f = 0, b = 0, l = 0, r = 0}
 local maxspeed = 100
 local speed = 1
 
 function Fly()
 plr.Character.Humanoid.WalkSpeed = 16.5
 plr.Character.Humanoid.JumpPower = 50.5
 local bg = Instance.new("BodyGyro", UpperTorso)
 bg.P = 9e4
 bg.maxTorque = Vector3.new(9e9, 9e9, 9e9)
 bg.cframe = UpperTorso.CFrame
 local bv = Instance.new("BodyVelocity", UpperTorso)
 bv.velocity = Vector3.new(0,0.1,0)
 bv.maxForce = Vector3.new(9e9, 9e9, 9e9)
 repeat wait()
 plr.Character.Humanoid.PlatformStand = true
 if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then
 speed = speed+.5+(speed/maxspeed)
 if speed > maxspeed then
 speed = maxspeed
 end
 elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then
 speed = speed-1
 if speed < 0 then
 speed = 0
 end
 end
 if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then
 bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
 lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r}
 elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then
 bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
 else
 bv.velocity = Vector3.new(0,0.1,0)
 end
 bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0)
 until not flying
 ctrl = {f = 0, b = 0, l = 0, r = 0}
 lastctrl = {f = 0, b = 0, l = 0, r = 0}
 speed = 0
 bg:Destroy()
 bv:Destroy()
 plr.Character.Humanoid.PlatformStand = false
 end
 mouse.KeyDown:connect(function(key)
 if key:lower() == "f" then
 if flying then flying = false
 else
 flying = true
 Fly()
 end
 elseif key:lower() == "w" then
 ctrl.f = 1
 elseif key:lower() == "s" then
 ctrl.b = -1
 elseif key:lower() == "a" then
 ctrl.l = -1
 elseif key:lower() == "d" then
 ctrl.r = 1
 end
 end)
 mouse.KeyUp:connect(function(key)
 if key:lower() == "w" then
 ctrl.f = 0
 elseif key:lower() == "s" then
 ctrl.b = 0
 elseif key:lower() == "a" then
 ctrl.l = 0
 elseif key:lower() == "d" then
 ctrl.r = 0
 end
 end)
 Fly()
 print("Fly Enabled")
end)
 local b = w:Button("Destroy Gui", function()
    game:GetService("CoreGui").ScreenGui:Destroy()
    print("Gui Destroyed")
 end)
 game:GetService("Workspace").ExploitCheckRemote:Destroy()
 print("AntiCheat Deactivated")
 print("Gui Loaded")
