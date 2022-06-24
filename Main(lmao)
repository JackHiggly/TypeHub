_G.AccentColors = {
    Accent1 = Color3.fromRGB(24, 117, 255),
    Accent2 = Color3.fromRGB(18, 92, 202)
}

local Framework = loadstring(game:HttpGet("https://pastebinp.com/raw/KP1dUHFg"))()
local CoolDowns = { AutoPickUps = { MoneyCooldown = false, ScrapCooldown = false, ToolCooldown = false } }
local ESPSettings = { PlayerESP = { Enabled = false, TracersOn = false, BoxesOn = false, NamesOn = false, DistanceOn = false, HealthOn = false, ToolOn = false, FaceCamOn = false, Distance = 2000 }, ScrapESP = { Enabled = false, Distance = 2000, LegendaryOnly = true, RareOnly = true, GoodOnly = true, BadOnly = true }, SafeESP = { Enabled = false, Distance = 2000, BigOnly = true, SmallOnly = true }, RegisterESP = { Enabled = false, Distance = 2000 }, ESPColor = Color3.fromRGB(255, 255, 255), ToolColor = Color3.fromRGB(255, 255, 255)};
local ESPFramework = loadstring(game:HttpGet("https://raw.githubusercontent.com/DOXSASHW/ewewew/main/esp", true))()
local Settings  = { GunMods = { NoRecoil = false, InstantEquip = false, Burst = false, Spread = false, AutoMode = false, SpreadAmount = 0 }, DownedChat = false, KillChat = false, DownedMSG = "IM A FEMALE", KillMSG = "", IsDead = false, AutoPickCash = false, AutoPickTools = false, AutoPickScrap = false, InfiniteStamina = false, NoJumpCooldown = false, SpaceJump = false, NoFailLockpick = false, ShowChatLogs = false, NoFlashbang  = false, NoSmoke = false, UnlockDoorsNearby = false, OpenDoorsNearby = false, NoClip = false, FullBright = false, CamFovToggled = false, CamFov = 70, Zoom = 10, InfinitePepperSpray = false, PepperSprayAura = false, WalkSpeed = {Enabled = false, Amount = 30}, JumpPower = {Enabled = false, Amount = 75}, NoBarbwire = false, NoFallDamage = false, NoRagdoll = false, WatermarkOn = false, ViewModel = { Enabled = false, Viewmodel = { Color = Color3.fromRGB(255, 255, 255), Material = Enum.Material.ForceField }, Melees = { Color = Color3.fromRGB(255, 255, 255), Material = Enum.Material.ForceField }, Guns = { Color = Color3.fromRGB(255, 255, 255), Material = Enum.Material.Plastic }, LeftArmOff = false }, CustomHitSound = 5043539486, VolumeHitsound = 1, WallBang = false, ElevatorTP = false, TowerTP = false, UIKey = Enum.KeyCode.LeftAlt};
local Watermark = Framework:CreateWatermark("TypeHub | {game} | {fps}")
local WriteLine = Framework:CreateWindow("TypeHub | 1.0.1", Vector2.new(492, 588), Enum.KeyCode.RightControl)
loadstring(game:HttpGet("https://raw.githubusercontent.com/NougatBitz/BitzUtils/main/CriminalityFeatures.lua"))()



local game                              = game;
local GetService                        = game.GetService;

local Workspace                         = GetService(game, "Workspace");
local Players                           = GetService(game, "Players");
local ReplicatedStorage                 = GetService(game, "ReplicatedStorage");
local StarterGui                        = GetService(game, "StarterGui");

local LogService                        = GetService(game, "LogService");
local HttpService                       = GetService(game, "HttpService");
local ScriptContext                     = GetService(game, "ScriptContext");

local Player                            = Players.LocalPlayer;
local Character                         = Player.Character;
local Mouse                             = Player:GetMouse()
local Cam                               = workspace.CurrentCamera;


game:GetService("RunService").RenderStepped:Connect(function()
    if Settings.IsDead == false then
        if Player.Character:FindFirstChild("Pepper-spray") then
            if Settings.InfinitePepperSpray == true then
                game.Players.LocalPlayer.Character["Pepper-spray"].Ammo.Value = 99
                game.Players.LocalPlayer.Character["Pepper-spray"].RemoteEvent:FireServer("Update", 99)
            end
        end
    end
end)

game:GetService("RunService").RenderStepped:Connect(function()
    if Settings.IsDead == false then
        if Settings.WalkSpeed.Enabled == true then
            Player.Character:FindFirstChild("Humanoid").WalkSpeed = Settings.WalkSpeed.Amount
        end

        if Settings.JumpPower.Enabled == true then
            Player.Character:FindFirstChild("Humanoid").JumpPower = Settings.JumpPower.Amount
        end
    end
end)

game:GetService("RunService").RenderStepped:Connect(function()
if Settings.CamFovToggled == true then
game.Workspace.Camera.FieldOfView = Settings.CamFov
end
end)


for i, v in pairs(game:GetService("ReplicatedStorage").Storage.HitStuff.Main:GetDescendants()) do
if v:IsA("Sound") then
    v.Volume = Settings.VolumeHitsound
end
end


game.Players.PlayerAdded:Connect(function(AdminUserCheck)
if AdminUserCheck.UserId == 68246168 or AdminUserCheck.UserId == 955294 or AdminUserCheck.UserId == 1095419 or AdminUserCheck.UserId == 50585425 or AdminUserCheck.UserId == 48405917 or AdminUserCheck.UserId == 9212846 or AdminUserCheck.UserId == 47352513 or AdminUserCheck.UserId == 48058122 then
    StarterGui:SetCore("SendNotification", {Title = "run"; Text = "Mod Alert\n"..AdminUserCheck.Name..", Is in the server."; Duration = 10 })
elseif AdminUserCheck.UserId == 42066711 or AdminUserCheck.UserId == 513615792 then
    StarterGui:SetCore("SendNotification", {Title = "run"; Text = "Contractors Alert\n"..AdminUserCheck.Name..", Is in the server"; Duration = 10 })
elseif AdminUserCheck.UserId == 151691292 or AdminUserCheck.UserId == 92504899 or AdminUserCheck.UserId == 31967243 then
    StarterGui:SetCore("SendNotification", {Title = "run"; Text = "Devs Alert\n"..AdminUserCheck.Name..", Is in the server."; Duration = 10 })
elseif AdminUserCheck.UserId == 29761878 then
    StarterGui:SetCore("SendNotification", {Title = "run"; Text = "Owner Alert\nRvvz, Is in the server."; Duration = 10 })
end
end)

for i, v in pairs(game.Players:GetPlayers()) do
if v.UserId == 68246168 or v.UserId == 955294 or v.UserId == 1095419 or v.UserId == 50585425 or v.UserId == 48405917 or v.UserId == 9212846 or v.UserId == 47352513 or v.UserId == 48058122 then
    StarterGui:SetCore("SendNotification", {Title = "run"; Text = "Mod Alert\n"..v.Name..", Is in the server."; Duration = 10 })
elseif v.UserId == 42066711 or v.UserId == 513615792 then
    StarterGui:SetCore("SendNotification", {Title = "run"; Text = "Contractors Alert\n"..v.Name..", Is in the server"; Duration = 10 })
elseif v.UserId == 151691292 or v.UserId == 92504899 or v.UserId == 31967243 then
    StarterGui:SetCore("SendNotification", {Title = "run"; Text = "Devs Alert\n"..v.Name..", Is in the server."; Duration = 10 })
elseif v.UserId == 29761878 then
    StarterGui:SetCore("SendNotification", {Title = "leave boy"; Text = "Owner Alert\nRvvz, Is in the server."; Duration = 10 })
end
end



local oldStamina
oldStamina =
hookfunction(
    getupvalue(getrenv()._G.S_Take, 2),
    function(v1, ...)
        if (Settings.InfiniteStamina) then 
        v1 = 0
    end
        return oldStamina(v1, ...)
    end
)

local General = WriteLine:CreateTab("Main")
local Setting = WriteLine:CreateTab("Settings")


local __newindex
__newindex = hookmetamethod(game, "__newindex", function(t, k, v)
if (t:IsDescendantOf(Character) and k == "Jump" and v == false) then
    if Settings.NoJumpCooldown == true then
        return
    end
end

return __newindex(t, k, v)
end)

local Player = game.Players.LocalPlayer
Player.Character.ChildAdded:Connect(function(Item)
if Item:IsA("Tool") then
    for i,v in pairs(getgc(true)) do 
        if type(v) == 'table' and rawget(v, 'EquipTime') then 
            if Settings.GunMods.NoRecoil == true then
                v.Recoil = 0
                v.CameraRecoilingEnabled = false
                v.AngleX_Min = 0 
                v.AngleX_Max = 0 
                v.AngleY_Min = 0
                v.AngleY_Max = 0
                v.AngleZ_Min = 0
                v.AngleZ_Max = 0
            end

            if Settings.GunMods.InstantEquip == true then
                v.EquipTime = 0
            end

            if Settings.GunMods.Spread == true then
                v.Spread = Settings.GunMods.SpreadAmount
            end

            if Settings.GunMods.AutoMode == true then
                v.FireModeSettings = {FireMode = "Semi", BurstAmount = 6, BurstRate = 25, CanSwitch = true, SwitchTo = "Auto"}
            end
        end
    end
end
end)


game:GetService("RunService").RenderStepped:Connect(function()
if Settings.UnlockDoorsNearby == true then
    if Settings.IsDead == false then
        for i, v in pairs(game:GetService("Workspace").Map.Doors:GetChildren()) do
            if (game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart").Position - v:FindFirstChild("DoorBase").Position).Magnitude <= 5 then
                if v:FindFirstChild("Values"):FindFirstChild("Locked").Value == true then
                    v:FindFirstChild("Events"):FindFirstChild("Toggle"):FireServer("Unlock", v.Lock)
                end
            end
        end
    end
end

if Settings.OpenDoorsNearby == true then
    if Settings.IsDead == false then
        for i, v in pairs(game:GetService("Workspace").Map.Doors:GetChildren()) do
            if (game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart").Position - v:FindFirstChild("DoorBase").Position).Magnitude <= 5 then
                if v:FindFirstChild("Values"):FindFirstChild("Open").Value == false then
                    v:FindFirstChild("Events"):FindFirstChild("Toggle"):FireServer("Open", v.Knob2)
                end
            end
        end
    end
end
end)



coroutine.wrap(function()
    game:GetService("RunService").RenderStepped:Connect(function()
        if Settings.IsDead == false then
            if game.Workspace.Camera:FindFirstChild("ViewModel") then
                if Settings.ViewModel.Enabled == true then
                    game.Workspace.Camera.ViewModel["Left Arm"].Color = Settings.ViewModel.Viewmodel.Color
                    game.Workspace.Camera.ViewModel["Right Arm"].Color = Settings.ViewModel.Viewmodel.Color 

                    game.Workspace.Camera.ViewModel["Right Arm"].Material = Settings.ViewModel.Viewmodel.Material
                    game.Workspace.Camera.ViewModel["Left Arm"].Material = Settings.ViewModel.Viewmodel.Material

                    if Settings.ViewModel.LeftArmOff == true then
                        game.Workspace.Camera.ViewModel["Left Arm"].Transparency = 1
                    end

                    if game.Workspace.Camera.ViewModel:FindFirstChild("Tool") then
                        for i,v in pairs(game.Workspace.Camera.ViewModel.Tool:GetDescendants()) do
                            if v.Name == "SurfaceAppearance" then
                                v:Destroy()
                            end
                        end
                    end

                    if game.Workspace.Camera.ViewModel:FindFirstChild("Tool") then
                        if game.Workspace.Camera.ViewModel.Tool.Handle:FindFirstChild("Trail") then
                            for i, v in pairs(game.Workspace.Camera.ViewModel.Tool:GetDescendants()) do
                                if v:IsA("Mesh") or v:IsA("BasePart") or v:IsA("UnionOperation") then
                                    v.Color = Settings.ViewModel.Melees.Color
                                    v.Material = Settings.ViewModel.Melees.Material
                                end
                            end
                        else
                            for i, v in pairs(game.Workspace.Camera.ViewModel.Tool:GetDescendants()) do
                                if v:IsA("Mesh") or v:IsA("BasePart") or v:IsA("UnionOperation") then
                                    v.Color = Settings.ViewModel.Guns.Color
                                    v.Material = Settings.ViewModel.Guns.Material
                                end
                            end
                        end
                    end
                end
            end
        end
    end)
end)()

-->> AutoPickup
coroutine.wrap(function()
game:GetService("RunService").RenderStepped:Connect(function()

    if Settings.CamFovToggled == true then
        game.Workspace.Camera.FieldOfView = Settings.CamFov
    end

    if Settings.AutoPickScrap == true then
        for i, v in pairs(game:GetService("Workspace").Filter.SpawnedPiles:GetChildren()) do
            if Settings.IsDead == false then
                if (game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart").Position - v:FindFirstChild("MeshPart").Position).Magnitude < 5 then
                    if CoolDowns.AutoPickUps.ScrapCooldown == false then
                        CoolDowns.AutoPickUps.ScrapCooldown = true
                        game:GetService("ReplicatedStorage").Events.PIC_PU:FireServer(string.reverse(v:GetAttribute("zp")))

                        wait(1)

                        CoolDowns.AutoPickUps.ScrapCooldown = false
                    end
                end
            end 
        end
    end
end)
end)()

coroutine.wrap(function()
game:GetService("RunService").RenderStepped:Connect(function()
    if Settings.AutoPickTools == true then
        for i, v in pairs(game:GetService("Workspace").Filter.SpawnedTools:GetChildren()) do
            if Settings.IsDead == false then
                if (game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart").Position - v:FindFirstChildWhichIsA("MeshPart").Position).Magnitude < 5 then
                    if CoolDowns.AutoPickUps.ToolCooldown == false then
                        CoolDowns.AutoPickUps.ToolCooldown = true
                        game:GetService("ReplicatedStorage").Events.PIC_TLO:FireServer(v:FindFirstChildWhichIsA("MeshPart"))

                        wait(1)

                        CoolDowns.AutoPickUps.ToolCooldown = false
                    end
                end
            end
        end
    end
end)
end)()

coroutine.wrap(function()
game:GetService("RunService").RenderStepped:Connect(function()
    if Settings.AutoPickCash == true then
        for i, v in pairs(game:GetService("Workspace").Filter.SpawnedBread:GetChildren()) do
            if Settings.IsDead == false then
                if (game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart").Position - v.Position).Magnitude < 5 then
                    if CoolDowns.AutoPickUps.MoneyCooldown == false then
                        CoolDowns.AutoPickUps.MoneyCooldown = true
                        game:GetService("ReplicatedStorage").Events.CZDPZUS:FireServer(v)

                        wait(1)

                        CoolDowns.AutoPickUps.MoneyCooldown = false
                    end
                end
            end
        end
    end
end)
end)()
-->> End auto pickup

-->> Start Notification
function Notify(msg)
local l__ReplicatedStorage__1 = game:GetService("ReplicatedStorage");
l__ReplicatedStorage__1.Events2.Notification:Fire({
    Title = "ELITE", 
    Text = tostring(msg), 
    Duration = 5
}, "lost");
end

Notify("Loaded!")

-->> End Noti

-->> Important
game:GetService("RunService").RenderStepped:Connect(function()
for _, Connection in next, getconnections(game:GetService("ScriptContext").Error) do
    Connection:Disable()
end

for _, Connection in next, getconnections(game:GetService("LogService").MessageOut) do
    Connection:Disable()
end
end)


for i,v in pairs(getgc(true)) do
if typeof(v) == 'table' and rawget(v, 'A') then
v.A = function()
    
end
end
if typeof(v) == 'table' and rawget(v, 'B') then
v.B = function()
    
end
end
end
-->> End Important


-->> Anti stuff
local oldNamecall
    oldNamecall =
        hookmetamethod(
            game,
            "__namecall",
            newcclosure(
                function(...)
                    if (not checkcaller() and getnamecallmethod() == "FireServer" and Settings.NoFallDamage) then
                    local tab = ...
                    if (tostring(tab) == "__DFfDD") then
                        return wait(9e9)
                    end
                elseif (not checkcaller() and getnamecallmethod() == "FireServer" and Settings.NoBarbwire) then
                    local tab = ...
                    if (tostring(tab) == "BHHh") then
                        return wait(9e9)
                    end
                elseif (not checkcaller() and getnamecallmethod() == "FireServer" and Settings.NoRagdoll) then
                    local tab = ...
                    if (tostring(tab) == "__--r") then
                        return wait(9e9)
                    end
                end

                    return oldNamecall(...)
                end
            )
        )
-->> End anti stuff

-->> Noclip Bypass
local statetype = Enum.HumanoidStateType
local rnd = Random.new():NextInteger(150, 100000)
local mt = getrawmetatable(statetype)
local mt_index = mt.__index
setreadonly(mt, false)

mt.__index = newcclosure(function(t, k)
if not checkcaller() and t == statetype and k == "StrafingNoPhysics"  then
return rnd
end

return mt_index(t, k)
end)

setreadonly(mt, true)

    game:GetService("RunService").RenderStepped:Connect(function()
        for _, Connection in next, getconnections(game:GetService("ScriptContext").Error) do
            Connection:Disable()
        end

        for _, Connection in next, getconnections(game:GetService("LogService").MessageOut) do
            Connection:Disable()
        end
    end)
-->> End Noclip Bypass

local Main = General:CreateSector("Player", "left")
local Main2 = General:CreateSector("Combat", "right")
local Main3 = General:CreateSector("Misc", "left")
local Main4 = General:CreateSector("Visuals", "right")
local Main6 = Setting:CreateSector("Settings", "Left") 
local Main7 = Setting:CreateSector("Advanced", "Left") 
local Main10 = Setting:CreateSector("Panic", "right") 
Main:AddSeperator("Blatant")

local WALKSPEED = Main:AddToggle("WalkSpeed", Settings.WalkSpeed.Enabled, function(V)
    Settings.WalkSpeed.Enabled = V
end)

WALKSPEED:AddKeybind("None", "UserIToggle")


local JUMPPOWER = Main:AddToggle("JumpPower", Settings.JumpPower.Enabled, function(V)
    Settings.JumpPower.Enabled = V
end)

JUMPPOWER:AddKeybind("None", "UserIToggle")

Main:AddSlider("WalkSpeed", 16, Settings.WalkSpeed.Amount, 30, 10, function(V)
    Settings.WalkSpeed.Amount = V
end)

Main:AddSlider("JumpPower", 50, Settings.JumpPower.Amount, 75, 10, function(V)
    Settings.JumpPower.Amount = V
end)
Main:AddSeperator("Extra")

Main:AddSlider("Tp Speed", 5, 5, 100, 1, function(v)
    _G.TPSPEED = v
end)

Main:AddButton("Ctrl + Click to tp", function()
    function Notify(msg)
        local l__ReplicatedStorage__1 = game:GetService("ReplicatedStorage");
        l__ReplicatedStorage__1.Events2.Notification:Fire({
            Title = "ELITE", 
            Text = tostring(msg), 
            Duration = 5
        }, "lost");
        end
        
        Notify("Not Far.")
    local speed = (_G.TPSPEED) -- set this lower to make it slower
    local bodyvelocityenabled = true -- set this to false if you are getting kicked
    
    local Imput = game:GetService("UserInputService")
    local Plr = game.Players.LocalPlayer
    local Mouse = Plr:GetMouse()
    
    function To(position)
    local Chr = Plr.Character
    if Chr ~= nil then
    local ts = game:GetService("TweenService")
    local char = game.Players.LocalPlayer.Character
    local hm = char.HumanoidRootPart
    local dist = (hm.Position - Mouse.Hit.p).magnitude
    local tweenspeed = dist/tonumber(speed)
    local ti = TweenInfo.new(tonumber(tweenspeed), Enum.EasingStyle.Linear)
    local tp = {CFrame = CFrame.new(position)}
    ts:Create(hm, ti, tp):Play()
    if bodyvelocityenabled == true then
    local bv = Instance.new("BodyVelocity")
    bv.Parent = hm
    bv.MaxForce = Vector3.new(100000,100000,100000)
    bv.Velocity = Vector3.new(0,0,0)
    wait(tonumber(tweenspeed))
    bv:Destroy()
    end
    end
    end
    
    Imput.InputBegan:Connect(function(input)
       if input.UserInputType == Enum.UserInputType.MouseButton1 and Imput:IsKeyDown(Enum.KeyCode.LeftControl) then
           To(Mouse.Hit.p)
       end
    end)
end)

Main:AddButton("[❗] Float [Q & E]", function()
bruh = Instance.new('Part', game.Workspace)
bruh.Name = "bruh"
bruh.Size = Vector3.new(6,.1,6)
bruh.Color = Color3.fromRGB(100,166,200)
bruh.Anchored = true
bruh.Transparency = 1 --set to whatever lol
loop = false
a = game.Players.LocalPlayer:GetMouse()
a.KeyDown:Connect(function(black)
if black == "q" then
   loop = true
   while loop do
       wait()
bruh.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame + Vector3.new(0,-3.05,0)
end
elseif black == "e" and loop == true then
loop = false
end
end)
end)

Main:AddToggle("No Jump Cooldown", Settings.NoJumpCooldown,function(v)
Settings.NoJumpCooldown = v
end)

Main:AddSeperator("Infinite")


Main:AddToggle("Infinite Jump", false,function(v)
if v == true then
    local Player = game:GetService'Players'.LocalPlayer;
local UIS = game:GetService'UserInputService';
 
_G.JumpHeight = 50;
 
function Action(Object, Function) if Object ~= nil then Function(Object); end end
 
UIS.InputBegan:connect(function(UserInput)
    if UserInput.UserInputType == Enum.UserInputType.Keyboard and UserInput.KeyCode == Enum.KeyCode.Space then
        Action(Player.Character.Humanoid, function(self)
            if self:GetState() == Enum.HumanoidStateType.Jumping or self:GetState() == Enum.HumanoidStateType.Freefall then
                Action(self.Parent.HumanoidRootPart, function(self)
                    self.Velocity = Vector3.new(0, _G.JumpHeight, 0);
                end)
            end
        end)
    end
end)
end
  if v == false then
    local Player = game:GetService'Players'.LocalPlayer;
local UIS = game:GetService'UserInputService';
 
_G.JumpHeight = 0;
 
function Action(Object, Function) if Object ~= nil then Function(Object); end end
 
UIS.InputBegan:connect(function(UserInput)
    if UserInput.UserInputType == Enum.UserInputType.Keyboard and UserInput.KeyCode == Enum.KeyCode.Space then
        Action(Player.Character.Humanoid, function(self)
            if self:GetState() == Enum.HumanoidStateType.Jumping or self:GetState() == Enum.HumanoidStateType.Freefall then
                Action(self.Parent.HumanoidRootPart, function(self)
                    self.Velocity = Vector3.new(0, _G.JumpHeight, 0);
                end)
            end
        end)
    end
end)
end
end)

local INFSTAMINA = Main:AddToggle("Infinite Stamina", Settings.InfiniteStamina, function(V)
Settings.InfiniteStamina = V
end)
INFSTAMINA:AddKeybind("None", "UserIToggle")

Main:AddSeperator("Noclip")

Main:AddToggle("Noclip", false, function(v)
_G.Noclip = v
        
local function Noclip()
if game.Players.LocalPlayer.Character ~= nil and _G.Noclip == true then
for _, selfChar in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
    if selfChar:IsA("BasePart") and selfChar.CanCollide == true and selfChar.Name then
            selfChar.CanCollide = false
        end
    end
end
end

game:GetService('RunService').Stepped:Connect(Noclip)
end)

Main:AddToggle("Noclip doors", false, function(v)
_G.Noclipdoor = v
    
if  _G.Noclipdoor == true then
    for _, v in pairs(game:GetService("Workspace").Map.Doors:GetChildren()) do
        if v:FindFirstChild("DoorBase") then
            v.DoorBase.CanCollide = false
        end
        if v:FindFirstChild("DoorA") then
            v.DoorA.CanCollide = false
        end
        if v:FindFirstChild("DoorB") then
            v.DoorB.CanCollide = false
        end
        if v:FindFirstChild("DoorC") then
            v.DoorC.CanCollide = false
        end
        if v:FindFirstChild("DoorD") then
            v.DoorD.CanCollide = false
        end
    end
else
    for _, v in pairs(game:GetService("Workspace").Map.Doors:GetChildren()) do
        if v:FindFirstChild("DoorBase") then
            v.DoorBase.CanCollide = true
        end
        if v:FindFirstChild("DoorA") then
            v.DoorA.CanCollide = true
        end
        if v:FindFirstChild("DoorB") then
            v.DoorB.CanCollide = true
        end
        if v:FindFirstChild("DoorC") then
            v.DoorC.CanCollide = true
        end
        if v:FindFirstChild("DoorD") then
            v.DoorD.CanCollide = true
        end
    end
end
end)



Main:AddSeperator("Anti Mods")

Main:AddToggle("Disable Barbwire", Settings.NoBarbwire, function(V)
Settings.NoBarbwire = V
end)

Main:AddToggle("Disable Fall Damage", Settings.NoFallDamage, function(V)
Settings.NoFallDamage = V
end)

Main:AddToggle("Disable Ragdoll", Settings.NoRagdoll, function(V)
Settings.NoRagdoll = V
end)

Main:AddToggle("Anti Flash Bang", false, function(v)
_G.NoFlashBang = v
game.Workspace.Camera.ChildAdded:Connect(function(Item)
    if _G.NoFlashBang == true then
        if Item.Name == "BlindEffect" then
            Item.Enabled = false
        end
    end
end)

game.Players.LocalPlayer.PlayerGui.ChildAdded:Connect(function(Item)
    if Item.Name == "FlashedGUI" then
        if _G.NoFlashBang == true then
            Item.Enabled = false
        end
    end
end)
end)


Main:AddToggle("Anti Smoke", false, function(v)
_G.NoSmoke = v
game.Workspace.Debris.ChildAdded:Connect(function(Item)
    if Item.Name == "SmokeExplosion" then
        if _G.NoSmoke == true then
            wait(0.1)
            Item.Particle1:Destroy()
            Item.Particle2:Destroy()
        end
    end
end)

game.Players.LocalPlayer.PlayerGui.ChildAdded:Connect(function(Item)
    if Item.Name == "SmokeScreenGUI" then
        if _G.NoSmoke == true then
            Item.Enabled = false
        end
    end
end)
end)

Main:AddToggle("Anti Kick", false, function(v)
print('!&%^')
function Notify(msg)
    local l__ReplicatedStorage__1 = game:GetService("ReplicatedStorage");
    l__ReplicatedStorage__1.Events2.Notification:Fire({
        Title = "Elite", 
        Text = tostring(msg), 
        Duration = 5
    }, "lost");
    end
    
    Notify("Anti Kick Region : !&%^")
end)

Main:AddSeperator("God")
Main:AddButton("Bruh Breathing sounds", function()
    local breathing = game.Workspace.Characters[game.Players.LocalPlayer.Name].Head.BreathingLoop
    breathing.PlaybackSpeed = 1
    breathing.SoundId = "rbxassetid://5646824941"
end)
Main:AddToggle("Walk on water", false, function(v)
    Callback = function(Value)
        if v == false then 
            for _,v in pairs(game.Workspace.Filter.WaterCurrents:GetChildren()) do 
                v.CanCollide = false
            end
        end
        if v == true then
            for _,v in pairs(game.Workspace.Filter.WaterCurrents:GetChildren()) do 
            v.CanCollide = true
        end
    end
end
end)

Main:AddToggle("Reveal fake displays", false, function(v)
    Callback = function(v)
        if v == true then
            wait()
            lp.PlayerGui.CurrentGUI.MFrame.DisplayNameLabel.Text = "Bruh"
            lp.PlayerGui.CurrentGUI.MFrame.DisplayNameLabel.TextColor3 = Color3.fromRGB(255,0,0)
            lp.DisplayName = "BruhSoundEffect"
        elseif v == false then
            lp.PlayerGui.CurrentGUI.MFrame.DisplayNameLabel.Text = realdisplayname
            lp.PlayerGui.CurrentGUI.MFrame.DisplayNameLabel.TextColor3 = Color3.fromRGB(255,255,255)
            lp.DisplayName = realdisplayname
        end
    end
end)
    



Main:AddSeperator("Misc")

Main:AddButton("V - Prints Cframe of mouse", function()
    local UIS = game:GetService("UserInputService")
    plr = game.Players.LocalPlayer
    mouse = plr:GetMouse()
    
    UIS.InputBegan:Connect(function(F)
    if F.KeyCode == Enum.KeyCode.V then
       print(mouse.Hit.p)
    end
    end)
end)

Main:AddButton("Remove Textures", function()
for _,v in pairs(workspace:GetDescendants()) do
    if v.ClassName == "Part" or v.ClassName == "SpawnLocation" or v.ClassName == "WedgePart" or v.ClassName == "Terrain" or v.ClassName == "MeshPart" then
        v.Material = "Plastic"
    end
end

for i, v in pairs(workspace:GetDescendants()) do
    if v.ClassName == "Decal" or v.ClassName == "Texture" then
        v:Destroy()
    end
end
end)



local TOGGLEFOV = Main:AddToggle("Toggle FOV", Settings.CamFovToggled, function(v)
Settings.CamFovToggled = v
end, "FOVToggle")
TOGGLEFOV:AddKeybind("None", "UserIToggle")

Main:AddSlider("FOV", 5, 5, 120, 1, function(v)
Settings.CamFov = v
end)

Main:AddToggle("Full Bright", false, function(v)
if v == true then
    game:GetService("Lighting").ExposureCompensation = 2.7
elseif v == false then
    game:GetService("Lighting").ExposureCompensation = 0
end  
end)

Main:AddColorpicker("Ambient Color", Color3.new(1, 1, 1), function(v)
game:GetService("Lighting").OutdoorAmbient = v
end) 

Main:AddSlider("Max Zoom", 5, 5, 1000, 1, function(v)
game.Players.LocalPlayer.CameraMaxZoomDistance = v
end)

Main:AddButton("Noclip Fly [T]", function()
function Notify(msg)
    local l__ReplicatedStorage__1 = game:GetService("ReplicatedStorage");
    l__ReplicatedStorage__1.Events2.Notification:Fire({
        Title = "Elite", 
        Text = tostring(msg), 
        Duration = 5
    }, "lost");
    end
    
    Notify("Not to far!")
game.Players.LocalPlayer.DevCameraOcclusionMode = 'Invisicam' 
local mouse = game.Players.LocalPlayer:GetMouse()
local torso = game.Players.LocalPlayer.Character.Torso
local dir = {w = 0, s = 0, a = 0, d = 0}
local spd = 2 mouse.KeyDown:connect(function(key)
if key:lower() == "w" then dir.w = 1
elseif key:lower() == "s" then dir.s = 1
elseif key:lower() == "a" then dir.a = 1
elseif key:lower() == "d" then dir.d = 1
elseif key:lower() == "q" then spd = spd + 1
elseif key:lower() == "e" then spd = spd - 1
end 
end)
mouse.KeyUp:connect(function(key)
if key:lower() == "w" then
dir.w = 0
elseif key:lower() == "s" then dir.s = 0
elseif key:lower() == "a" then dir.a = 0
elseif key:lower() == "d" then dir.d = 0
end 
end)


enabled = false
mouse.keyDown:connect(function(key)
if (key) == "t" and enabled == false then
  enabled = true
  repeat wait(1/44)
     game.Players.LocalPlayer.Character.Torso.Anchored = true
     game.Players.LocalPlayer.Character.Humanoid.PlatformStand = true
     torso.CFrame = CFrame.new(torso.Position, game.Workspace.CurrentCamera.CoordinateFrame.p) * CFrame.Angles(0,math.rad(180),0) * CFrame.new((dir.d-dir.a)*spd,0,(dir.s-dir.w)*spd)
  until enabled == false
elseif enabled == false then
  game.Players.LocalPlayer.Character.Humanoid.PlatformStand = false
  game.Players.LocalPlayer.Character.Torso.Anchored = false
end
if (key) == "t" and enabled == true then
  enabled = false
  game.Players.LocalPlayer.Character.Humanoid.PlatformStand = false
  game.Players.LocalPlayer.Character.Torso.Anchored = false


end

end)       
end)

Main:AddSeperator("Hat Things")

Main:AddTextbox("Distance", "0", function(V)
    _G.HAT = V
end)

Main:AddButton("Spin Hats", function()
    _G.Distance = (HAT)
for i,v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
    if v.Name == "AccessoryWeld" then
        v:Destroy()
    end
end
for i,v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
    if v:IsA("Part") and v.Name == "Handle" and v.Parent:IsA("Accessory") then
        wait(0.04)
        local Part = Instance.new("Part") 
        Part.Parent = workspace
        Part.Size = Vector3.new(5,5,5)
        Part.Transparency = 1
        Part.CanCollide = false 
        Part.Position = v.Position
        Part.Anchored = true
        Part.CanTouch = false
        Part.Name = "CenterOfGravitationalForce"
        local Att1 = Instance.new("Attachment")
        Att1.Name = "Att1"
        Att1.Visible = false 
        Att1.Parent = v
        
        local Att2 = Instance.new("Attachment")
        Att2.Name = "Att2"
        Att2.Visible = false 
        Att2.Parent = Part
        Att2.Position = Vector3.new(0.1, -0.8, -1.5)
        
        local AlignPos = Instance.new("AlignPosition")
        local AlignGyro = Instance.new("AlignOrientation")
        
        AlignPos.Parent = v
        AlignPos.Attachment0 = Att1
        AlignPos.MaxForce = math.huge
        AlignPos.MaxVelocity = math.huge
        AlignPos.Mode = Enum.PositionAlignmentMode.TwoAttachment
        AlignPos.Attachment1 = Att2
        AlignPos.RigidityEnabled = false 
        
        AlignGyro.Parent = v
        AlignGyro.Mode = Enum.OrientationAlignmentMode.OneAttachment
        AlignGyro.CFrame = workspace.CurrentCamera.CFrame
        AlignGyro.MaxTorque = math.huge
        AlignGyro.Attachment0 = Att1
        AlignGyro.RigidityEnabled = false
        antifall = Instance.new("BodyVelocity", v)
        antifall.Velocity = Vector3.new(0,0,0)
        local tp = game:GetService("RunService").Heartbeat:Connect(function()
            AlignGyro.CFrame = AlignGyro.CFrame
        end)
        Part.Anchored = true
        local i = 0
        local circle = game:GetService("RunService").RenderStepped:Connect(function(dt)
            i = (i + dt/1) % 1
            local alpha = 2 * math.pi * i
            Part.CFrame = CFrame.Angles(0, alpha, 0)* CFrame.new(0, 0, _G.Distance) + game.Players.LocalPlayer.Character.HumanoidRootPart.Position
        end)
    end
end

local tp2 = game:GetService("RunService").Heartbeat:Connect(function()
    for i,v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
        if v:IsA("Accessory") then
            v.Handle.CFrame = v.Handle.CFrame
        end
    end
end)

local function visualize()
    _G.Distance = game.Players.LocalPlayer.Character.BoomBox.Handle.Sound.PlaybackLoudness * 0.1
end

game:GetService('RunService').Heartbeat:Connect(visualize)
end)

Main:AddButton("Following Hats", function()
    local obese = game:GetService('Players')
    for i,v in pairs(obese.LocalPlayer.Character:GetChildren()) do
    if v.ClassName == "Accessory" then
    local stg = v.Handle:FindFirstChildOfClass("BodyForce")
    if stg == nil then
    local a = Instance.new("BodyPosition")
    local b = Instance.new("BodyAngularVelocity")
    a.Parent = v.Handle
    b.Parent = v.Handle
    v.Handle.AccessoryWeld:Destroy()
    b.AngularVelocity = Vector3.new(1,1,1)
    b.MaxTorque = Vector3.new(1,1,1)
    a.P = 150
    a.D = 25
    game:GetService('RunService').Stepped:connect(function()
    a.Position = obese.LocalPlayer.Character.Head.Position
    end)
    end
    end
    end
end)

Main2:AddSeperator("Silent Aim")
-->> Silent Aim [Section 1 - Tab 1]
local Camera = workspace.CurrentCamera
local Players = game:GetService("Players")
local RunService = game:GetService("RunService")
local RenderStepped = RunService.RenderStepped

local LocalPlayer = Players.LocalPlayer
local chr = LocalPlayer.Character
local hum = chr:WaitForChild("Humanoid")

local game = game;
local GetService = game.GetService;

local RunService = game:GetService("RunService")
local RenderStepped = RunService.RenderStepped

local Workspace = GetService(game, "Workspace");
local Players = GetService(game, "Players");
local ReplicatedStorage = GetService(game, "ReplicatedStorage");
local StarterGui = GetService(game, "StarterGui");

local resume = coroutine.resume 
local create = coroutine.create

local LogService = GetService(game, "LogService");
local HttpService = GetService(game, "HttpService");
local ScriptContext = GetService(game, "ScriptContext");

local UIS = game:GetService("UserInputService")

local Request = http_request or request or HttpPost or syn.request
local Player = Players.LocalPlayer;
local Character = Player.Character;
local Mouse = Player:GetMouse()
local Cam = workspace.CurrentCamera;

local WorldToScreen = Cam.WorldToScreenPoint
local WorldToViewportPoint = Cam.WorldToViewportPoint
local GetPartsObscuringTarget = Cam.GetPartsObscuringTarget

local SilentSettings = { Main = { Enabled = false, TeamCheck = false, VisibleCheck = false, TargetPart = "Head" }, FOVSettings = { Visible = false, Radius = 120 } };
local ValidTargetParts = {"Head", "Torso"};

local RequiredArgs = {
ArgCountRequired = 3,
    Args = {
    "Instance", "Vector3", "Vector3", "RaycastParams"
}
}

local fov_circle = Drawing.new("Circle")
fov_circle.Thickness = 1
fov_circle.NumSides = 100
fov_circle.Radius = 120
fov_circle.Filled = false
fov_circle.Visible = false
fov_circle.ZIndex = 999
fov_circle.Transparency = 1
fov_circle.Color = Color3.fromRGB(255, 255 ,255)

local function GetPositionOnScreen(Vector)
local Vec3, OnScreen = WorldToScreen(Cam, Vector)
return Vector2.new(Vec3.X, Vec3.Y), OnScreen
end
local function ValidateArguments(Args, RayMethod)
local Matches = 0

if #Args < RayMethod.ArgCountRequired then
    return false
end

for Pos, Argument in next, Args do
    if typeof(Argument) == RayMethod.Args[Pos] then
        Matches = Matches + 1
    end
end

return Matches >= RayMethod.ArgCountRequired
end
    
local function GetDirection(Origin, Position)
return (Position - Origin).Unit * 1000
end
    
local function GetMousePosition()
return Vector2.new(Mouse.X, Mouse.Y)
end
    
    local function GetClosestPlayer()
        if not SilentSettings.Main.TargetPart then return end

        local Closest
        local DistanceToMouse

        for _, v in next, game.GetChildren(Players) do
            if v == Player then continue end
            if SilentSettings.Main.TeamCheck and v.Team == Player.Team then continue end
    
            local Character = v.Character
            if not Character then continue end
    
            local HumanoidRootPart = game.FindFirstChild(Character, "HumanoidRootPart")
            local Humanoid = game.FindFirstChild(Character, "Humanoid")
    
            if not HumanoidRootPart or not Humanoid or Humanoid and Humanoid.Health <= 0 then continue end
    
            local ScreenPosition, OnScreen = GetPositionOnScreen(HumanoidRootPart.Position)
    
            if not OnScreen then continue end
    
            local Distance = (GetMousePosition() - ScreenPosition).Magnitude
            if Distance <= (DistanceToMouse or (SilentSettings.Main.Enabled and SilentSettings.FOVSettings.Radius) or 2000) then
                Closest = ((SilentSettings.Main.TargetPart == "Random" and Character[ValidTargetParts[math.random(1, #ValidTargetParts)]]) or Character[SilentSettings.Main.TargetPart])
                DistanceToMouse = Distance
            end
        end
        return Closest
    end
    
            local oldNamecall
    oldNamecall = hookmetamethod(game, "__namecall", function(...)
        local Method = getnamecallmethod()
        local Arguments = {...}
        local self = Arguments[1]
    
        if SilentSettings.Main.Enabled and self == workspace then
            if ValidateArguments(Arguments, RequiredArgs) then
                local A_Origin = Arguments[2]
                local HitPart = GetClosestPlayer()

                if HitPart then
                    Arguments[3] = GetDirection(A_Origin, HitPart.Position)

                    return oldNamecall(unpack(Arguments))
                end
            end
        end

        return oldNamecall(...)
end)
    

resume(create(function()
game:GetService("RunService").RenderStepped:Connect(function()
    if SilentSettings.FOVSettings.Visible then 
        fov_circle.Position = GetMousePosition() + Vector2.new(0, 36)
    end
end)
end))

local SaylintTogle = Main2:AddToggle("Enabled", false, function(v)
SilentSettings.Main.Enabled = v
end)

Main2:AddDropdown("Hit Part", {"Head", "Torso", "Random"}, "Head", false, function(V)
SilentSettings.Main.TargetPart = V
end)


local FovToggle = Main2:AddToggle("Fov Circle", false, function(v)
SilentSettings.FOVSettings.Visible = v
fov_circle.Visible = v
end)

local Slider1 = Main2:AddSlider("Fov Radius", 5, 5, 1000, 1, function(v)
SilentSettings.FOVSettings.Radius = v
fov_circle.Radius = v
end)

local Colorpicker1 = Main2:AddColorpicker("Fov Color", Color3.new(1, 1, 1), function(v)
fov_circle.Color = v
end) 


Main2:AddSeperator("Gun Mods")

Main2:AddToggle("No Recoil", false, function(v)
if v == true then
    ToggleBitzFeature("NoRecoil", true)
end
if v == false then
    ToggleBitzFeature("NoRecoil", false)
end
end)

Main2:AddToggle("No Spread", false, function(v)
if v == true then
    ToggleBitzFeature("NoSpread", true)
end
if v == false then
    ToggleBitzFeature("NoSpread", false)
end
end)

Main2:AddToggle("Auto Mode", Settings.GunMods.AutoMode, function(V)
Settings.GunMods.AutoMode = V
end)














Main2:AddToggle("Wallbang", false, function(v)
game:service[[Workspace]]:FindFirstChild('Map'):FindFirstChild('Parts'):FindFirstChild('M_Parts').Parent = game:service[[Workspace]]:FindFirstChild('Characters')
end)

Main2:AddSeperator("Misc")

Main2:AddButton("Melee Godmode", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/14212352135124/melee-god/main/123", true))()
end)

Main2:AddToggle("Infinite Pepper Spray", Settings.InfinitePepperSpray, function(V)
    Settings.InfinitePepperSpray = V
end)

local KillAuraEnabled = false
Main2:AddToggle("Kill Aura", false, function(v)
KillAuraEnabled = v
end)

Main2:AddToggle("Hitbox Extender", false, function(v)
_G.HBE = v
_G.HBE_Size = (_G.HEADSIZE)

local head_size = game.Players.LocalPlayer.Character:FindFirstChild("Head").Size

game:GetService("RunService").Heartbeat:connect(function()
for i, v in next, game:GetService("Players"):GetPlayers() do
    if v.Name ~= game:GetService("Players").LocalPlayer.Name then
        pcall(function()
            if _G.HBE then
                v.Character.Head.Size = Vector3.new(_G.HBE_Size, _G.HBE_Size, _G.HBE_Size)
                v.Character.Head.Transparency = 0.8
            else
                v.Character.Head.Size = head_size
                v.Character.Head.Transparency = 0
            end
        end)
    end
end
end)

local old

old = hookmetamethod(game,"__index",function(self,index)
if index == "Size" and not checkcaller() then
    if old(self,"Name") == "Head" then
        return head_size
    end
end
return old(self,index)
end)
end)

Main2:AddSlider("Slider", 1, 1, 6, 1, function(v)
_G.HEADSIZE = v
end)

Main2:AddSeperator("Material")

Main2:AddToggle("Enabled", Settings.ViewModel.Enabled, function(V)
    Settings.ViewModel.Enabled = V
end)

Main2:AddColorpicker("Viewmodel Color", Color3.new(1, 1, 1), function(V)
    Settings.ViewModel.Viewmodel.Color = V
end) 

Main2:AddDropdown("Viewmodel Material", {"ForceField", "Plastic", "Wood", "Slate", "Concrete"}, "ForceField", false, function(V)
    local ThingySelected = nil

    if V == "ForceField" then
        ThingySelected = Enum.Material.ForceField
    elseif V == "Plastic" then
        ThingySelected = Enum.Material.Plastic
    elseif V == "Wood" then
        ThingySelected = Enum.Material.Wood
    elseif V == "Slate" then
        ThingySelected = Enum.Material.Slate
    elseif V == "Concrete" then
        ThingySelected = Enum.Material.Concrete
    end

    Settings.ViewModel.Viewmodel.Material = ThingySelected
end)

Main2:AddColorpicker("Guns Color", Color3.new(1, 1, 1), function(V)
    Settings.ViewModel.Guns.Color = V
end) 

Main2:AddDropdown("Guns Material", {"ForceField", "Plastic", "Wood", "Slate", "Concrete"}, "ForceField", false, function(V)
    local ThingySelected = nil

    if V == "ForceField" then
        ThingySelected = Enum.Material.ForceField
    elseif V == "Plastic" then
        ThingySelected = Enum.Material.Plastic
    elseif V == "Wood" then
        ThingySelected = Enum.Material.Wood
    elseif V == "Slate" then
        ThingySelected = Enum.Material.Slate
    elseif V == "Concrete" then
        ThingySelected = Enum.Material.Concrete
    end

    Settings.ViewModel.Guns.Material = ThingySelected
end)

Main2:AddColorpicker("Melees Color", Color3.new(1, 1, 1), function(V)
    Settings.ViewModel.Melees.Color = V
end) 

Main2:AddDropdown("Melees Material", {"ForceField", "Plastic", "Wood", "Slate", "Concrete"}, "ForceField", false, function(V)
    local ThingySelected = nil

    if V == "ForceField" then
        ThingySelected = Enum.Material.ForceField
    elseif V == "Plastic" then
        ThingySelected = Enum.Material.Plastic
    elseif V == "Wood" then
        ThingySelected = Enum.Material.Wood
    elseif V == "Slate" then
        ThingySelected = Enum.Material.Slate
    elseif V == "Concrete" then
        ThingySelected = Enum.Material.Concrete
    end

    Settings.ViewModel.Melees.Material = ThingySelected
end)


Main3:AddDropdown("Hit Sounds", {"Boink", "TF2", "Rust", "CSGO", "Hitmarker"}, "Boink", false, function(V)
local SelectedId = nil

if V == "Boink" then
    SelectedId = 5451260445
elseif V == "TF2" then
    SelectedId = 5650646664
elseif V == "Rust" then
    SelectedId = 5043539486
elseif V == "CSGO" then
    SelectedId = 8679627751
elseif V == "Hitmarker" then
    SelectedId = 160432334
end

Settings.CustomHitSound = SelectedId

for i, v in pairs(game:GetService("ReplicatedStorage").Storage.HitStuff.Main:GetDescendants()) do
    if v:IsA("Sound") then
        v.SoundId = "rbxassetid://"..SelectedId
    end
end


if Player.PlayerGui:FindFirstChild("MouseGUI") then
    Player.PlayerGui:FindFirstChild("MouseGUI").HitmarkerSound.SoundId = "rbxassetid://"..SelectedId
    Player.PlayerGui:FindFirstChild("MouseGUI").HeadshotSound.SoundId = "rbxassetid://"..SelectedId
end
end)

Main3:AddSlider("Hitsound Volume", 1, Settings.VolumeHitsound, 10, 10, function(V)
Settings.VolumeHitsound = V
end)



Main3:AddButton("Block Troll [FE]", function()
game.Players.LocalPlayer.Character["Left Arm"]:Destroy()
game.Players.LocalPlayer.Character["Right Leg"]:Destroy()
game.Players.LocalPlayer.Character["Left Leg"]:Destroy()
game.Players.LocalPlayer.Character.Humanoid.HipHeight = 10
for i,v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
    if v:IsA("SpecialMesh") or v.Name == "SpecialMesh" then
        v:Destroy()
    end
end
end)

Main3:AddButton("Force Reset", function()
game.Players.LocalPlayer.Character.Humanoid.Health = 0
end)

Main3:AddToggle("Enable Chat", false, function(v)
if v == true then
    local ChatFrame = game.Players.LocalPlayer.PlayerGui.Chat.Frame
    ChatFrame.ChatChannelParentFrame.Visible = true
    ChatFrame.ChatBarParentFrame.Position = ChatFrame.ChatChannelParentFrame.Position + UDim2.new(UDim.new(), ChatFrame.ChatChannelParentFrame.Size.Y)
elseif v == false then
    local ChatFrame = game.Players.LocalPlayer.PlayerGui.Chat.Frame
    ChatFrame.ChatChannelParentFrame.Visible = false
    ChatFrame.ChatBarParentFrame.Position = ChatFrame.ChatChannelParentFrame.Position + UDim2.new(0, 0, 0, 0)
end
end)

Main3:AddToggle("Fast Death", false, function(v)
_G.AntiStomp = v
local Downed = game:GetService("ReplicatedStorage").CharStats[game:GetService("Players").LocalPlayer.Name].Downed
Downed.Changed:Connect(function()
    if Downed.Value == true and _G.AntiStomp == true then
        for i, v in pairs(game:GetService("Players").LocalPlayer.Character:GetChildren()) do
            if v:IsA("BasePart") then
                v:Destroy()
            end
        end
    end
end)
end)

Main3:AddSeperator("Unlocks")

Main3:AddToggle("Unlock nearby doors", Settings.UnlockDoorsNearby, function(v)
Settings.UnlockDoorsNearby = v
end)

Main3:AddToggle("Open nearby doors", Settings.OpenDoorsNearby, function(v)
Settings.OpenDoorsNearby = v
end)

Main3:AddSeperator("Auto(s)")

Main3:AddToggle("Auto Lockpick", false, function(v)

Main3:AddToggle("[⚠️] Auto Pickup All", false, function(v)
getgenv().Instant = v

while Instant do wait(0.5)
for _,v in pairs(game:GetService("Workspace"):GetDescendants()) do
    if v:IsA("ProximityPrompt") and game:GetService("Players").LocalPlayer:DistanceFromCharacter(v.Parent.Position) <= 30 then
      fireproximityprompt(v,0)
      wait(0.1)
      fireproximityprompt(v,1)
    end
end
end 
end)


Main3:AddToggle("Auto Pickup Tools", Settings.AutoPickTools, function(v)
    Settings.AutoPickTools = v
end)

Main3:AddToggle("Auto Pickup Cash", Settings.AutoPickCash, function(v)
    Settings.AutoPickCash = v
end)

Main3:AddToggle("Auto Pickup Scrap", Settings.AutoPickScrap, function(v)
    Settings.AutoPickScrap = v
end)

Main4:AddSeperator("Player ESP")

Main4:AddToggle("Enable ESP", ESPSettings.PlayerESP.Enabled, function(v)
    ESPSettings.PlayerESP.Enabled = v
    ESPFramework.Color = Color3.fromRGB(24, 117, 255)
    ESPFramework.ToolColor = ESPSettings.ToolColor
    ESPFramework.Tracers = ESPSettings.PlayerESP.TracersOn
    ESPFramework.Names = ESPSettings.PlayerESP.NamesOn
    ESPFramework.Health = ESPSettings.PlayerESP.HealthOn
    ESPFramework.Distance = ESPSettings.PlayerESP.DistanceOn
    ESPFramework.Tool = ESPSettings.PlayerESP.ToolOn
    ESPFramework.Boxes = ESPSettings.PlayerESP.BoxesOn
    ESPFramework.FaceCamera = ESPSettings.PlayerESP.FaceCamOn
    ESPFramework:Toggle(ESPSettings.PlayerESP.Enabled)
end, "PlayerESPsToggle")

Main4:AddToggle("Face Camera", ESPSettings.PlayerESP.FaceCamOn, function(v)
    ESPSettings.PlayerESP.FaceCamOn = v
    ESPFramework.FaceCamera = ESPSettings.PlayerESP.FaceCamOn
end)

Main4:AddToggle("Box ESP", ESPSettings.PlayerESP.BoxesOn, function(v)
    ESPSettings.PlayerESP.BoxesOn = v
    ESPFramework.Boxes = ESPSettings.PlayerESP.BoxesOn
end)

Main4:AddToggle("Tracers ESP", ESPSettings.PlayerESP.TracersOn, function(v)
    ESPSettings.PlayerESP.TracersOn = v
    ESPFramework.Tracers = ESPSettings.PlayerESP.TracersOn
end)

Main4:AddToggle("Name ESP", ESPSettings.PlayerESP.NamesOn, function(v)
    ESPSettings.PlayerESP.NamesOn = v
    ESPFramework.Names = ESPSettings.PlayerESP.NamesOn
end)

Main4:AddToggle("Health ESP", ESPSettings.PlayerESP.HealthOn, function(v)
    ESPSettings.PlayerESP.HealthOn = v
    ESPFramework.Health = ESPSettings.PlayerESP.HealthOn
end)

Main4:AddToggle("Tool ESP", ESPSettings.PlayerESP.ToolOn, function(v)
    ESPSettings.PlayerESP.ToolOn = v
    ESPFramework.Tool = ESPSettings.PlayerESP.ToolOn
end)

Main4:AddToggle("Distance ESP", ESPSettings.PlayerESP.DistanceOn, function(v)
    ESPSettings.PlayerESP.DistanceOn = v
    ESPFramework.Distance = ESPSettings.PlayerESP.DistanceOn
end)

Main4:AddSeperator("Enviroment ESP")

local ESP = loadstring(game:HttpGet("https://kiriot22.com/releases/ESP.lua"))()
ESP:Toggle(true)
ESP.Players = false 
ESP.Tracers = false 
ESP.Boxes = false 
ESP.Names = false

-- Med safes
for i,v in pairs(game:GetService("Workspace").Map.BredMakurz:GetDescendants()) do
if string.find(v.Name,"MediumSafe") then 
    if v:FindFirstChild("MainPart") then 
        ESP:Add(v.MainPart, {
            Name = "Medium Safe",
            IsEnabled = "mediumSafe",
            Color = Color3.fromRGB(228, 236, 243)
        })
    end 
end 
end

-- Small safes
for i,v in pairs(game:GetService("Workspace").Map.BredMakurz:GetDescendants()) do
if string.find(v.Name,"SmallSafe") then 
    if v:FindFirstChild("MainPart") then 
        ESP:Add(v.MainPart, {
            Name = "Small Safe",
            IsEnabled = "smallSafe",
            Color = Color3.fromRGB(228, 236, 243)
        })
    end 
end 
end

-- Registers
for i,v in pairs(game:GetService("Workspace").Map.BredMakurz:GetDescendants()) do
if string.find(v.Name,"Register") then 
    if v:FindFirstChild("MainPart") then 
        ESP:Add(v.MainPart, {
            Name = "Register",
            IsEnabled = "registerSafe",
            Color = Color3.fromRGB(228, 236, 243)
        })
    end 
end 
end

-- ATMs 
for i,v in pairs(game:GetService("Workspace").Map.ATMz:GetDescendants()) do
if string.find(v.Name,"ATM") then 
    if v:FindFirstChild("MainPart") then 
        ESP:Add(v.MainPart, {
            Name = "ATM",
            IsEnabled = "atmPart",
            Color = Color3.fromRGB(228, 236, 243)
        })
    end 
end 
end

-- Dealers
for i,v in pairs(game:GetService("Workspace").Map.Shopz:GetDescendants()) do
if string.find(v.Name,"Dealer") then 
    if v:FindFirstChild("MainPart") then 
        ESP:Add(v.MainPart, {
            Name = "Dealer",
            IsEnabled = "dealerStore",
            Color = Color3.fromRGB(228, 236, 243)
        })
    end 
end 
end


-- Scraps
ESP:AddObjectListener(game:GetService("Workspace").Filter.SpawnedPiles, {
Type = "Model",
CustomName = "Scrap",
Color = Color3.fromRGB(228, 236, 243),
IsEnabled = "scrapPart"
})

Main4:AddToggle("Enable ESP", false, function(Value)
ESP:Toggle(Value)
end)

Main4:AddToggle("ESP Boxes", false, function(Value)
ESP.Boxes = Value  
end)


Main4:AddToggle("ESP Nametags", false, function(Value)
ESP.Names = Value 
end)


Main4:AddToggle("Show Medium Safes", false, function(Value)
ESP.mediumSafe = Value 
end)

Main4:AddToggle("Show Small Safes", false, function(Value)
ESP.smallSafe = Value 
end)

Main4:AddToggle("Show Registers", false, function(Value)
ESP.registerSafe = Value 
end)

Main4:AddToggle("Show ATMs", false, function(Value)
ESP.atmPart = Value 
end)

Main4:AddToggle("Show Dealers", false, function(Value)
ESP.dealerStore = Value 
end)

Main4:AddToggle("Show Scraps", false, function(Value)
ESP.scrapPart = Value 
end)




Main6:AddSeperator("Main")

Main6:AddColorpicker("Main ESP", ESPFramework.Color, function(V)
    ESPFramework.Color = V
    ESPSettings.ESPColor = V
end)

Main6:AddColorpicker("Tool ESP", ESPFramework.ToolColor, function(V)
   ESPFramework.ToolColor = V
   ESPSettings.ToolColor = V
end)


Main6:AddColorpicker("Health ESP", ESPFramework.HealthColor, function(V)
   ESPFramework.HealthColor = V
   ESPSettings.HealthColor = V
end)

Main6:AddColorpicker("DistanceESP", ESPFramework.DistanceColor, function(V)
   ESPFramework.DistanceColor = V
   ESPSettings.DistanceColor = V
end)



Main6:AddSeperator("UI Settings")

Main6:AddColorpicker("Accent 1", Framework.theme.accentcolor, function(V)
Framework.theme.accentcolor = V
end)

Main6:AddColorpicker("Accent 2", Framework.theme.accentcolor2, function(V)
Framework.theme.accentcolor2 = V
end)

Main6:AddSeperator("Signs")

Main6:AddLabel("⚠️ - Lag")
Main6:AddLabel("❗ - Blatant")


spawn(function()
local function closestHumanoidRootPart(maxDist)
local dist = maxDist
local ret = nil
for i, v in next, game.Players:GetPlayers() do
    if v ~= game.Players.LocalPlayer then
        if v.Character then
            local chr = v.Character
            if chr:FindFirstChild("HumanoidRootPart") then
                if chr.Humanoid.Health > 0 then
                    local e = chr.HumanoidRootPart
                    local d = (e.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
                    if d < dist then
                        dist = d
                        ret = e
                    end
                end
            end
        end
    end
end
return ret
end
while task.wait() do
if KillAuraEnabled then
    local ClosestHumanoidRootPart = closestHumanoidRootPart(10)
   if not ClosestHumanoidRootPart then continue end
   if not game.Players.LocalPlayer.Character:FindFirstChildWhichIsA("Tool") then
            continue
     end
    -- if the target or player is downed
    -- check if the player is holding a actual melee
    local KillAuraValue = game:GetService("ReplicatedStorage").Events["XMHH.1"]:InvokeServer(
        "\240\159\154\168",
        tick(),
        game:GetService("Players").LocalPlayer.Character:FindFirstChildWhichIsA("Tool"),
        "43TRFWJ",
        "Normal",
        tick(),
        true
    )
    wait(KillAuraTime)
    game:GetService("ReplicatedStorage").Events["XMHH2.1"]:FireServer(
        "\240\159\154\168",
        tick(),
        game:GetService("Players").LocalPlayer.Character:FindFirstChildWhichIsA("Tool"),
        "2389ZFX33",
        KillAuraValue,
        false,
        game:GetService("Players").LocalPlayer.Character["Right Arm"],
        ClosestHumanoidRootPart.Parent:FindFirstChild("Head"),
        ClosestHumanoidRootPart.Parent,
        game:GetService("Players").LocalPlayer.Character["Right Arm"].Position,
        ClosestHumanoidRootPart.Parent:FindFirstChild("Head").Position
    )
end
end
end)

game:GetService("Players").LocalPlayer.CharacterAdded:Connect(function(Character)
Character.ChildAdded:Connect(function(Object)
    if KillAuraEnabled and Object:IsA("Tool") then
pcall(function()
        KillAuraTime = require(game:GetService("Players").LocalPlayer.Character:FindFirstChildWhichIsA("Tool").Config).Mains.E.SwingTime
end)
    end
end)
end)

if game:GetService("Players").LocalPlayer.Character ~= nil then
game:GetService("Players").LocalPlayer.Character.ChildAdded:Connect(function(Object)
    if KillAuraEnabled  and Object:IsA("Tool") then
pcall(function()
        KillAuraTime = require(game:GetService("Players").LocalPlayer.Character:FindFirstChildWhichIsA("Tool").Config).Mains.E.SwingTime
end)
    end
end)
end


Main7:AddSeperator("Settings")

Main7:AddToggle("Toggle Watermark", Settings.WatermarkOn, function(V)
    Watermark.Visible = V
    Settings.WatermarkOn = V
end)

Main7:AddDropdown("Execution Logs", {"Off", "On"}, "Off", false, function(v)
    print('v')
end)

Main7:AddDropdown("Error Logs", {"Off", "On"}, "On", false, function(v)
    print('v')
end)

Main7:AddSeperator("E Guard!")



Main10:AddSeperator("Panic")

Main10:AddButton("Fake Crash", function()
    local Player = game.Players.LocalPlayer
    game.Players.LocalPlayer:Kick("")
end)

Main10:AddButton("Fake Disconnect", function()
    local Player = game.Players.LocalPlayer
    game.Players.LocalPlayer:Kick("Client Disconnected.")
end)



end)
