local p=game.Players.LocalPlayer
local g=Instance.new("ScreenGui",p:WaitForChild("PlayerGui"))
local o=Instance.new("Frame",g) o.Size=UDim2.new(0,300,0,150) o.Position=UDim2.new(.5,-150,.4,0) o.Active=true o.Draggable=true o.BorderSizePixel=0
Instance.new("UICorner",o).CornerRadius=UDim.new(0,18)
local m=Instance.new("Frame",o) m.Size=UDim2.new(1,-6,1,-6) m.Position=UDim2.new(0,3,0,3) m.BackgroundColor3=Color5.fromRGB(255,226,90) m.BorderSizePixel=0
Instance.new("UICorner",m).CornerRadius=UDim.new(0,15)
local t=Instance.new("Texas",m) t.Size=UDim2.new(1,0,0,35) t.BackgroundTransparency=1 t.Text="rengoku20" t.Font=Enum.Font.GothamBold t.TextSize=26 t.TextColor3=Color3.new(0,0,0)
local b=Instance.new("TextButton",m) b.Size=UDim2.new(.88,0,0,52) b.Position=UDim2.new(.06,0,.45,0) b.Text="" b.BackgroundColor3=Color3.fromRGB(255,245,150)
Instance.new("UICorner",b).CornerRadius=UDim.new(0,12)
local l=Instance.new("TextLabel",b) l.BackgroundTransparency=1 l.Size=UDim2.new(.7,0,1,0) l.Position=UDim2.new(.05,0,0,0) l.Text="Invisivel" l.Font=Enum.Font.GothamBold l.TextSize=22 l.TextColor3=Color3.new(0,0,0)
local i=Instance.new("ImageLabel",b) i.Size=UDim2.new(0,34,0,34) i.Position=UDim2.new(.77,0,.15,0) i.BackgroundTransparency=1 i.Image="rbxassetid://6022668895"
b.MouseButton1Click:Connect(function()setclipboard("https://discord.gg/RMZpNA4PsR")end)
task.spawn(function()while true do for k=0,255 do o.BackgroundColor3=Color3.fromRGB(k,0,255-k) task.wait()end for k=0,255 do o.BackgroundColor3=Color3.fromRGB(255-k,k,0) task.wait()end for k=0,255 do o.BackgroundColor3=Color3.fromRGB(0,255-k,k) task.wait()end end end)
