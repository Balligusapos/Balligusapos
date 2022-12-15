-- // Logins: // --

local Usernames = {
["yamete-uwu"] = true;
}



-- // Variables: // --

local Login = game.CoreGui.Login

local Key = Login.Main.WhitelistFrame.Key

local Username = Login.Main.UserFrame.UserBox

local Userpassed = false

local WLPassed = false



-- // Login Function: // --

if Usernames[Username.Text] then
Userpassed = true
else
game.Players.LocalPlayer:Kick("dumbass! Wrong key")
end




if Userpassed == true then
if WLPassed == true then
for i,v in pairs(game.CoreGui:GetDescendants()) do
 if v.Name == "Main" then
  v:Destroy()
 end
end
loadstring(game:HttpGet('https://raw.githubusercontent.com/Balligusapos/Balligusapos/main/robloxs-obfuscated'))()
end
end
