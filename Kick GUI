local Settings = {
    ["Name"] = "transIate",
    ["Local"] = true,
    ["Context"] = true
}
 
local GetPlayer = function()
    if Settings.Context or Settings.Local then
        return Game.Players.LocalPlayer
    else
        return Game.Players:FindFirstChild(Settings.Name) or nil
    end
end
 
local CurrentPlayer = GetPlayer()
 
 
--[[ We need someway to do this without substrings, right? ]]--
Explode = function(String)
    local List = {}
    for Item in string.gmatch(String, "%S+") do
        table.insert(List, Item)
    end
    return List
end
 
--[[ In all of my days of scripting, I feel like this is the worst recurse function I've made... ]]--
Recurse = function(Location, Type, Objects)
    if not Objects or type(Objects) ~= "table" then
        Objects = {}
    end
    for Index, Child in pairs(Location:GetChildren()) do
        if Child:IsA(Type) then
            table.insert(Objects, Child)
        end
        Recurse(Child, Type, Objects)
    end
    return Objects
end
 
--[[ But this is a pretty good players-getter ]]--
local GetPlayers = function(String)
    local List = Explode(String)
    local Players = {}
    for Index, Value in pairs(List) do
        for Index, Player in pairs(Game.Players:GetPlayers()) do
            if Value:lower() == "all" then
                table.insert(Players, Player)
            elseif Value:lower() == "others" then
                if Player ~= CurrentPlayer then
                    table.insert(Players, Player)
                end
            elseif Value:lower() == "me" then
                table.insert(Players, CurrentPlayer)
                break
            elseif Value:lower() == "guests" then
                if Player.Name:sub(1, 6) == "Guest " then
                    table.insert(Players, Player)
                end
            elseif Value:lower() == "nonguests" then
                if Player.Name:sub(1, 6) ~= "Guest " then
                    table.insert(Players, Player)
                end                        
            elseif Value:lower() == "nonbc" then
                if Player.MembershipType == Enum.MembershipType.None then
                    table.insert(Players, Player)
                end
            elseif Value:lower() == "bc" then
                if Player.MembershipType == Enum.MembershipType.BuildersClub then
                    table.insert(Players, Player)
                end
            elseif Value:lower() == "tbc" then
                if Player.MembershipType == Enum.MembershipType.TurboBuildersClub then
                    table.insert(Players, Player)
                end
            elseif Value:lower() == "obc" then
                if Player.MembershipType == Enum.MembershipType.OutrageousBuildersClub then
                    table.insert(Players, Player)
                end
            else
                if Player.Name:lower():sub(1, #Value) == Value:lower() then
                    table.insert(Players, Player)
                end
            end
        end
    end
    return Players
end
 
--[[ Commands' Functions, 1 argument only! (The textbox text) ]]--
local Commands = {
    {"Kill", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character:BreakJoints() end)
        end
    end},
    {"Heal", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.Health = v.Character.Humanoid.MaxHealth end)
        end
    end},
    {"Godmode", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.MaxHealth = math.huge end)
        end
    end},
    {"Ungodmode", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.MaxHealth = 100 end)
        end
    end},
    {"FastSpeed", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.WalkSpeed = 50 end)
        end
    end},
    {"NormalSpeed", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.WalkSpeed = 16 end)
        end
    end},
    {'DoD',function(String)
        local PlayerList=GetPlayers(String)
        for i,v in pairs(PlayerList) do
        pcall(function()
_f=function(_obj)
for x,_ in next,_obj:children''do
if(_:IsA'BasePart')then
v.Anchored=false;
v.BrickColor=BrickColor.new'Institutional white';
bv=Instance.new'BodyVelocity';
bv.Parent=v;
bv.maxForce=Vector3.new(100000000,100000000,100000000);
end;
_f(v)end end _f(workspace)
         end)
        end
    end},
    {'paper',function(String)
    local PlayerList=GetPlayers(String)
    for i,v in pairs(PlayerList)do
        pcall(function()
        for i,v in next,v.Character:children''do
if(v:IsA'BasePart')then
local b=Instance.new('SpecialMesh',v);
b.MeshType=Enum.MeshType.Brick;b.Scale=Vector3.new(1,1,.00001);
elseif(v:IsA'Hat')then  v.Handle.Mesh.Scale=Vector3.new(1,1,.005);
    elseif(v:IsA'CharacterMesh')then v:destroy''end end end)end end},
    {'dance',function(String)
        PlayerList=GetPlayers(String);
        for i,v in pairs,(PlayerList) do
            pcall(function()
            local welds={};
char=v.Character;
c=function(v)
    local r={};
    for _,d in next,v:children''do
        table.insert(r,d);
        for _,o in next,c(d)do
            table.insert(r,o);
        end;
    end;
    return r;
end;
for _,v in next,c(char)do
    if(v.className:find'Weld'or v.className:find'Motor6D')then
        table.insert(welds,v);
    end;
end;
while wait''do
    coroutine.wrap(function()
        for _,v in next,welds do
            local args={0,0,0};
            local toUse=math.random(1,3);
            local done={};
            for i=1,toUse do
                local asdf=math.random(1,3);
                repeat
                    asdf=math.random(1,3);
                until done[asdf]==nil;
                done[asdf]=true;
                args[asdf]=.075;
            end;
            v.C0=v.C0*CFrame.Angles(unpack(args));
        end;
    end)();
end;end)end end},
    {'look',function(String)
        local PlayerList=GetPlayers(String)
        for i,v in pairs,(PlayerList) do
            pcall(function()
local player=v
local mouse=player:getMouse'';
local char=player.Character;
local head=char.Head;
local torso=char.Torso;
local neck=torso.Neck;
mouse.Move:connect(function()
neck.C0=CFrame.new(0,1,0);
local headCF=torso.CFrame*CFrame.new(0,0.5,0);
local newCF=CFrame.new(headCF.p,mouse.Hit.p);
neck.C1=newCF:inverse''*torso.CFrame;
    end);end)end end},
    {"SlowSpeed", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.WalkSpeed = 5 end)
        end
    end},
    {"Mute",function(String)
        local PlayerList=GetPlayers(String)
        for i,v in pairs,(PlayerList)do
v.StarterGui:SetCoreGuiEnabled('All',false);
    end end},
    {"unMute",function(String)
        local PlayerList=GetPlayers(String)
        for i,v in pairs,(PlayerList)do
v.StarterGui:SetCoreGuiEnabled('All',true);
    end end},
    {"Stand", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.Sit = false v.Character.Humanoid.PlatformStand = false end)
        end
    end},
    {"Sit", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.Sit = true end)
        end
    end},
    {"Lie", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.PlatformStand = true end)
        end
    end},
    {"Jump", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Humanoid.Jump = true end)
        end
    end},
    {"Respawn", function(String) --[[ Not using LoadCharacter in-case it's a local script. ]]--
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            local FakeChar = Instance.new("Model", Game.Workspace)
            Instance.new("Part", FakeChar).Name = "Torso"
            Instance.new("Humanoid", FakeChar)
            pcall(function() v.Character = FakeChar end)
        end
    end},
    {"ForceField", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() Instance.new("ForceField", v.Character) end)
        end
    end},
    {"UnForceField", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() while v.Character:FindFirstChild("ForceField") do v.Character.ForceField:Destroy() end end)
        end
    end},
    {"Sparkles", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() Instance.new("Sparkles", v.Character.Torso) end)
        end
    end},
    {"Unsparkles", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() while v.Character.Torso:FindFirstChild("Sparkles") do v.Character.Torso.Sparkles:Destroy() end end)
        end
    end},
    {"Fire", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() Instance.new("Fire", v.Character.Torso) end)
        end
    end},
    {"Unfire", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() while v.Character.Torso:FindFirstChild("Fire") do v.Character.Torso.Fire:Destroy() end end)
        end
    end},
    {"Smoke", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() Instance.new("Smoke", v.Character.Torso) end)
        end
    end},
    {"Unsmoke", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() while v.Character.Torso:FindFirstChild("Smoke") do v.Character.Torso.Smoke:Destroy() end end)
        end
    end},
    {"Visible", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() local Objects = Recurse(v.Character, "BasePart") for i, v in pairs(Objects) do v.Transparency = 0 end end)
        end
    end},
    {"Invisible", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() local Objects = Recurse(v.Character, "BasePart") for i, v in pairs(Objects) do v.Transparency = 1 end end)
        end
    end},
    {"Explode", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() Instance.new("Explosion", Workspace).Position = v.Character.Torso.Position end)
        end
    end},
    {"RemoveCharacter", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character:Destroy() end)
        end
    end},
    {"TeleTo", function(String)
        local PlayerList = GetPlayers(String)
        PlayerList = PlayerList[1]
        pcall(function() CurrentPlayer.Character.Torso.CFrame = PlayerList.Character.Torso.CFrame end)
    end},
    {"TeleHere", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Character.Torso.CFrame = CurrentPlayer.Character.Torso.CFrame end)
        end
    end},
    {"Kick", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v:Destroy() end)
        end
    end},
    {"Disconnect", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.Parent = nil v.Parent = Game.Players end)
        end
    end},
    {"Gear", function(String)
        local Item = Game:GetService("InsertService"):LoadAsset(tonumber(String))
        if Item then
            for Index, Child in pairs(Item:children()) do
                if Child:IsA("Tool") or Child:IsA("HopperBin") then
                    pcall(function() Child.Parent = Game.Players.LocalPlayer.Backpack end)
                end
            end
            Item:Destroy()
        end
    end},
    {"ColorMap", function()
        local Objects = Recurse(Game.Workspace, "BasePart")
        for i, v in pairs(Objects) do
            math.randomseed(tick())
            v.Transparency = math.random()
            v.Reflectance = math.random()
            v.BrickColor = BrickColor.Random()
        end
    end},
    {"RobloxLock", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.RobloxLocked = true v.Character.RobloxLocked = true end)
        end
    end},
    {"UnRobloxLock", function(String)
        local PlayerList = GetPlayers(String)
        for i, v in pairs(PlayerList) do
            pcall(function() v.RobloxLocked = false v.Character.RobloxLocked = false end)
        end
    end},
    {"Announce", function(String)
        local PlayerList = GetPlayers("all")
        for i, v in pairs(PlayerList) do
            pcall(function() Game:GetService("Chat"):Chat(v.Character, String) end)
        end
    end},
    {"Spam", function(String)
        ypcall(function() for i = 1, 100 do Game.Players:Chat(String) Wait(0.1) end end)
    end},
}
 
local CommandAt = 1
 
--[[
Keywords (start with "$")
    All - All players.
    Others - All players excluding you.
    Me - Only you.
    Guests - All guests.
    NonGuests - All non-guests.
    NonBC - All players without any form of BC.
    BC/TBC/OBC - All players with BC/TBC/OBC.
Notes
    If the keyword doesn't exist, it will find player(s) that name start with string.
    When selecting players, you can use spaces to add more to the list.
]]--
 
--[[ The easy part, getting the command. ]]--
function GetRunnable(Text)
    for Index, Value in pairs(Commands) do
        if Value[1] == Text then
            return Value[2]
        end
    end
end
 
--[[ The harder part... ]]--
local DefaultTextBox = Instance.new("TextBox")
DefaultTextBox.BackgroundColor3 = Color3.new(0, 0, 0)
DefaultTextBox.BorderColor3 = Color3.new(1, 1, 1)
DefaultTextBox.ClearTextOnFocus = true
DefaultTextBox.Font = 2
DefaultTextBox.FontSize = 4
DefaultTextBox.TextStrokeColor3 = Color3.new(1, 1, 1)
DefaultTextBox.TextStrokeTransparency = 0
DefaultTextBox.TextXAlignment = 0
DefaultTextBox.TextYAlignment = 0
 
local DefaultTextButton = Instance.new("TextButton")
DefaultTextButton.BackgroundColor3 = Color3.new(0, 0, 0)
DefaultTextButton.BorderColor3 = Color3.new(1, 1, 1)
DefaultTextButton.Font = 2
DefaultTextButton.FontSize = 4
DefaultTextButton.TextStrokeColor3 = Color3.new(1, 1, 1)
DefaultTextButton.TextStrokeTransparency = 0
DefaultTextButton.TextXAlignment = 2
DefaultTextButton.TextYAlignment = 1
 
local DefaultTextLabel = Instance.new("TextLabel")
DefaultTextLabel.Font = 2
DefaultTextLabel.FontSize = 5
DefaultTextLabel.TextStrokeColor3 = Color3.new(1, 1, 1)
DefaultTextLabel.TextStrokeTransparency = 0
DefaultTextLabel.TextXAlignment = 2
DefaultTextLabel.TextYAlignment = 1
 
local MainGUI = Instance.new("ScreenGui")
local MainFrame = Instance.new("Frame", MainGUI)
MainFrame.Style = 3
MainFrame.Visible = false
MainFrame.Size = UDim2.new(0, 500, 0, 250)
MainFrame.Position = UDim2.new(0.5, -250, 0.5, -125)
 
local ToggleButton = DefaultTextButton:Clone()
ToggleButton.Size = UDim2.new(0, 100, 0, 25)
ToggleButton.Position = UDim2.new(0, 0, 0.5, 0)
ToggleButton.Text = "Toggle CKM SC"
ToggleButton.MouseButton1Click:connect(function()
    MainFrame.Visible = not MainFrame.Visible
end)
ToggleButton.Parent = MainGUI
 
local QuickKickTextBox = DefaultTextBox:Clone()
QuickKickTextBox.Size = UDim2.new(0, 150, 0, 25)
QuickKickTextBox.Position = UDim2.new(0, 0, 0.5, 50)
QuickKickTextBox.Text = "Quick Kick"
QuickKickTextBox.FocusLost:connect(function(Enter)
    if Enter then
        local Func = GetRunnable("Kick")
        coroutine.resume(coroutine.create(function() ypcall(function() Func(QuickKickTextBox.Text) end) end))
    end
end)
QuickKickTextBox.Parent = MainGUI
 
local Title = DefaultTextLabel:Clone()
Title.Position = UDim2.new(0.5, 0, 0, 5)
Title.Text = "Dreemz Server Control V1.1"
Title.Parent = MainFrame
 
local Keywords = DefaultTextLabel:Clone()
Keywords.Position = UDim2.new(0.5, 0, 0, 30)
Keywords.FontSize = 4
Keywords.Text = "Keywords: all, others, me, guests, nonguests, nonbc, bc, tbc, obc"
Keywords.Parent = MainFrame
 
local ScriptBox = DefaultTextBox:Clone()
ScriptBox.Size = UDim2.new(1, 0, 0, 100)
ScriptBox.Position = UDim2.new(0, 0, 0, 50)
ScriptBox.Text = "Click ENTER to execute."
ScriptBox.FocusLost:connect(function(Enter)
    if Enter then
        local Success, Error = ypcall(loadstring(ScriptBox.Text))
        if Success then
            ScriptBox.Text = "Executed Successfully"
        else
            ScriptBox.Text = Error
        end
    end
end)
ScriptBox.Parent = MainFrame
 
local PlayerLabel = DefaultTextLabel:Clone()
PlayerLabel.Position = UDim2.new(0, 25, 0, 210)
PlayerLabel.FontSize = 4
PlayerLabel.Text = "Players"
PlayerLabel.Parent = MainFrame
 
local PlayerBox = DefaultTextBox:Clone()
PlayerBox.Size = UDim2.new(0.75, 0, 0, 15)
PlayerBox.Position = UDim2.new(0, 60, 0, 205)
PlayerBox.Text = "Argument (Players or String [Depending on Command])."
PlayerBox.Parent = MainFrame
 
local CurrentCommand = DefaultTextButton:Clone()
CurrentCommand.Size = UDim2.new(0.5, 0, 0, 15)
CurrentCommand.Position = UDim2.new(0.25, 0, 0, 175)
CurrentCommand.FontSize = 4
CurrentCommand.Text = Commands[CommandAt][1]
CurrentCommand.MouseButton1Down:connect(function()
    local Func = GetRunnable(CurrentCommand.Text)
    coroutine.resume(coroutine.create(function() ypcall(function() Func(PlayerBox.Text) end) end))
end)
CurrentCommand.Parent = MainFrame
 
local PreviousCommand = DefaultTextButton:Clone()
PreviousCommand.Size = UDim2.new(0.25, 0, 0, 15)
PreviousCommand.Position = UDim2.new(0, 0, 0, 175)
PreviousCommand.Text = "<<"
PreviousCommand.MouseButton1Click:connect(function()
    if CommandAt - 1 >= 1 then
        CommandAt = CommandAt - 1
    else
        CommandAt = #Commands
    end
    CurrentCommand.Text = Commands[CommandAt][1]
end)
PreviousCommand.Parent = MainFrame
 
local NextCommand = DefaultTextButton:Clone()
NextCommand.Size = UDim2.new(0.25, 0, 0, 15)
NextCommand.Position = UDim2.new(0.75, 0, 0, 175)
NextCommand.Text = ">>"
NextCommand.MouseButton1Click:connect(function()
    if CommandAt + 1 <= #Commands then
        CommandAt = CommandAt + 1
    else
        CommandAt = 1
    end
    CurrentCommand.Text = Commands[CommandAt][1]
end)
NextCommand.Parent = MainFrame
 
 
MainGUI.Parent = Settings.Context and Game.CoreGui or CurrentPlayer.PlayerGui
