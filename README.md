local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

Rayfield:LoadConfiguration()
local Window = Rayfield:CreateWindow({
	Name = "tubergamer(beta)",
	Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
	LoadingTitle = "Rayfield Interface Suite",
	LoadingSubtitle = "by Sirius",
	Theme = "Ocean", -- Check https://docs.sirius.menu/rayfield/configuration/themes
 
	DisableRayfieldPrompts = false,
	DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface
 
	ConfigurationSaving = {
	   Enabled = true,
	   FolderName = nil, -- Create a custom folder for your hub/game
	   FileName = "Big Hub"
	},
 
	Discord = {
	   Enabled = false, -- Prompt the user to join your Discord server if their executor supports it
	   Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ ABCD would be ABCD
	   RememberJoins = true -- Set this to false to make them join the discord every time they load it up
	},
 
	KeySystem = false, -- Set this to true to use our key system
	KeySettings = {
	   Title = "tuber hub",
	   Subtitle = "script-modded",
	   Note = "tuber key (patchet key)(new key admin-modded)", -- Use this to tell the user how to get a key
	   FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
	   SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
	   GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
	   Key = {"admin-modded"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
	}
 })



 local Tab = Window:CreateTab("blade ball", 4483362458) -- Title, Image
 local TabMisc= Window:CreateTab("misc", 4483362458)
 local TabCre= Window:CreateTab("Credits", 4483362458)

 local Button = Tab:CreateButton({
	Name = "auto parry (beta)",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/kauepsantos/blade_ball/refs/heads/main/README.md"))()
 })

 local Label = TabCre:CreateLabel("credits")

local Button = Tab:CreateButton({
	Name = "destruir",
	Callback = function()
		Rayfield:Destroy()
	end,
 })

 Rayfield:LoadConfiguration()
