game.Players.LocalPlayer:GetMouse().KeyDown:Connect(function(k)
if k == "e" then
local Gun = game.ReplicatedStorage.Weapons:FindFirstChild(game.Players.LocalPlayer.NRPBS.EquippedTool.Value);
local Crit = math.random() > .6 and true or false;
for i,v in pairs(game.Players:GetPlayers()) do
if v and v.Character and v.Character:FindFirstChild("Head") then
local Distance = (game.Players.LocalPlayer.Character.Head.Position - v.Character.Head.Position).magnitude
for i  = 1,10 do
game.ReplicatedStorage.Events.HitPart:FireServer(v.Character.Head,
v.Character.Head.Position + Vector3.new(math.random(), math.random(), math.random()),
Gun.Name,
Crit and 2 or 1,
Distance,
Backstab,
Crit,
false,
1,
false,
Gun.FireRate.Value,
Gun.ReloadTime.Value,
Gun.Ammo.Value,
Gun.StoredAmmo.Value,
Gun.Bullets.Value,
Gun.EquipTime.Value,
Gun.RecoilControl.Value,
Gun.Auto.Value,
Gun['Speed%'].Value,
game.ReplicatedStorage.wkspc.DistributedTime.Value);
end
end
end
end
end)
