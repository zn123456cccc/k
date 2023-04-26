--//====================================================\\--
--||                       BASIS
--\\====================================================//--
 
-- CREDIT TO THE ORIGINAL OWNERS
game.TestService.IsSleepAllowed = false
for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
	if v:IsA("BasePart") then 
		game:GetService("RunService").Heartbeat:connect(function()
			v.Velocity = Vector3.new(-40,0,-10)
			pcall(function()
				v.CanCollide = false
			end)
			pcall(function()
				v.CanQuery = false
			end)
		end)
	end
end

Bypass = "death"
loadstring(game:GetObjects("rbxassetid://5325226148")[1].Source)()
for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
game:GetService("RunService").Heartbeat:connect(function()
v.Velocity = Vector3.new(0,30,0)
wait(0.5)
end)
end
end
local p = game.Players.LocalPlayer
local char = p.Character
local mouse = p:GetMouse()
local larm = char["Left Arm"]
local rarm = char["Right Arm"]
local lleg = char["Left Leg"]
local rleg = char["Right Leg"]
local hed = char.Head
local torso = char.Torso
local hum = char.Humanoid
local cam = game.Workspace.CurrentCamera
local root = char.HumanoidRootPart
for i,v in pairs (char:GetChildren()) do
	if v:IsA("Accessory") then
		v.Handle.Massless = true
		v.Handle.CustomPhysicalProperties = PhysicalProperties.new(0,0,0,0,0)
	end
end

hed.Massless = true
hed.CustomPhysicalProperties = PhysicalProperties.new(0,0,0,0,0)
torso.Massless = true
torso.CustomPhysicalProperties = PhysicalProperties.new(0,0,0,0,0)
rarm.Massless = true
rarm.CustomPhysicalProperties = PhysicalProperties.new(0,0,0,0,0)
larm.Massless = true
larm.CustomPhysicalProperties = PhysicalProperties.new(0,0,0,0,0)
lleg.Massless = true
lleg.CustomPhysicalProperties = PhysicalProperties.new(0,0,0,0,0)
rleg.Massless = true
rleg.CustomPhysicalProperties = PhysicalProperties.new(0,0,0,0,0)
root.Massless = true
root.CustomPhysicalProperties = PhysicalProperties.new(0,0,0,0,0)
warn("Netless Activated!")
Bypass = "Death"
plr = game.Players.LocalPlayer
dead = false
char = plr.Character



bullet = workspace[plr.Name]["HumanoidRootPart"]
bullet.Transparency = 0
bhandle = bullet
bullet.Massless = true

mouse = plr:GetMouse()
head = char.Head
camera = workspace.CurrentCamera
lt = true
ltt = false

local function IsFirstPerson()
     return (head.CFrame.p - camera.CFrame.p).Magnitude < 1
end

     bbv = Instance.new("BodyPosition",bhandle)
     bbv.Position = char.Torso.CFrame.p
   
     
     
     mouse.Button1Down:Connect(function()
         if dead == false then
        lt = false
        ltt = false
     bbav = Instance.new("BodyAngularVelocity",bhandle)
     bbav.MaxTorque = Vector3.new(math.huge,math.huge,math.huge)
     bbav.P = 1000000000000000000000000000
     bbav.AngularVelocity = Vector3.new(10000000000000000000000000000000,100000000000000000000000000,100000000000000000)
     game:GetService("Debris"):AddItem(bbav,0.1)
        if game.Players:GetPlayerFromCharacter(mouse.Target.Parent) then
            if mouse.Target.Parent.Name == char.Name or mouse.Target.Parent.Name == "non" then return end
              --repeat 
            game:GetService("RunService").RenderStepped:Wait()
            bbv.Position = (CFrame.new(mouse.Target.Parent.HumanoidRootPart.CFrame.p,char.Torso.CFrame.p) * CFrame.new(0,0,0)).p
            bhandle.Position = (CFrame.new(mouse.Target.Parent.HumanoidRootPart.CFrame.p,char.Torso.CFrame.p) * CFrame.new(0,0,0)).p
            wait(1)
            --until char.Humanoid.Health == 100 or char.Humanoid.Health == 0
        elseif game.Players:GetPlayerFromCharacter(mouse.Target.Parent.Parent) then
            if mouse.Target.Parent.Name == char.Name or mouse.Target.Parent.Name == "non" then return end
            --repeat 
            game:GetService("RunService").RenderStepped:Wait()
            bbv.Position = (CFrame.new(mouse.Target.Parent.Parent.HumanoidRootPart.CFrame.p,char.Torso.CFrame.p) * CFrame.new(0,0,0)).p
            bhandle.Position = (CFrame.new(mouse.Target.Parent.Parent.HumanoidRootPart.CFrame.p,char.Torso.CFrame.p) * CFrame.new(0,0,0)).p
            wait(1)
            --until char.Humanoid.Health == 100 or char.Humanoid.Health == 0
            
            else
       -- repeat 
        game:GetService("RunService").RenderStepped:Wait()
        wait(1)
        --until char.Humanoid.Health == 100 or char.Humanoid.Health == 0
        end
        wait()
        lt = true
         end
         end)
         
    spawn(
        function()
            while true do
                game:GetService("RunService").Heartbeat:Wait()
                bullet.Velocity = Vector3.new(0,26,0)
         end
    end)

 plr:GetMouse().Button1Down:Connect(function()
attackingwithhrp = true	
end)

 
plr:GetMouse().Button1Up:Connect(function()
attackingwithhrp = false
end)

plr:GetMouse().Button1Down:Connect(function()
repeat wait() until attackingwithhrp == true
repeat
game:GetService("RunService").Heartbeat:Wait()
if plr:GetMouse().Target ~= nil then
bullet.Position = game:GetService("Players").LocalPlayer:GetMouse().Hit.p
end
until attackingwithhrp == false
end)

local MODULE = game:GetObjects("rbxassetid://10446353580")[1]
local CHARACTER = Workspace.non
local PLAYER = game:GetService("Players").LocalPlayer
local HUM = CHARACTER.Humanoid


local ROOT = HUM.Torso
local HEAD = CHARACTER.Head
local TORSO = CHARACTER.Torso
local RIGHTARM = CHARACTER["Right Arm"]
local LEFTARM = CHARACTER["Left Arm"]
local RIGHTLEG = CHARACTER["Right Leg"]
local LEFTLEG = CHARACTER["Left Leg"]
local ROOTJOINT = ROOT["RootJoint"]
local NECK = TORSO["Neck"]
local RIGHTSHOULDER = TORSO["Right Shoulder"]
local LEFTSHOULDER = TORSO["Left Shoulder"]
local RIGHTHIP = TORSO["Right Hip"]
local LEFTHIP = TORSO["Left Hip"]
local MOUSEPOS = ROOT.Position

IT = Instance.new
CF = CFrame.new
VT = Vector3.new
RAD = math.rad
C3 = Color3.new
UD2 = UDim2.new
BRICKC = BrickColor.new
ANGLES = CFrame.Angles
EULER = CFrame.fromEulerAnglesXYZ
COS = math.cos
ACOS = math.acos
SIN = math.sin
ASIN = math.asin
ABS = math.abs
MRANDOM = math.random
FLOOR = math.floor

--//====================================================\\--
--||                  BACKGROUND VALUES
--\\====================================================//--

local ANIM_SPEED = 3
local MOUSE = PLAYER:GetMouse()
local FRAME_SPEED = 1 / 60 -- (1 / 30) OR (1 / 60)
local CHANGE = 2 / ANIM_SPEED
local DAMAGEMULTIPLIER = 1
local ANIM = "Idle"
local KEYHOLD = false
local MOUSEHOLD = false
local SINE = 0
local ATTACKING = false
local Debris = game:GetService("Debris")
local Effects = IT("Folder",CHARACTER)
Effects.Name = "FXFolder"
local ROOTC0 = CF(0, 0, 0) * ANGLES(RAD(-90), RAD(0), RAD(180))
local NECKC0 = CF(0, 1, 0) * ANGLES(RAD(-90), RAD(0), RAD(180))
local RIGHTSHOULDERC0 = CF(-0.5, 0, 0) * ANGLES(RAD(0), RAD(90), RAD(0))
local LEFTSHOULDERC0 = CF(0.5, 0, 0) * ANGLES(RAD(0), RAD(-90), RAD(0))
local COMBO = 1

--//====================================================\\--
--||                     HEARTBEAT
--\\====================================================//--

ArtificialHB = Instance.new("BindableEvent", script)
ArtificialHB.Name = "ArtificialHB"

script:WaitForChild("ArtificialHB")

frame = FRAME_SPEED
tf = 0
allowframeloss = false
tossremainder = false
lastframe = tick()
script.ArtificialHB:Fire()

game:GetService("RunService").Heartbeat:connect(function(s, p)
	tf = tf + s
	if tf >= frame then
		if allowframeloss then
			ArtificialHB:Fire()
			lastframe = tick()
		else
			for i = 1, math.floor(tf / frame) do
				ArtificialHB:Fire()
			end
			lastframe = tick()
		end
		if tossremainder then
			tf = 0
		else
			tf = tf - frame * math.floor(tf / frame)
		end
	end
end)

function PositiveAngle(NUMBER)
	if NUMBER >= 0 then
		NUMBER = 0
	end
	return NUMBER
end

function NegativeAngle(NUMBER)
	if NUMBER <= 0 then
		NUMBER = 0
	end
	return NUMBER
end

function Swait(NUMBER)
	if NUMBER == 0 or NUMBER == nil then
		ArtificialHB.Event:wait()
	else
		for i = 1, NUMBER do
			ArtificialHB.Event:wait()
		end
	end
end

--//====================================================\\--
--||                       CLERP
--\\====================================================//--

function QuaternionFromCFrame(cf)
	local mx, my, mz, m00, m01, m02, m10, m11, m12, m20, m21, m22 = cf:components()
	local trace = m00 + m11 + m22
	if trace > 0 then 
		local s = math.sqrt(1 + trace)
		local recip = 0.5 / s
		return (m21 - m12) * recip, (m02 - m20) * recip, (m10 - m01) * recip, s * 0.5
	else
		local i = 0
		if m11 > m00 then
			i = 1
		end
		if m22 > (i == 0 and m00 or m11) then
			i = 2
		end
		if i == 0 then
			local s = math.sqrt(m00 - m11 - m22 + 1)
			local recip = 0.5 / s
			return 0.5 * s, (m10 + m01) * recip, (m20 + m02) * recip, (m21 - m12) * recip
		elseif i == 1 then
			local s = math.sqrt(m11 - m22 - m00 + 1)
			local recip = 0.5 / s
			return (m01 + m10) * recip, 0.5 * s, (m21 + m12) * recip, (m02 - m20) * recip
		elseif i == 2 then
			local s = math.sqrt(m22 - m00 - m11 + 1)
			local recip = 0.5 / s return (m02 + m20) * recip, (m12 + m21) * recip, 0.5 * s, (m10 - m01) * recip
		end
	end
end
 
function QuaternionToCFrame(px, py, pz, x, y, z, w)
	local xs, ys, zs = x + x, y + y, z + z
	local wx, wy, wz = w * xs, w * ys, w * zs
	local xx = x * xs
	local xy = x * ys
	local xz = x * zs
	local yy = y * ys
	local yz = y * zs
	local zz = z * zs
	return CFrame.new(px, py, pz, 1 - (yy + zz), xy - wz, xz + wy, xy + wz, 1 - (xx + zz), yz - wx, xz - wy, yz + wx, 1 - (xx + yy))
end
 
function QuaternionSlerp(a, b, t)
	local cosTheta = a[1] * b[1] + a[2] * b[2] + a[3] * b[3] + a[4] * b[4]
	local startInterp, finishInterp;
	if cosTheta >= 0.0001 then
		if (1 - cosTheta) > 0.0001 then
			local theta = ACOS(cosTheta)
			local invSinTheta = 1 / SIN(theta)
			startInterp = SIN((1 - t) * theta) * invSinTheta
			finishInterp = SIN(t * theta) * invSinTheta
		else
			startInterp = 1 - t
			finishInterp = t
		end
	else
		if (1 + cosTheta) > 0.0001 then
			local theta = ACOS(-cosTheta)
			local invSinTheta = 1 / SIN(theta)
			startInterp = SIN((t - 1) * theta) * invSinTheta
			finishInterp = SIN(t * theta) * invSinTheta
		else
			startInterp = t - 1
			finishInterp = t
		end
	end
	return a[1] * startInterp + b[1] * finishInterp, a[2] * startInterp + b[2] * finishInterp, a[3] * startInterp + b[3] * finishInterp, a[4] * startInterp + b[4] * finishInterp
end

function Clerp(a, b, t)
	local qa = {QuaternionFromCFrame(a)}
	local qb = {QuaternionFromCFrame(b)}
	local ax, ay, az = a.x, a.y, a.z
	local bx, by, bz = b.x, b.y, b.z
	local _t = 1 - t
	return QuaternionToCFrame(_t * ax + t * bx, _t * ay + t * by, _t * az + t * bz, QuaternionSlerp(qa, qb, t))
end

--//====================================================\\--
--||                     FUNCTIONS
--\\====================================================//--

function WeldParts(A,B)
	local WLD = IT("ManualWeld")
	WLD.Part0 = A
	WLD.Part1 = B
	WLD.C1 = B.CFrame:inverse() * A.CFrame
	WLD.Parent = A
	return WLD
end

--NewSound({ID = 0,PARENT = ROOT,VOLUME = 0.5,PITCH = 1,LOOP = false,MAXDISTANCE = 1000,EMITTERSIZE = 10,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
function NewSound(TABLE)
	local ID = "rbxassetid://"..(TABLE.ID or 0)
	local PARENT = (TABLE.PARENT or ROOT)
	local VOLUME = (TABLE.VOLUME or 0.5)
	local PITCH = (TABLE.PITCH or 1)
	local LOOP = (TABLE.LOOP or false)
	local MAXDISTANCE = (TABLE.MAXDISTANCE or 100)
	local EMITTERSIZE = (TABLE.EMITTERSIZE or 10)
	local PLAYING = (TABLE.PLAYING or true)
	local PLAYONREMOVE = (TABLE.PLAYONREMOVE or false)
	local DOESDEBRIS = (TABLE.DOESDEBRIS or true)
	if ID ~= "rbxassetid://0" then
		local SOUND = IT("Sound",PARENT)
		SOUND.SoundId = ID
		SOUND.Volume = VOLUME
		SOUND.Pitch = PITCH
		SOUND.Looped = LOOP
		SOUND.MaxDistance = MAXDISTANCE
		SOUND.EmitterSize = EMITTERSIZE
		SOUND.PlayOnRemove = PLAYONREMOVE
		if DOESDEBRIS == true and PLAYING == true and LOOP == false then
			Debris:AddItem(SOUND,SOUND.TimeLength+5)
		end
		if PLAYING == true then
			SOUND:Play()
		end
		return SOUND
	end
end

function CreateMesh(MESH, PARENT, MESHTYPE, MESHID, TEXTUREID, SCALE, OFFSET)
	local NEWMESH = IT(MESH)
	if MESH == "SpecialMesh" then
		NEWMESH.MeshType = MESHTYPE
		if MESHID ~= "nil" and MESHID ~= "" then
			NEWMESH.MeshId = "http://www.roblox.com/asset/?id="..MESHID
		end
		if TEXTUREID ~= "nil" and TEXTUREID ~= "" then
			NEWMESH.TextureId = "http://www.roblox.com/asset/?id="..TEXTUREID
		end
	end
	NEWMESH.Offset = OFFSET or VT(0, 0, 0)
	NEWMESH.Scale = SCALE
	NEWMESH.Parent = PARENT
	return NEWMESH
end

function CreatePart(FORMFACTOR, PARENT, MATERIAL, REFLECTANCE, TRANSPARENCY, BRICKCOLOR, NAME, SIZE, ANCHOR)
	local NEWPART = IT("Part")
	NEWPART.formFactor = FORMFACTOR
	NEWPART.Reflectance = REFLECTANCE
	NEWPART.Transparency = TRANSPARENCY
	NEWPART.CanCollide = false
	NEWPART.Locked = true
	NEWPART.Anchored = true
	if ANCHOR == false then
		NEWPART.Anchored = false
	end
	NEWPART.BrickColor = BRICKC(tostring(BRICKCOLOR))
	NEWPART.Name = NAME
	NEWPART.Size = SIZE
	NEWPART.Position = ROOT.Position
	NEWPART.Material = MATERIAL
	NEWPART:BreakJoints()
	NEWPART.Parent = PARENT
	return NEWPART
end

function Raycast(POSITION, DIRECTION, RANGE, IGNOREDECENDANTS)
	return workspace:FindPartOnRay(Ray.new(POSITION, DIRECTION.unit * RANGE), IGNOREDECENDANTS)
end

--WACKYEFFECT({EffectType = "", Size = VT(1,1,1), Size2 = VT(0,0,0), Transparency = 0, Transparency2 = 1, CFrame = CF(), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = C3(1,1,1), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = false, Boomerang = 0, SizeBoomerang = 0})
function WACKYEFFECT(Table)
	local TYPE = (Table.EffectType or "Sphere")
	local SIZE = (Table.Size or VT(1,1,1))
	local ENDSIZE = (Table.Size2 or VT(0,0,0))
	local TRANSPARENCY = (Table.Transparency or 0)
	local ENDTRANSPARENCY = (Table.Transparency2 or 1)
	local CFRAME = (Table.CFrame or ROOT.CFrame)
	local MOVEDIRECTION = (Table.MoveToPos or nil)
	local ROTATION1 = (Table.RotationX or 0)
	local ROTATION2 = (Table.RotationY or 0)
	local ROTATION3 = (Table.RotationZ or 0)
	local MATERIAL = (Table.Material or "Neon")
	local COLOR = (Table.Color or C3(1,1,1))
	local TIME = (Table.Time or 45)
	local SOUNDID = (Table.SoundID or nil)
	local SOUNDPITCH = (Table.SoundPitch or nil)
	local SOUNDVOLUME = (Table.SoundVolume or nil)
	local USEBOOMERANGMATH = (Table.UseBoomerangMath or false)
	local BOOMERANG = (Table.Boomerang or 0)
	local SIZEBOOMERANG = (Table.SizeBoomerang or 0)
	coroutine.resume(coroutine.create(function()
		local PLAYSSOUND = false
		local SOUND = nil
		local EFFECT = CreatePart(3, Effects, MATERIAL, 0, TRANSPARENCY, BRICKC("Pearl"), "Effect", VT(1,1,1), true)
		if SOUNDID ~= nil and SOUNDPITCH ~= nil and SOUNDVOLUME ~= nil then
			PLAYSSOUND = true
			SOUND = NewSound({ID = SOUNDID,PARENT = EFFECT,VOLUME = SOUNDVOLUME,PITCH = SOUNDPITCH,LOOP = false,MAXDISTANCE = 200,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
		end
		EFFECT.Color = COLOR
		local MSH = nil
		if TYPE == "Sphere" then
			MSH = CreateMesh("SpecialMesh", EFFECT, "Sphere", "", "", SIZE, VT(0,0,0))
		elseif TYPE == "Block" or TYPE == "Box" then
			MSH = IT("BlockMesh",EFFECT)
			MSH.Scale = SIZE
		elseif TYPE == "Wave" then
			MSH = CreateMesh("SpecialMesh", EFFECT, "FileMesh", "20329976", "", SIZE, VT(0,0,-SIZE.X/8))
		elseif TYPE == "Ring" then
			MSH = CreateMesh("SpecialMesh", EFFECT, "FileMesh", "559831844", "", VT(SIZE.X,SIZE.X,0.1), VT(0,0,0))
		elseif TYPE == "Slash" then
			MSH = CreateMesh("SpecialMesh", EFFECT, "FileMesh", "662586858", "", VT(SIZE.X/10,0,SIZE.X/10), VT(0,0,0))
		elseif TYPE == "Round Slash" then
			MSH = CreateMesh("SpecialMesh", EFFECT, "FileMesh", "662585058", "", VT(SIZE.X/10,0,SIZE.X/10), VT(0,0,0))
		elseif TYPE == "Swirl" then
			MSH = CreateMesh("SpecialMesh", EFFECT, "FileMesh", "168892432", "", SIZE, VT(0,0,0))
		elseif TYPE == "Skull" then
			MSH = CreateMesh("SpecialMesh", EFFECT, "FileMesh", "4770583", "", SIZE, VT(0,0,0))
		elseif TYPE == "Crystal" then
			MSH = CreateMesh("SpecialMesh", EFFECT, "FileMesh", "9756362", "", SIZE, VT(0,0,0))
		end
		if MSH ~= nil then
			local BOOMR1 = 1+BOOMERANG/50
			local BOOMR2 = 1+SIZEBOOMERANG/50
			local MOVESPEED = nil
			if MOVEDIRECTION ~= nil then
				if USEBOOMERANGMATH == true then
					MOVESPEED = ((CFRAME.p - MOVEDIRECTION).Magnitude/TIME)*BOOMR1
				else
					MOVESPEED = ((CFRAME.p - MOVEDIRECTION).Magnitude/TIME)
				end
			end
			local GROWTH = nil
			if USEBOOMERANGMATH == true then
				GROWTH = (SIZE - ENDSIZE)*(BOOMR2+1)
			else
				GROWTH = (SIZE - ENDSIZE)
			end
			local TRANS = TRANSPARENCY - ENDTRANSPARENCY
			if TYPE == "Block" then
				EFFECT.CFrame = CFRAME*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)))
			else
				EFFECT.CFrame = CFRAME
			end
			if USEBOOMERANGMATH == true then
				for LOOP = 1, TIME+1 do
					Swait()
					MSH.Scale = MSH.Scale - (VT((GROWTH.X)*((1 - (LOOP/TIME)*BOOMR2)),(GROWTH.Y)*((1 - (LOOP/TIME)*BOOMR2)),(GROWTH.Z)*((1 - (LOOP/TIME)*BOOMR2)))*BOOMR2)/TIME
					if TYPE == "Wave" then
						MSH.Offset = VT(0,0,-MSH.Scale.Z/8)
					end
					EFFECT.Transparency = EFFECT.Transparency - TRANS/TIME
					if TYPE == "Block" then
						EFFECT.CFrame = CFRAME*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)))
					else
						EFFECT.CFrame = EFFECT.CFrame*ANGLES(RAD(ROTATION1),RAD(ROTATION2),RAD(ROTATION3))
					end
					if MOVEDIRECTION ~= nil then
						local ORI = EFFECT.Orientation
						EFFECT.CFrame = CF(EFFECT.Position,MOVEDIRECTION)*CF(0,0,-(MOVESPEED)*((1 - (LOOP/TIME)*BOOMR1)))
						EFFECT.CFrame = CF(EFFECT.Position)*ANGLES(RAD(ORI.X),RAD(ORI.Y),RAD(ORI.Z))
					end
				end
			else
				for LOOP = 1, TIME+1 do
					Swait()
					MSH.Scale = MSH.Scale - GROWTH/TIME
					if TYPE == "Wave" then
						MSH.Offset = VT(0,0,-MSH.Scale.Z/8)
					end
					EFFECT.Transparency = EFFECT.Transparency - TRANS/TIME
					if TYPE == "Block" then
						EFFECT.CFrame = CFRAME*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)))
					else
						EFFECT.CFrame = EFFECT.CFrame*ANGLES(RAD(ROTATION1),RAD(ROTATION2),RAD(ROTATION3))
					end
					if MOVEDIRECTION ~= nil then
						local ORI = EFFECT.Orientation
						EFFECT.CFrame = CF(EFFECT.Position,MOVEDIRECTION)*CF(0,0,-MOVESPEED)
						EFFECT.CFrame = CF(EFFECT.Position)*ANGLES(RAD(ORI.X),RAD(ORI.Y),RAD(ORI.Z))
					end
				end
			end
			EFFECT.Transparency = 1
			if PLAYSSOUND == false then
				EFFECT:remove()
			else
				repeat Swait() until EFFECT:FindFirstChildOfClass("Sound") == nil
				EFFECT:remove()
			end
		else
			if PLAYSSOUND == false then
				EFFECT:remove()
			else
				repeat Swait() until EFFECT:FindFirstChildOfClass("Sound") == nil
				EFFECT:remove()
			end
		end
	end))
end

function CameraShake(AREA,RANGE,SHAKE,TIMER)

end

function Chatter(Text,Timer)
	local chat = coroutine.wrap(function()
		if CHARACTER:FindFirstChild("SpeechBoard")~= nil then
			CHARACTER:FindFirstChild("SpeechBoard"):destroy()
		end
		local naeeym2 = IT("BillboardGui",CHARACTER)
		naeeym2.Size = UD2(0,100,0,40)
		naeeym2.StudsOffset = Vector3.new(0,2,0)
		naeeym2.Adornee = HEAD
		naeeym2.Name = "SpeechBoard"
		naeeym2.AlwaysOnTop = true
		local tecks2 = IT("TextLabel",naeeym2)
		tecks2.BackgroundTransparency = 1
		tecks2.BorderSizePixel = 0
		tecks2.Text = ""
		tecks2.Font = "Legacy"
		tecks2.TextSize = 15
		tecks2.TextStrokeTransparency = 0
		tecks2.TextColor3 = Color3.new(1,1,1)
		tecks2.TextStrokeColor3 = Color3.new(0,0,0)
		tecks2.Size = UDim2.new(1,0,0.5,0)
		for i = 1,string.len(Text),1 do
			if naeeym2.Parent ~= CHARACTER then 
				break
			end
			NewSound({ID = 418252437,PARENT = HEAD,VOLUME = 1,PITCH = MRANDOM(8,12)/10,LOOP = false,MAXDISTANCE = 75,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
			tecks2.Text = string.sub(Text,1,i)
			wait(Timer)
		end
		wait(1)
		naeeym2:Destroy()
	end)
	chat()
end

function OofOuchBlood(LOCATION,TO,AMOUNT)
	local P = CreatePart(3, Effects, "Granite", 0, 1, BRICKC("Pearl"), "Blood", VT(0,0,0), true)
	P.CFrame = CF(LOCATION,TO)
	local BLOOD = MODULE.Blood:Clone()
	BLOOD.Parent = P
	BLOOD:Emit(AMOUNT)
	Debris:AddItem(P,2)
end

function ManSlaughter(MAN)

end

function AttachmentCFrame(A)
	return A.Parent.CFrame*CF(A.Position)
end

function CastProperRay(StartPos, EndPos, Distance, Ignore)
	local DIRECTION = CF(StartPos,EndPos).lookVector
	return Raycast(StartPos, DIRECTION, Distance, Ignore)
end

--//====================================================\\--
--||                     CHARACTER
--\\====================================================//--

local GUN = MODULE.Pistol
GUN.Parent = CHARACTER
GUN.Anchored = false
GUN.CFrame = RIGHTARM.CFrame*CF(0,-1.75,0)*ANGLES(RAD(-90),RAD(90),0)
local GRIP = WeldParts(RIGHTARM,GUN)
GRIP.Parent = nil
GUN.CFrame = RIGHTLEG.CFrame*CF(0.5,0.25,0)*ANGLES(RAD(-90),RAD(90),0)
local PISTOLARMC1 = GRIP.C1
local PISTOLLEGC1 = GUN.CFrame:inverse() * RIGHTLEG.CFrame
GRIP.Parent = RIGHTARM

HUM.DisplayDistanceType = "None"
local SHOTGUNMODEL = MODULE.ShotgunThing
local SHOTGUN = SHOTGUNMODEL.Shotgun
SHOTGUNMODEL.Parent = CHARACTER
SHOTGUNMODEL.PrimaryPart = SHOTGUNMODEL.Torso
SHOTGUNMODEL:SetPrimaryPartCFrame(TORSO.CFrame)
local SHOTTORSOWELD = IT("ManualWeld")
SHOTTORSOWELD.Part0 = TORSO
SHOTTORSOWELD.Part1 = SHOTGUN
SHOTTORSOWELD.C1 = SHOTGUN.CFrame:inverse() * TORSO.CFrame
SHOTGUNMODEL.PrimaryPart = SHOTGUNMODEL.Arm
SHOTGUNMODEL:SetPrimaryPartCFrame(RIGHTARM.CFrame)
local SHOTGUNARMWELD = IT("ManualWeld")
SHOTGUNARMWELD.Part0 = RIGHTARM
SHOTGUNARMWELD.Part1 = SHOTGUN
SHOTGUNARMWELD.C1 = SHOTGUN.CFrame:inverse() * RIGHTARM.CFrame
SHOTGUN.Parent = CHARACTER
SHOTGUN.Anchored = false
SHOTGUNMODEL:Remove()
SHOTTORSOWELD.Parent = TORSO
local STATE = "Pistol"


--//====================================================\\--
--||                     ABILITIES
--\\====================================================//--

function FireGun()
	COMBO = 1
	local DETECTKILL = function(HIT,POS,FORCE)

	end
	if GRIP.Parent == RIGHTARM or STATE == "Shotgun" then
		ATTACKING = true
		local GYRO = IT("BodyGyro")
		GYRO.D = 20
		GYRO.P = 5000
		GYRO.MaxTorque = VT(0,4000000,0)
		GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
		GYRO.Parent = ROOT
		HUM.WalkSpeed = 5
		HUM.JumpPower = 0
		if STATE == "Pistol" then
			NewSound({ID = 171140306,PARENT = GUN,VOLUME = 1,PITCH = MRANDOM(9,11)/10,LOOP = false,MAXDISTANCE = 75,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
			repeat
				for i=0, 0.5, 0.1 / ANIM_SPEED do
					Swait()
					GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
					ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(15)), 0.5 / ANIM_SPEED)
					NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(-15)), 0.5 / ANIM_SPEED)
					RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.65, 0.5, 0) * ANGLES(RAD(90), RAD(0), RAD(15)) * RIGHTSHOULDERC0, 2 / ANIM_SPEED)
					LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-5)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
					RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(65), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
					LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				end
				WACKYEFFECT({Time = 12, EffectType = "Block", Size = VT(0,0,0), Size2 = VT(1,1,1), Transparency = 0, Transparency2 = 1, CFrame = CF(AttachmentCFrame(GUN.Nuzzle).p), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = C3(1,1,0), SoundID = 136523485, SoundPitch = 2, SoundVolume = 2.5})
				local HIT,POS = CastProperRay(AttachmentCFrame(GUN.Nuzzle).p,MOUSE.Hit.p,1000,CHARACTER)
				local DISTANCE = (POS - AttachmentCFrame(GUN.Nuzzle).p).Magnitude
				if HIT then
					DETECTKILL(HIT,POS,25)
				end
				WACKYEFFECT({Time = 8, EffectType = "Box", Size = VT(0,0,DISTANCE), Size2 = VT(0.3,0.3,DISTANCE), Transparency = 0, Transparency2 = 1, CFrame = CF(AttachmentCFrame(GUN.Nuzzle).p,POS)*CF(0,0,-DISTANCE/2), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = C3(1,1,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
				for i=0, 0.2, 0.1 / ANIM_SPEED do
					Swait()
					GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
					ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(20)), 0.5 / ANIM_SPEED)
					NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(15), RAD(0), RAD(-20)), 0.5 / ANIM_SPEED)
					RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.70, 0.5, 0.5) * ANGLES(RAD(140), RAD(0), RAD(20)) * RIGHTSHOULDERC0, 0.15 / ANIM_SPEED)
					LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-5)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
					RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(60), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
					LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				end
			until MOUSEHOLD == false
		elseif STATE == "Shotgun" then
			for i=0, 0.2, 0.1 / ANIM_SPEED do
				Swait()
				GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
				ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.1, 0.35, 0.2) * ANGLES(RAD(90), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-0.25, 0.35, -1) * ANGLES(RAD(90), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
				RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			end
			CameraShake(AttachmentCFrame(SHOTGUN.Nuzzle).p,20,25,10)
			WACKYEFFECT({Time = 18, EffectType = "Block", Size = VT(0,0,0), Size2 = VT(1,1,1), Transparency = 0, Transparency2 = 1, CFrame = CF(AttachmentCFrame(SHOTGUN.Nuzzle).p), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = C3(1,1,0), SoundID = 136523485, SoundPitch = 1, SoundVolume = 5})
			for i = 1, 6 do
				local HIT,POS = CastProperRay(AttachmentCFrame(SHOTGUN.Nuzzle).p,CF(AttachmentCFrame(SHOTGUN.Nuzzle).p,MOUSE.Hit.p)*ANGLES(0,0,RAD(MRANDOM(0,359)))*CF(0,MRANDOM(0,15),-100).p,1000,CHARACTER)
				local DISTANCE = (POS - AttachmentCFrame(GUN.Nuzzle).p).Magnitude
				if HIT then
					DETECTKILL(HIT,POS,75)
				end
				WACKYEFFECT({Time = 12, EffectType = "Box", Size = VT(0,0,DISTANCE), Size2 = VT(0.3,0.3,DISTANCE), Transparency = 0, Transparency2 = 1, CFrame = CF(AttachmentCFrame(SHOTGUN.Nuzzle).p,POS)*CF(0,0,-DISTANCE/2), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = C3(1,1,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
			end
			for i=0, 1, 0.1 / ANIM_SPEED do
				Swait()
				ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.1, 0.35, 0.4) * ANGLES(RAD(120), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-0.25, 0.6, -1) * ANGLES(RAD(120), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
				RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			end
		end
		HUM.WalkSpeed = 13
		HUM.JumpPower = 50
		GYRO:Remove()
		ATTACKING = false
	end
end

function GunThrow()
	COMBO = 1
	ATTACKING = true
	HUM.WalkSpeed = 5
	HUM.JumpPower = 0
	if GRIP.Parent == RIGHTARM and STATE == "Pistol" then
		local GYRO = IT("BodyGyro")
		GYRO.D = 20
		GYRO.P = 5000
		GYRO.MaxTorque = VT(0,4000000,0)
		GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
		GYRO.Parent = ROOT
		for i=0, 1, 0.1 / ANIM_SPEED do
			Swait()
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-15)), 0.5 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(15)), 0.5 / ANIM_SPEED)
			RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.45, 0.5, 0.5) * ANGLES(RAD(170), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 0.8 / ANIM_SPEED)
			LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(0)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-60), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
		end
		local INSTANTRESPAWN = false
		GRIP.Parent = nil
		local HIT,POS = CastProperRay(GUN.Position,MOUSE.Hit.p,200,CHARACTER)
		if HIT then
			GUN.Parent = Effects
			GUN.CFrame = CF(POS+VT(0,0.1,0),ROOT.Position)*CF(0,0,-1)*ANGLES(0,RAD(90),0)
			coroutine.resume(coroutine.create(function()
				GUN.CanCollide = true
				wait(0.7)
				while true do
					Swait()
					if ((ROOT.Position-VT(0,2.5,0) - GUN.Position).Magnitude <= 3 or GUN.Parent ~= Effects) and ATTACKING == false then
						break
					end
				end
				ATTACKING = true
				HUM.WalkSpeed = 0
				HUM.JumpPower = 0
				for i=0, 0.3, 0.1 / ANIM_SPEED do
					Swait()
					ROOT.CFrame = Clerp(ROOT.CFrame,CF(ROOT.Position,VT(GUN.Position.X,ROOT.Position.Y,GUN.Position.Z)),0.2)
					ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, -1) * ANGLES(RAD(30), RAD(0), RAD(0)), 1.5 / ANIM_SPEED)
					NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.5 / ANIM_SPEED)
					RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(90), RAD(0), RAD(-10)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
					LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(-10), RAD(0), RAD(-5)) * LEFTSHOULDERC0, 1.5 / ANIM_SPEED)
					RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, 0, -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.5 / ANIM_SPEED)
					LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.2) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(35)), 1.5 / ANIM_SPEED)
				end
				NewSound({ID = 169310310,PARENT = GUN,VOLUME = 5,PITCH = MRANDOM(9,11)/10,LOOP = false,MAXDISTANCE = 75,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
				GUN.Parent = CHARACTER
				GRIP.Parent = RIGHTARM
				GUN.CanCollide = false
				for i=0, 0.15, 0.1 / ANIM_SPEED do
					Swait()
					ROOT.CFrame = Clerp(ROOT.CFrame,CF(ROOT.Position,VT(GUN.Position.X,ROOT.Position.Y,GUN.Position.Z)),0.2)
					ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, -1) * ANGLES(RAD(30), RAD(0), RAD(0)), 1.5 / ANIM_SPEED)
					NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.5 / ANIM_SPEED)
					RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(90), RAD(0), RAD(-10)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
					LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(-10), RAD(0), RAD(-5)) * LEFTSHOULDERC0, 1.5 / ANIM_SPEED)
					RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, 0, -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.5 / ANIM_SPEED)
					LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.2) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(35)), 1.5 / ANIM_SPEED)
				end
				ATTACKING = false
				HUM.WalkSpeed = 10
				HUM.JumpPower = 50
			end))
			local BV = IT("BodyVelocity")
			BV.MaxForce = BV.MaxForce * 500
			BV.Velocity = CF(GUN.Position,ROOT.Position+VT(0,5,0)).lookVector*35
			BV.Parent = GUN
			GUN.RotVelocity = VT(MRANDOM(-25,25),MRANDOM(-25,25),MRANDOM(-25,25))/10
			Debris:AddItem(BV,0.05)
			local HUM = HIT.Parent:FindFirstChildOfClass("Humanoid") or HIT.Parent.Parent:FindFirstChildOfClass("Humanoid")
			if HUM then
				local TORS = HUM.Parent:FindFirstChild("Torso") or HUM.Parent:FindFirstChild("UpperTorso")
				if TORS then
					TORS.RotVelocity = VT(MRANDOM(-25,25),MRANDOM(-25,25),MRANDOM(-25,25))
					local BV = IT("BodyVelocity")
					BV.MaxForce = BV.MaxForce * 500
					BV.Velocity = CF(GUN.Position,TORS.Position+VT(0,0.5,0)).lookVector*65
					BV.Parent = TORS
					Debris:AddItem(BV,0.05)
					NewSound({ID = 2330778973,PARENT = TORS,VOLUME = 3,PITCH = MRANDOM(8,12)/10,LOOP = false,MAXDISTANCE = 125,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
				end
				HUM.Health = HUM.Health - 80
				HUM.PlatformStand = true
				OofOuchBlood(POS,ROOT.Position,5)
				if HUM.Health <= 0 then
					ManSlaughter(HUM.Parent)
				end
			end
		else
			INSTANTRESPAWN = true
			GUN.Parent = nil
		end
		for i=0, 0.35, 0.1 / ANIM_SPEED do
			Swait()
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(25)), 2 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(-25)), 0.5 / ANIM_SPEED)
			RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.45, 0.5, 0.5) * ANGLES(RAD(45), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 2 / ANIM_SPEED)
			LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(0)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(55), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 2 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 2 / ANIM_SPEED)
		end
		if INSTANTRESPAWN == true then
			GUN.Parent = CHARACTER
			GRIP.Parent = RIGHTARM
		end
		GYRO:Remove()
	else
		HUM.WalkSpeed = 0
		for i = 1, 40 do
			Swait()
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(25 - 2.5 * SIN(SINE / 12)), RAD(15), RAD(45*SIN(i/4))), 0.5 / ANIM_SPEED)
			if STATE == "Pistol" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(10 - 2.5 * SIN(SINE / 12))) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-10 + 2.5 * SIN(SINE / 12))) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			elseif STATE == "Shotgun" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.1, 0, 0.3) * ANGLES(RAD(90), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-0.25, 0, -1) * ANGLES(RAD(90), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			end
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
		end
	end
	HUM.WalkSpeed = 13
	HUM.JumpPower = 50
	ATTACKING = false
end

function Grenade()
	COMBO = 1
	ATTACKING = true
	coroutine.resume(coroutine.create(function()
		repeat
			Swait()
			if STATE == "Pistol" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(10)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
				--LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-10 + 2.5 * SIN(SINE / 12))) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			elseif STATE == "Shotgun" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0, 0.3) * ANGLES(RAD(65), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
				--LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.25, 0.45, 0.2) * ANGLES(RAD(45), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			end
		until ATTACKING == false
	end))
	for i=0, 0.2, 0.1 / ANIM_SPEED do
		Swait()
		ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
		NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
		--RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, -0.5) * ANGLES(RAD(0), RAD(0), RAD(10)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
		LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.25, 0.5, 0.4) * ANGLES(RAD(-15), RAD(0), RAD(45)) * LEFTSHOULDERC0, 1.5 / ANIM_SPEED)
		RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
		LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
	end
	local GYRO = IT("BodyGyro")
	GYRO.D = 20
	GYRO.P = 5000
	GYRO.MaxTorque = VT(0,4000000,0)
	GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
	GYRO.Parent = ROOT
	local NADE = CreatePart(3,Effects,"Granite",0,0,"Green","Grenade",VT(0.5, 1, 0.5),false)
	CreateMesh("SpecialMesh",NADE,"FileMesh","232379763","232379808",VT(1.5,1.5,1.5),VT(0,0,0))
	NADE.CFrame = LEFTARM.CFrame*CF(0,-1.2,0)
	local WELD = WeldParts(LEFTARM,NADE)
	for i=0, 0.3, 0.1 / ANIM_SPEED do
		Swait()
		GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
		ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(25)), 0.5 / ANIM_SPEED)
		NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(-25)), 0.5 / ANIM_SPEED)
		--RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, -0.5) * ANGLES(RAD(0), RAD(0), RAD(10)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
		LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.75, 0) * ANGLES(RAD(200), RAD(0), RAD(0)) * LEFTSHOULDERC0, 1.25 / ANIM_SPEED)
		RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
		LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-55), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
	end
	for i=0, 0.1, 0.1 / ANIM_SPEED do
		Swait()
		GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
		ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-25)), 1.25 / ANIM_SPEED)
		NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(25)), 0.5 / ANIM_SPEED)
		--RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, -0.5) * ANGLES(RAD(0), RAD(0), RAD(10)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
		LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.25, -0.25) * ANGLES(RAD(25), RAD(0), RAD(0)) * LEFTSHOULDERC0, 1.25 / ANIM_SPEED)
		RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.25 / ANIM_SPEED)
		LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-55), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.25 / ANIM_SPEED)
	end
	coroutine.resume(coroutine.create(function()
		NewSound({ID = 153647549,PARENT = NADE,VOLUME = 3,PITCH = MRANDOM(8,12)/10,LOOP = false,MAXDISTANCE = 125,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
		NADE.CanCollide = true
		WELD:Remove()
		local FORCE = 50 + (NADE.Position-MOUSE.Hit.p).Magnitude
		if FORCE > 300 then
			FORCE = 300
		end
		local BV = IT("BodyVelocity")
		BV.MaxForce = BV.MaxForce * 500
		BV.Velocity = CF(NADE.Position,MOUSE.Hit.p+VT(0,6,0)).lookVector*FORCE
		BV.Parent = NADE
		Debris:AddItem(BV,0.05)
		local A = IT("Attachment",NADE)
		A.Position = VT(0,0.45,0)
		local B = IT("Attachment",NADE)
		B.Position = VT(0,-0.45,0)
		local TRAIL = script.GrenadeTrail:Clone()
		TRAIL.Parent = NADE
		TRAIL.Attachment0 = A
		TRAIL.Attachment1 = B
		local BOOM = function()
			if NADE.Transparency ~= 1 then
				NADE.Anchored = true
				NADE.CanCollide = false
				NADE.Transparency = 1
				Debris:AddItem(NADE,5)
				NADE.CFrame = CF(NADE.Position)
				NewSound({ID = 142070127,PARENT = NADE,VOLUME = 7,PITCH = MRANDOM(8,12)/10,LOOP = false,MAXDISTANCE = 300,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
				for index, CHILD in pairs(script.Grenade:GetChildren()) do
					local C = CHILD:Clone()
					C.Parent = NADE
					C:Emit(125)
				end
				CameraShake(NADE.Position,35,8.5,170)
				for index, CHILD in pairs(workspace:GetChildren()) do
					if CHILD:FindFirstChildOfClass("Humanoid") and CHILD ~= CHARACTER then
						local HUMAN = CHILD:FindFirstChildOfClass("Humanoid")
						local TORS = CHILD:FindFirstChild("Torso") or CHILD:FindFirstChild("UpperTorso")
						if TORS then
							if (TORS.Position - NADE.Position).Magnitude <= MRANDOM(20,25) then
								NewSound({ID = 150315649,PARENT = TORS,VOLUME = 3,PITCH = MRANDOM(9,11)/10,LOOP = false,MAXDISTANCE = 125,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
								OofOuchBlood(TORS.Position,NADE.Position,75)
								ManSlaughter(CHILD)
								local BV = IT("BodyVelocity")
								BV.MaxForce = BV.MaxForce * 500
								BV.Velocity = CF(NADE.Position,TORS.Position+VT(0,2,0)).lookVector*MRANDOM(75,100)
								BV.Parent = TORS
								Debris:AddItem(BV,0.1)
							end
						end
					end
				end
			end
		end
		local HIT = NADE.Touched:Connect(function(PART)
			if PART.Parent:FindFirstChildOfClass("Humanoid") and PART.Parent ~= CHARACTER then
				BOOM()
			end
		end)
		wait(2)
		BOOM()
	end))
	for i=0, 0.4, 0.1 / ANIM_SPEED do
		Swait()
		GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
		ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-25)), 1.25 / ANIM_SPEED)
		NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(25)), 0.5 / ANIM_SPEED)
		--RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, -0.5) * ANGLES(RAD(0), RAD(0), RAD(10)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
		LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.25, -0.25) * ANGLES(RAD(25), RAD(0), RAD(0)) * LEFTSHOULDERC0, 1.25 / ANIM_SPEED)
		RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.25 / ANIM_SPEED)
		LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-55), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.25 / ANIM_SPEED)
	end
	GYRO:Remove()
	ATTACKING = false
end

function Recollect()
	if HUM.PlatformStand == true then
		local HITFLOOR,POS = Raycast(ROOT.Position, (CF(ROOT.Position, ROOT.Position + VT(0, -1, 0))).lookVector, 4+HUM.HipHeight, CHARACTER)
		if HITFLOOR then
			ROOT.Anchored = true
			ATTACKING = true
			NewSound({ID = 143384769,PARENT = HEAD,VOLUME = 2,PITCH = MRANDOM(9,11)/15,LOOP = false,MAXDISTANCE = 35,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
			for i=0, 0.8, 0.1 / ANIM_SPEED do
				Swait()
				ROOT.CFrame = Clerp(ROOT.CFrame,CF(POS+VT(0,2.5,0))*ANGLES(0,RAD(ROOT.Orientation.Y),0),0.2)
				ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, -1) * ANGLES(RAD(30), RAD(0), RAD(0)), 1.5 / ANIM_SPEED)
				NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.5 / ANIM_SPEED)
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, -1) * ANGLES(RAD(90), RAD(0), RAD(-10)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, -1) * ANGLES(RAD(90), RAD(0), RAD(10)) * LEFTSHOULDERC0, 1.5 / ANIM_SPEED)
				RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, 0, -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.5 / ANIM_SPEED)
				LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.2) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(35)), 1.5 / ANIM_SPEED)
			end
			HUM.PlatformStand = false
			ROOT.Anchored = false
			ATTACKING = false
		end
	end
end

function SwitchGuns()
	if STATE == "Pistol" then
		if GRIP.Parent == RIGHTARM then
			GRIP.Parent = RIGHTLEG
			GRIP.Part0 = RIGHTLEG
			GRIP.C1 = PISTOLLEGC1
			SHOTTORSOWELD.Parent = nil
			SHOTGUNARMWELD.Parent = RIGHTARM
			STATE = "Shotgun"
			NewSound({ID = 171140306,PARENT = ROOT,VOLUME = 1,PITCH = MRANDOM(9,11)/15,LOOP = false,MAXDISTANCE = 75,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
		end
	elseif STATE == "Shotgun" then
		GRIP.Parent = RIGHTARM
		GRIP.Part0 = RIGHTARM
		GRIP.C1 = PISTOLARMC1
		SHOTTORSOWELD.Parent = TORSO
		SHOTGUNARMWELD.Parent = nil
		STATE = "Pistol"
		NewSound({ID = 171140306,PARENT = ROOT,VOLUME = 1,PITCH = MRANDOM(9,11)/10,LOOP = false,MAXDISTANCE = 75,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
	end
end

function MeleeCombo()
	ATTACKING = true
	HUM.WalkSpeed = 7
	HUM.JumpPower = 0
	local MELEEAREA = function(BEEF,KNOCKBACK)
		local DIDHIT = false
		NewSound({ID = 153647549,PARENT = ROOT,VOLUME = 1,PITCH = MRANDOM(8,12)/10,LOOP = false,MAXDISTANCE = 125,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
		for index, CHILD in pairs(workspace:GetChildren()) do
			if CHILD:FindFirstChildOfClass("Humanoid") and CHILD ~= CHARACTER then
				local HUMAN = CHILD:FindFirstChildOfClass("Humanoid")
				local TORS = CHILD:FindFirstChild("Torso") or CHILD:FindFirstChild("UpperTorso")
				if TORS then
					if (TORS.Position - ROOT.CFrame*CF(0,0,-1.5).p).Magnitude <= 3.25 then
						DIDHIT = true
						NewSound({ID = 2330778973,PARENT = TORS,VOLUME = 3,PITCH = MRANDOM(8,12)/10,LOOP = false,MAXDISTANCE = 125,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
						HUMAN.Health = HUMAN.Health - BEEF
						local BV = IT("BodyVelocity")
						BV.MaxForce = BV.MaxForce * 500
						BV.Velocity = CF(ROOT.Position,TORS.Position+VT(0,0.5,0)).lookVector*(KNOCKBACK+(BEEF/2))
						BV.Parent = TORS
						Debris:AddItem(BV,0.05)
						OofOuchBlood(TORS.Position,ROOT.Position,math.ceil(BEEF/4))
						if HUMAN.Health <= 0 then
							ManSlaughter(CHILD)
						end
					end
				end
			end
		end
		if DIDHIT == true then
			CameraShake(ROOT.CFrame*CF(0,0,-1.5).p,4,5,1)
		end
	end
	local GYRO = IT("BodyGyro")
	GYRO.D = 20
	GYRO.P = 5000
	GYRO.MaxTorque = VT(0,4000000,0)
	GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
	GYRO.Parent = ROOT
	coroutine.resume(coroutine.create(function()
		repeat
			Swait()
			GYRO.CFrame = CF(ROOT.Position,MOUSE.Hit.p)
			if COMBO ~= 3 then
				if STATE == "Pistol" then
					RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(10)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
					--LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-10 + 2.5 * SIN(SINE / 12))) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
				elseif STATE == "Shotgun" then
					RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0, 0.3) * ANGLES(RAD(65), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
				--LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.25, 0.45, 0.2) * ANGLES(RAD(45), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
				end
			end
		until ATTACKING == false
		GYRO:Remove()
	end))
	if COMBO == 1 then
		COMBO = 2
		for i=0, 0.2, 0.1 / ANIM_SPEED do
			Swait()
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, -0.1) * ANGLES(RAD(-30), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(32), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(-10), RAD(0), RAD(0)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -0.5, -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(-45)), 2 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(60)), 0.5 / ANIM_SPEED)
		end
		MELEEAREA(10,7)
		for i=0, 0.35, 0.1 / ANIM_SPEED do
			Swait()
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, -0.1) * ANGLES(RAD(-40), RAD(0), RAD(0)), 1 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(32), RAD(0), RAD(0)), 1 / ANIM_SPEED)
			RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
			LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(0)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(70)), 2.5 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(70)), 1 / ANIM_SPEED)
		end
	elseif COMBO == 2 then
		COMBO = 3
		for i=0, 0.15, 0.1 / ANIM_SPEED do
			Swait()
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(35)), 1 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(-35)), 1 / ANIM_SPEED)
			LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0.4) * ANGLES(RAD(90), RAD(0), RAD(-45)) * LEFTSHOULDERC0, 1 / ANIM_SPEED)
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(55), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / ANIM_SPEED)
		end
		MELEEAREA(15,15)
		for i=0, 0.2, 0.1 / ANIM_SPEED do
			Swait()
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-25)), 2 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(25)), 1 / ANIM_SPEED)
			LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, -0.5) * ANGLES(RAD(90), RAD(0), RAD(15)) * LEFTSHOULDERC0, 2 / ANIM_SPEED)
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 2 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-65), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 2 / ANIM_SPEED)
		end
	elseif COMBO == 3 then
		if GRIP.Parent == RIGHTARM or STATE == "Shotgun" then
			for i=0, 0.3, 0.1 / ANIM_SPEED do
				Swait()
				ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-45)), 1.5 / ANIM_SPEED)
				NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(10), RAD(0), RAD(45)), 0.5 / ANIM_SPEED)
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.35, 0.5, -0.5) * ANGLES(RAD(0), RAD(0), RAD(90)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-15)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
				RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(85), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-57), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			end
			MELEEAREA(35,5)
			for i=0, 0.3, 0.1 / ANIM_SPEED do
				Swait()
				ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(25)), 1.5 / ANIM_SPEED)
				NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(10), RAD(0), RAD(-25)), 0.5 / ANIM_SPEED)
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.35, 0.5, -0.5) * ANGLES(RAD(0), RAD(0), RAD(90)) * ANGLES(RAD(160), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-15)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
				RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(65), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			end
		else
			for i=0, 0.15, 0.1 / ANIM_SPEED do
				Swait()
				ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-45)), 1.5 / ANIM_SPEED)
				NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(10), RAD(0), RAD(45)), 0.5 / ANIM_SPEED)
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.35, 0.5, -0.5) * ANGLES(RAD(0), RAD(0), RAD(90)) * RIGHTSHOULDERC0, 1.5 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-15)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
				RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(85), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-57), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			end
			MELEEAREA(10,17)
			for i=0, 0.3, 0.1 / ANIM_SPEED do
				Swait()
				ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(25)), 1.5 / ANIM_SPEED)
				NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(10), RAD(0), RAD(-25)), 0.5 / ANIM_SPEED)
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.35, 0.5, -0.5) * ANGLES(RAD(0), RAD(0), RAD(90)) * ANGLES(RAD(160), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 1 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-15)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
				RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(65), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			end
		end
		COMBO = 1
	end
	ATTACKING = false
	HUM.WalkSpeed = 13
	HUM.JumpPower = 50
end

function Be_A_Dick(KEY)
	HUM.WalkSpeed = 0
	HUM.JumpPower = 0
	ATTACKING = true
	if KEY == "t" then
		NewSound({ID = 1535995263,PARENT = HEAD,VOLUME = 8,PITCH = 1,LOOP = false,MAXDISTANCE = 125,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
		for i = 1, 70 do
			Swait()
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(-20), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			if STATE == "Pistol" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(-10), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
			elseif STATE == "Shotgun" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0, 0.1) * ANGLES(RAD(50), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
			end
			LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-0.6, 0.25, -1) * ANGLES(RAD(155 + 30 * COS(i / 4)), RAD(0), RAD(15)) * CF(0,-0.25,0) * ANGLES(RAD(0), RAD(90), RAD(0)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(80), RAD(0)) * ANGLES(RAD(2), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(2), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
		end
	elseif KEY == "y" then
		NewSound({ID = 1535994669,PARENT = HEAD,VOLUME = 8,PITCH = 1,LOOP = false,MAXDISTANCE = 125,EMITTERSIZE = 15,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
		for i = 1, 70 do
			Swait()
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(40)), 0.5 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(-20), RAD(0), RAD(-40)), 0.5 / ANIM_SPEED)
			if STATE == "Pistol" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(-10), RAD(20), RAD(0)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
			elseif STATE == "Shotgun" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0, 0.1) * ANGLES(RAD(50), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
			end
			LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, -0.1) * ANGLES(RAD(90), RAD(0), RAD(40)) * ANGLES(RAD(0), RAD(-45), RAD(0)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(40), RAD(0)) * ANGLES(RAD(2), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(2), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
		end
	end
	ATTACKING = false
	HUM.WalkSpeed = 13
	HUM.JumpPower = 50
end

--//====================================================\\--
--||                       WRAP
--\\====================================================//--
MOUSE.Button1Down:connect(function ()
FireGun()
end)
MOUSE.KeyDown:Connect(function(V2)

					if V2 == "z" then
						GunThrow()
					elseif V2 == "q" then
						if HUM.WalkSpeed <= 15 then
							HUM.WalkSpeed = 35
						else
							HUM.WalkSpeed = 13
						end
					elseif V2 == "x" then
						Grenade()
					elseif V2 == "e" then
						if ROOT:FindFirstChild("BGM_MUSIC") then
							ROOT:FindFirstChild("BGM_MUSIC"):Remove()
						else
							local M = NewSound({ID = 2128308112,PARENT = ROOT,VOLUME = 1.5,PITCH = 1,LOOP = true,MAXDISTANCE = 300,EMITTERSIZE = 300,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
							M.Name = "BGM_MUSIC"
						end
					elseif V2 == "c" then
						MeleeCombo()
					elseif V2 == "f" then
						SwitchGuns()
					elseif V2 == "t" or V2 == "y" then
						Be_A_Dick(V2)
					end
end)

local M = NewSound({ID = 2128308112,PARENT = ROOT,VOLUME = 1.5,PITCH = 1,LOOP = true,MAXDISTANCE = 300,EMITTERSIZE = 300,PLAYING = true,PLAYONREMOVE = false,DOESDEBRIS = true})
M.Name = "BGM_MUSIC"

HUM.WalkSpeed = 13
 
while true do
	Swait()
	SINE = SINE + CHANGE
	if CHARACTER:FindFirstChild("Animate") then
		CHARACTER:FindFirstChild("Animate"):Destroy()
	end
	if CHARACTER:FindFirstChild("Sound") then
		CHARACTER:FindFirstChild("Sound"):Destroy()
	end
	for _,v in next, HUM:GetPlayingAnimationTracks() do
		v:Stop();
	end
	local TORSOVELOCITY = (ROOT.Velocity * VT(1, 0, 1)).magnitude
	local TORSOVERTICALVELOCITY = ROOT.Velocity.y
	local HITFLOOR = Raycast(ROOT.Position, (CF(ROOT.Position, ROOT.Position + VT(0, -1, 0))).lookVector, 4+HUM.HipHeight, CHARACTER)
	local WALKSPEEDVALUE = 7-(2*(HUM.WalkSpeed/16))
	if WALKSPEEDVALUE <= 3 then
		WALKSPEEDVALUE = 3
	end
	local SITTING = HUM.Sit
	if ANIM == "Walk" and TORSOVELOCITY > 1 and ATTACKING == false then
		ROOTJOINT.C1 = Clerp(ROOTJOINT.C1, ROOTC0 * CF(0, 0, -0.05 * COS(SINE / (WALKSPEEDVALUE / 2))) * ANGLES(RAD(0), RAD(0) - ROOT.RotVelocity.Y / 35, RAD(0)), 2 * (HUM.WalkSpeed / 16) / ANIM_SPEED)
		NECK.C1 = Clerp(NECK.C1, CF(0, -0.5, 0) * ANGLES(RAD(-90), RAD(0), RAD(180)) * ANGLES(RAD(2.5 * SIN(SINE / (WALKSPEEDVALUE / 2))), RAD(0), RAD(0) - HEAD.RotVelocity.Y / 30), 0.2 * (HUM.WalkSpeed / 16) / ANIM_SPEED)
		RIGHTHIP.C1 = Clerp(RIGHTHIP.C1, CF(0.5, 0.875 - 0.3 * SIN(SINE / WALKSPEEDVALUE), -0.5 * COS(SINE / WALKSPEEDVALUE) +0.2+ 0.2 * COS(SINE / WALKSPEEDVALUE)) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0) - RIGHTLEG.RotVelocity.Y / 35, RAD(0), RAD((35+HUM.WalkSpeed) * COS(SINE / WALKSPEEDVALUE))), 2 / ANIM_SPEED)
		LEFTHIP.C1 = Clerp(LEFTHIP.C1, CF(-0.5, 0.875 + 0.3 * SIN(SINE / WALKSPEEDVALUE), 0.5 * COS(SINE / WALKSPEEDVALUE) +0.2+ -0.2 * COS(SINE / WALKSPEEDVALUE)) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0) + LEFTLEG.RotVelocity.Y / 35, RAD(0), RAD((35+HUM.WalkSpeed) * COS(SINE / WALKSPEEDVALUE))), 2 / ANIM_SPEED)
	elseif (ANIM ~= "Walk") or (TORSOVELOCITY < 1) or ATTACKING == true then
		ROOTJOINT.C1 = Clerp(ROOTJOINT.C1, ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.2 / ANIM_SPEED)
		NECK.C1 = Clerp(NECK.C1, CF(0, -0.5, 0) * ANGLES(RAD(-90), RAD(0), RAD(180)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.2 / ANIM_SPEED)
		RIGHTHIP.C1 = Clerp(RIGHTHIP.C1, CF(0.5, 1, 0) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.2 / ANIM_SPEED)
		LEFTHIP.C1 = Clerp(LEFTHIP.C1, CF(-0.5, 1, 0) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.2 / ANIM_SPEED)
	end
	if SITTING == false then
		if HITFLOOR then
			if TORSOVELOCITY < 1 and HITFLOOR ~= nil then
				ANIM = "Idle"
				if ATTACKING == false then
					ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, -0.02 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(15)), 0.5 / ANIM_SPEED)
					NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(25 - 2.5 * SIN(SINE / 12)), RAD(15), RAD(-20)), 0.5 / ANIM_SPEED)
					if STATE == "Pistol" then
						RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(10 - 2.5 * SIN(SINE / 12))) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
						LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-10 + 2.5 * SIN(SINE / 12))) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
					elseif STATE == "Shotgun" then
						RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.1, 0, 0.3) * ANGLES(RAD(75), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
						LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-0.25, -0.175, -1) * ANGLES(RAD(75), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
					end
					RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(65), RAD(0)) * ANGLES(RAD(-5), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
					LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(-5), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
				end
			elseif TORSOVELOCITY > 1 and HITFLOOR ~= nil then
				ANIM = "Walk"
				if ATTACKING == false then
					ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, -0.05) * ANGLES(RAD(HUM.WalkSpeed/2), RAD(0), RAD(15*COS(SINE / WALKSPEEDVALUE))), 0.25 / ANIM_SPEED)
					NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(15-HUM.WalkSpeed/2 - 8 * SIN(SINE / (WALKSPEEDVALUE / 2))), RAD(0), RAD(-15*COS(SINE / WALKSPEEDVALUE))), 0.25 / ANIM_SPEED)
					if STATE == "Pistol" then
						RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(35 * COS(SINE / WALKSPEEDVALUE)), RAD(0), RAD(5)) * RIGHTSHOULDERC0, 0.75 / ANIM_SPEED)
						LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(-35 * COS(SINE / WALKSPEEDVALUE)), RAD(0), RAD(-5)) * LEFTSHOULDERC0, 0.75 / ANIM_SPEED)
					elseif STATE == "Shotgun" then
						RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.1, 0, 0.3) * ANGLES(RAD(60), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
						LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-0.25, -0.25, -1) * ANGLES(RAD(60), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
					end
					RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1 , -1, 0) * ANGLES(RAD(0), RAD(90-15*COS(SINE / WALKSPEEDVALUE)), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(-15)), 0.25 / ANIM_SPEED)
					LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, 0) * ANGLES(RAD(0), RAD(-90-15*COS(SINE / WALKSPEEDVALUE)), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(15)), 0.25 / ANIM_SPEED)
				end
			end
		else
			if TORSOVERTICALVELOCITY > 0 then
				ANIM = "Jump"
				if ATTACKING == false then
					ROOTJOINT.C0 = Clerp(ROOTJOINT.C0, ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
					NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(-20), RAD(0), RAD(0)), 0.2 / ANIM_SPEED)
					if STATE == "Pistol" then
						RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-10 - 2.5 * SIN(SINE / 12))) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
						LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(10 + 2.5 * SIN(SINE / 12))) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
					elseif STATE == "Shotgun" then
						RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.1, 0, 0.3) * ANGLES(RAD(90), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
						LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-0.25, 0, -1) * ANGLES(RAD(90), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
					end
					RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -0.9, -0.3) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(-20)), 0.5 / ANIM_SPEED)
					LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, -0.3) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(20)), 0.5 / ANIM_SPEED)
			    end
			else
			ANIM = "Fall"
				if ATTACKING == false then
					ROOTJOINT.C0 = Clerp(ROOTJOINT.C0, ROOTC0 * CF(0, 0, 0 ) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / ANIM_SPEED)
					NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0 , 0 + ((1) - 1)) * ANGLES(RAD(20), RAD(0), RAD(0)), 0.2 / ANIM_SPEED)
					if STATE == "Pistol" then
						RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(50 - 2.5 * SIN(SINE / 12))) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
						LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-50 + 2.5 * SIN(SINE / 12))) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
					elseif STATE == "Shotgun" then
						RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.1, 0, 0.3) * ANGLES(RAD(90), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
						LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-0.25, 0, -1) * ANGLES(RAD(90), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
					end
					RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -0.5, -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(20)), 0.2 / ANIM_SPEED)
					LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -1, 0) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(10)), 0.2 / ANIM_SPEED)
				end
			end
		end
	else
		ANIM = "Sit"
		if ATTACKING == false then
			ROOTJOINT.C0 = Clerp(ROOTJOINT.C0,ROOTC0 * CF(0, 0, -0.5) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.25 / ANIM_SPEED)
			NECK.C0 = Clerp(NECK.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1.25 / ANIM_SPEED)
			if STATE == "Pistol" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.5, 0.65, 0) * ANGLES(RAD(50), RAD(10), RAD(-45))*CF(0,-0.25,0) * RIGHTSHOULDERC0, 1.25 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-1.5, 0.65, 0) * ANGLES(RAD(50), RAD(-10), RAD(45))*CF(0,-0.25,0) * LEFTSHOULDERC0, 1.25 / ANIM_SPEED)
			elseif STATE == "Shotgun" then
				RIGHTSHOULDER.C0 = Clerp(RIGHTSHOULDER.C0, CF(1.1, 0, 0.3) * ANGLES(RAD(90), RAD(0), RAD(-5)) * RIGHTSHOULDERC0, 0.5 / ANIM_SPEED)
				LEFTSHOULDER.C0 = Clerp(LEFTSHOULDER.C0, CF(-0.25, 0, -1) * ANGLES(RAD(90), RAD(0), RAD(65)) * LEFTSHOULDERC0, 0.5 / ANIM_SPEED)
			end
			RIGHTHIP.C0 = Clerp(RIGHTHIP.C0, CF(1, -0.25, -1) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(10)), 1.25 / ANIM_SPEED)
			LEFTHIP.C0 = Clerp(LEFTHIP.C0, CF(-1, -0.25, -1) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(-10)), 1.25 / ANIM_SPEED)
		end
	end
	if MRANDOM(1,55) == 1 then
		NECK.C0 = NECK.C0 * ANGLES(RAD(MRANDOM(-5,5)/2), RAD(MRANDOM(-5,5)/2), RAD(MRANDOM(-5,5)/2))
	end
end
