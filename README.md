# All The Script is made by Maska

# Change any pets

```lua
local Petss = "Jolly Moose" -- The pet you want to change


local newpetname = "Nameofthepet" 
local rarity = "Legendary" -- Basic, Rare, Epic, Legendary, Mythical, Exclusive
local type = "Huge"-- Normal, Huge, Titanic, HatchHuge, HatchTitanic
local strengthMin = 1
local strengthMax = 32
local sounds = 4478156615
local random = 4478156278
local isVanity = true
local isPremium = true
local tradeable = true
local fly = true
local MeshID = "" 
local TextureID = ""
local GTextureID = ""
local thumbnail = ""
local goldenThumbnail = ""
local darkMatterThumbnail = ""





-- don't change the script after this 




_G.Petname = ""
_G.PetRemote = ""

for i, v in pairs(game:GetService("ReplicatedStorage").Game.Pets:GetDescendants()) do
	if v.name == ("Pet Data ("..Petss..")") and v.Parent then
	    print(v.Parent.Name)
		Petname = v.Parent.Name
		PetRemote = v.name
	end
end

local gunstatesmodule = game:GetService("ReplicatedStorage").Game.Pets[Petname][PetRemote]
local m = require(gunstatesmodule);

local goldeee = game:GetService("ReplicatedStorage").Game.Pets[Petname].Golden.Mesh
local changepets = game:GetService("ReplicatedStorage").Game.Pets[Petname].Pet.Mesh


m.name = newpetname
m.rarity = rarity
m.strengthMin = strengthMin
m.strengthMax = strengthMax
m.sounds = sounds
m.random = random

m.isVanity = isVanity
m.isPremium = isPremium
m.tradeable = tradeable
m.fly = fly


m.MeshID = MeshID
m.TextureID = TextureID


m.thumbnail = thumbnail
m.goldenThumbnail = goldenThumbnail
m.darkMatterThumbnail = darkMatterThumbnail


changepets.MeshId = MeshID
changepets.TextureId = TextureID
goldeee.MeshId = MeshID
goldeee.TextureId = GTextureID


    if PetType == "Normal" then 
    m.huge = false
	m.titanic = false
    changepets.Scale = Vector3.new(0.75, 0.75, 0.75)
    changepets.Offset = Vector3.new(0,0,0) 
    goldeee.Scale = Vector3.new(0.75, 0.75, 0.75)
    goldeee.Offset = Vector3.new(0,0,0)

	        elseif PetType == "Huge" then
	m.huge = true
	m.titanic = false
    changepets.Scale = Vector3.new(1.6, 1.6, 1.6) 
    changepets.Offset = Vector3.new(0, 2, 0) 
	goldeee.Scale = Vector3.new(1.6, 1.6, 1.6) 
    goldeee.Offset = Vector3.new(0, 2, 0)
	        
			elseif PetType == "Titanic" then
	m.huge = true
	m.titanic = true			
	changepets.Scale = Vector3.new(6, 6, 6) 
    changepets.Offset = Vector3.new(0, 9, 4) 
	goldeee.Scale = Vector3.new(6, 6, 6) 
    goldeee.Offset = Vector3.new(0, 9, 4)

			elseif PetType == "HatchHuge" then
	m.huge = true
	m.titanic = false
	changepets.Scale = Vector3.new(1.6, 1.6, 1.6) 
    changepets.Offset = Vector3.new(0,0,0) 
    goldeee.Scale = Vector3.new(1.6, 1.6, 1.6) 
    goldeee.Offset = Vector3.new(0,0,0)

			elseif PetType == "HatchTitanic" then
	m.huge = true
	m.titanic = true
	changepets.Scale = Vector3.new(6, 6, 6) 
    changepets.Offset = Vector3.new(0, 0, 0) 
	goldeee.Scale = Vector3.new(6, 6, 6) 
    goldeee.Offset = Vector3.new(0, 0, 0) 
			end
```

# Gampass Price
```lua
local gunstatesmodule = game:GetService("ReplicatedStorage").Directory.Gamepasses.Gamepasses
local m = require(gunstatesmodule);

gamepassid = 18674288

m.Hoverboard = gamepassid
m["8 Pets Equipped"] = gamepassid
m.Teleport = gamepassid
m.Hoverboard = gamepassid
m.VIP = gamepassid
m["Triple Egg Open"] = gamepassid
m["Skip Egg Open"] = gamepassid
m["Pet Storage"] = gamepassid
m["Super Pet Storage"] = gamepassid
m["Auto Hatch"] = gamepassid
m.Lucky = gamepassid
m["Mythical Hunter"] = gamepassid
m["Magic Eggs"] = gamepassid
m.Magnet = gamepassid
m["Shiny Hunter"] = gamepassid
```

