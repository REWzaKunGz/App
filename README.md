if game.PlaceId == 2753915549 or game.PlaceId == 4442272183 or game.PlaceId == 7449423635 or game.PlaceId == 2768379856 or game.PlaceId == 537413528 or game.PlaceId == 5780309044 or game.PlaceId == 1240123653 or game.PlaceId == 1240123653 or game.PlaceId == 1632210982 or game.PlaceId == 662417684 or game.PlaceId == 4520749081 or game.PlaceId == 4580204640 or game.PlaceId == 5780309044 or game.PlaceId == 13621938427 or game.PlaceId == 11423467063 then
			local JoinServer = 'game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId,'..'\''..tostring(game.JobId)..'\''..')'
			local GameTime = math.floor(workspace.DistributedGameTime+0.5)
			local Hour = math.floor(GameTime/(60^2))%24
			local Minute = math.floor(GameTime/(60^1))%60
			local Second = math.floor(GameTime/(60^0))%60
			local url =
			   "https://discord.com/api/webhooks/1185446950120722442/I098evfd3XbbOa91dNIlaJRqVXst2Ns1Aj82ZLbGb4sh5JbxwAsVxeKyGoO4Xm4TxVTI"
			local data = {
			   ["content"] = "",
			   ["embeds"] = {
				   {
					   ["title"] = "**Someone Executed Script**",
					   ["description"] = '```\nNAME USER : '..game:GetService("Players").LocalPlayer.Name..'\nGAME NAME : '..game:GetService("MarketplaceService"):GetProductInfo(game.PlaceId).Name..'\nEXECUTER TIME :'..'\nHours : '..os.date("%H")..'| Minute : '..os.date("%M")..'| Second : '..os.date("%S")..'``````'..JoinServer..'```',           
					   ["type"] = "rich",								
					   ["color"] = tonumber(0x7269da),
				   }
			   }
			}
			local newdata = game:GetService("HttpService"):JSONEncode(data)
			local headers = {
			   ["content-type"] = "application/json"
			}
			local abcdef = {Url = url, Body = newdata, Method = "POST", Headers = headers}
			request(abcdef)
			
			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()		
			wait(1)
			Notification:Notify(
				{Title = "Pado Hub", Description = "Game : " .. (tostring(game:GetService("MarketplaceService"):GetProductInfo(game.PlaceId).Name))},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
			)
			wait(0.5)
			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()		
			wait(1)
			Notification:Notify(
				{Title = "Pado Hub", Description = "Loading ..."},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
			)
		else
			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()		
			wait(1)
			Notification:Notify(
				{Title = "Pado Hub", Description = "This game is not available in the system."},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
			)
		end

		if game.PlaceId == 2753915549 or game.PlaceId == 4442272183 or game.PlaceId == 7449423635 then

			spawn(function()
				while wait() do
					if game.Players.LocalPlayer.Team == nil then
						pcall(function()
							if getgenv().Team == "Pirate" then
								game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton.Size = UDim2.new(10000,1000,10000,1000)
								game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton.Position = UDim2.new(-4,0,-5,0)
								wait(.5)
								game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,true,game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton,0)
								game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,false,game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton,0)
							elseif getgenv().Team == "Marine" then
								game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Marines.Frame.ViewportFrame.TextButton.Size = UDim2.new(10000,1000,10000,1000)
								game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Marines.Frame.ViewportFrame.TextButton.Position = UDim2.new(-4,0,-5,0)
								wait(.5)
								game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,true,game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton,0)
								game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,false,game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton,0)
							else
								game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton.Size = UDim2.new(10000,1000,10000,1000)
								game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton.Position = UDim2.new(-4,0,-5,0)
								wait(.5)
								game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,true,game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton,0)
								game:GetService("VirtualInputManager"):SendMouseButtonEvent(605,394,0,false,game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.ViewportFrame.TextButton,0)
							end
						end)
					end
				end
			end)
			
				local notifSound = Instance.new("Sound",workspace)
				notifSound.PlaybackSpeed = 1.5
				notifSound.Volume = 0.15
				notifSound.SoundId = "rbxassetid://170765130"
				notifSound.PlayOnRemove = true
				notifSound:Destroy()

		if game.PlaceId == 2753915549 then
				World1 = true
			elseif game.PlaceId == 4442272183 then
				World2 = true
			elseif game.PlaceId == 7449423635 then
				World3 = true
			end
			
			function CheckLevel() 
				local MyLevel = game.Players.LocalPlayer.Data.Level.Value
				if World1 then
					if MyLevel == 1 or MyLevel <= 9 or _G.SelectMonster == "Bandit" then -- Bandit
						Ms = "Bandit"
						NameQuest = "BanditQuest1"
						LevelQuest = 1
						NameMon = "Bandit"
						CFrameQuest = CFrame.new(1061.66699, 16.5166187, 1544.52905, -0.942978859, -3.33851502e-09, 0.332852632, 7.04340497e-09, 1, 2.99841325e-08, -0.332852632, 3.06188177e-08, -0.942978859)
						CFrameMon = CFrame.new(1199.31287, 52.2717781, 1536.91516, -0.929782331, 6.60215846e-08, -0.368109822, 3.9077392e-08, 1, 8.06501603e-08, 0.368109822, 6.06023249e-08, -0.929782331)
						SPAWNPOINT = "Default"
					elseif MyLevel == 10 or MyLevel <= 14 or _G.SelectMonster == "Monkey" then -- Monkey
						Ms = "Monkey"
						NameQuest = "JungleQuest"
						LevelQuest = 1
						NameMon = "Monkey"
						CFrameQuest = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
						CFrameMon = CFrame.new(-1502.74609, 98.5633316, 90.6417007, 0.836947978, 0, 0.547282517, -0, 1, -0, -0.547282517, 0, 0.836947978)
						SPAWNPOINT = "Jungle"
					elseif MyLevel == 15 or MyLevel <= 29 or _G.SelectMonster == "Gorilla" then -- Gorilla
						Ms = "Gorilla"
						NameQuest = "JungleQuest"
						LevelQuest = 2
						NameMon = "Gorilla"
						CFrameQuest = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
						CFrameMon = CFrame.new(-1223.52808, 6.27936459, -502.292664, 0.310949147, -5.66602516e-08, 0.950426519, -3.37275488e-08, 1, 7.06501808e-08, -0.950426519, -5.40241736e-08, 0.310949147)
						SPAWNPOINT = "Jungle"
					elseif MyLevel == 30 or MyLevel <= 39 or _G.SelectMonster == "Pirate" then -- Pirate
						Ms = "Pirate"
						NameQuest = "BuggyQuest1"
						LevelQuest = 1
						NameMon = "Pirate"
						CFrameQuest = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
						CFrameMon = CFrame.new(-1219.32324, 4.75205183, 3915.63452, -0.966492832, -6.91238853e-08, 0.25669381, -5.21195496e-08, 1, 7.3047012e-08, -0.25669381, 5.72206496e-08, -0.966492832)
						SPAWNPOINT = "Pirate"
					elseif MyLevel == 40 or MyLevel <= 59 or _G.SelectMonster == "Brute" then -- Brute
						Ms = "Brute"
						NameQuest = "BuggyQuest1"
						LevelQuest = 2
						NameMon = "Brute"
						CFrameQuest = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
						CFrameMon = CFrame.new(-1146.49646, 96.0936813, 4312.1333, -0.978175163, -1.53222057e-08, 0.207781896, -3.33316912e-08, 1, -8.31738873e-08, -0.207781896, -8.82843523e-08, -0.978175163)
						SPAWNPOINT = "Pirate"
					elseif MyLevel == 60 or MyLevel <= 74 or _G.SelectMonster == "Desert Bandit" then -- Desert Bandit
						Ms = "Desert Bandit"
						NameQuest = "DesertQuest"
						LevelQuest = 1
						NameMon = "Desert Bandit"
						CFrameQuest = CFrame.new(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
						CFrameMon = CFrame.new(932.788818, 6.4503746, 4488.24609, -0.998625934, 3.08948351e-08, 0.0524050146, 2.79967303e-08, 1, -5.60361286e-08, -0.0524050146, -5.44919629e-08, -0.998625934)
						SPAWNPOINT = "Desert"
					elseif MyLevel == 75 or MyLevel <= 89 or _G.SelectMonster == "Desert Officer" then -- Desert Officre
						Ms = "Desert Officer"
						NameQuest = "DesertQuest"
						LevelQuest = 2
						NameMon = "Desert Officer"
						CFrameQuest = CFrame.new(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
						CFrameMon = CFrame.new(1580.03198, 4.61375761, 4366.86426, 0.135744005, -6.44280718e-08, -0.990743816, 4.35738308e-08, 1, -5.90598574e-08, 0.990743816, -3.51534837e-08, 0.135744005)
						SPAWNPOINT = "Desert"
					elseif MyLevel == 90 or MyLevel <= 99 or _G.SelectMonster == "Snow Bandit" then -- Snow Bandits
						Ms = "Snow Bandit"
						NameQuest = "SnowQuest"
						LevelQuest = 1
						NameMon = "Snow Bandits"
						CFrameQuest = CFrame.new(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
						CFrameMon = CFrame.new(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
						SPAWNPOINT = "Ice"
					elseif MyLevel == 100 or MyLevel <= 119 or _G.SelectMonster == "Snowman"  then -- Snowman
						Ms = "Snowman"
						NameQuest = "SnowQuest"
						LevelQuest = 2
						NameMon = "Snowman"
						CFrameQuest = CFrame.new(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
						CFrameMon = CFrame.new(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
						SPAWNPOINT = "Ice"
					elseif MyLevel == 120 or MyLevel <= 149 or _G.SelectMonster == "Chief Petty Officer" then -- Chief Petty Officer
						Ms = "Chief Petty Officer"
						NameQuest = "MarineQuest2"
						LevelQuest = 1
						NameMon = "Chief Petty Officer"
						CFrameQuest = CFrame.new(-5035.0835, 28.6520386, 4325.29443, 0.0243340395, -7.08064647e-08, 0.999703884, -6.36926814e-08, 1, 7.23777944e-08, -0.999703884, -6.54350671e-08, 0.0243340395)
						CFrameMon = CFrame.new(-4882.8623, 22.6520386, 4255.53516, 0.273695946, -5.40380647e-08, -0.96181643, 4.37720793e-08, 1, -4.37274998e-08, 0.96181643, -3.01326679e-08, 0.273695946)
						SPAWNPOINT = "MarineBase"
					elseif MyLevel == 150 or MyLevel <= 174 or _G.SelectMonster == "Sky Bandit" then -- Sky Bandit
						Ms = "Sky Bandit"
						NameQuest = "SkyQuest"
						LevelQuest = 1
						NameMon = "Sky Bandit"
						CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
						CFrameMon = CFrame.new(-4970.74219, 294.544342, -2890.11353, -0.994874597, -8.61311236e-08, -0.101116329, -9.10836206e-08, 1, 4.43614923e-08, 0.101116329, 5.33441664e-08, -0.994874597)
						SPAWNPOINT = "Sky"
					elseif MyLevel == 175 or MyLevel <= 189 or _G.SelectMonster == "Dark Master" then -- Dark Master
						Ms = "Dark Master"
						NameQuest = "SkyQuest"
						LevelQuest = 2
						NameMon = "Dark Master"
						CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
						CFrameMon = CFrame.new(-5220.58594, 430.693298, -2278.17456, -0.925375521, 1.12086873e-08, 0.379051805, -1.05115507e-08, 1, -5.52320891e-08, -0.379051805, -5.50948407e-08, -0.925375521)
						SPAWNPOINT = "Sky"
					elseif MyLevel == 190 or MyLevel <= 209 or _G.SelectMonster == "Prisoner" then
						Ms = "Prisoner"
						NameQuest = "PrisonerQuest"
						LevelQuest = 1
						NameMon = "Prisoner"
						CFrameQuest = CFrame.new(5308.93115, 1.65517521, 475.120514, -0.0894274712, -5.00292918e-09, -0.995993316, 1.60817859e-09, 1, -5.16744869e-09, 0.995993316, -2.06384709e-09, -0.0894274712)
						CFrameMon = CFrame.new(5433.39307, 88.678093, 514.986877, 0.879988372, 0, -0.474995494, 0, 1, 0, 0.474995494, 0, 0.879988372)
						SPAWNPOINT = "Prison"
					elseif MyLevel == 210 or MyLevel <= 249 or _G.SelectMonster == "Dangerous Prisoner" then
						Ms = "Dangerous Prisoner"
						NameQuest = "PrisonerQuest"
						LevelQuest = 2
						NameMon = "Dangerous Prisoner"
						CFrameQuest = CFrame.new(5308.93115, 1.65517521, 475.120514, -0.0894274712, -5.00292918e-09, -0.995993316, 1.60817859e-09, 1, -5.16744869e-09, 0.995993316, -2.06384709e-09, -0.0894274712)
						CFrameMon = CFrame.new(5433.39307, 88.678093, 514.986877, 0.879988372, 0, -0.474995494, 0, 1, 0, 0.474995494, 0, 0.879988372)
						SPAWNPOINT = "Prison"
					elseif MyLevel == 250 or MyLevel <= 299 or _G.SelectMonster == "Toga Warrior" then -- Toga Warrior
						Ms = "Toga Warrior"
						NameQuest = "ColosseumQuest"
						LevelQuest = 1
						NameMon = "Toga Warrior"
						CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
						CFrameMon = CFrame.new(-1779.97583, 44.6077499, -2736.35474, 0.984437346, 4.10396339e-08, 0.175734788, -3.62286876e-08, 1, -3.05844168e-08, -0.175734788, 2.3741821e-08, 0.984437346)
						SPAWNPOINT = "Colosseum"
				   elseif MyLevel == 275 or MyLevel <= 299 or _G.SelectMonster == "Gladiator" then -- Gladiato
						Ms = "Gladiator"
						NameQuest = "ColosseumQuest"
						LevelQuest = 2
						NameMon = "Gladiato"
						CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
						CFrameMon = CFrame.new(-1274.75903, 58.1895943, -3188.16309, 0.464524001, 6.21005611e-08, 0.885560572, -4.80449414e-09, 1, -6.76054768e-08, -0.885560572, 2.71497012e-08, 0.464524001)
						SPAWNPOINT = "Colosseum" 
					elseif MyLevel == 300 or MyLevel <= 324 or _G.SelectMonster == "Military Soldier" then -- Military Soldier
						Ms = "Military Soldier"
						NameQuest = "MagmaQuest"
						LevelQuest = 1
						NameMon = "Military Soldier"
						CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
						CFrameMon = CFrame.new(-5363.01123, 41.5056877, 8548.47266, -0.578253984, -3.29503091e-10, 0.815856814, 9.11209668e-08, 1, 6.498761e-08, -0.815856814, 1.11920997e-07, -0.578253984)
						SPAWNPOINT = "Magma"
					elseif MyLevel == 325 or MyLevel <= 374 or _G.SelectMonster == "Military Spy" then -- Military Spy
						Ms = "Military Spy"
						NameQuest = "MagmaQuest"
						LevelQuest = 2
						NameMon = "Military Spy"
						CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
						CFrameMon = CFrame.new(-5787.99023, 120.864456, 8762.25293, -0.188358366, -1.84706277e-08, 0.982100308, -1.23782129e-07, 1, -4.93306951e-09, -0.982100308, -1.22495649e-07, -0.188358366)
						SPAWNPOINT = "Magma"
					elseif MyLevel == 375 or MyLevel <= 399 or _G.SelectMonster == "Fishman Warrior" then -- Fishman Warrior
						Ms = "Fishman Warrior"
						NameQuest = "FishmanQuest"
						LevelQuest = 1
						NameMon = "Fishman Warrior"
						CFrameQuest = CFrame.new(61122.5625, 18.4716396, 1568.16504, 0.893533468, 3.95251609e-09, 0.448996574, -2.34327455e-08, 1, 3.78297464e-08, -0.448996574, -4.43233645e-08, 0.893533468)
						CFrameMon = CFrame.new(60946.6094, 48.6735229, 1525.91687, -0.0817126185, 8.90751153e-08, 0.996655822, 2.00889794e-08, 1, -8.77269599e-08, -0.996655822, 1.28533992e-08, -0.0817126185)
						if _G.Auto_Farm_Level and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
						end
						SPAWNPOINT = "Fountain"
					elseif MyLevel == 400 or MyLevel <= 474 or _G.SelectMonster == "Fishman Commando" then -- Fishman Commando
						Ms = "Fishman Commando"
						NameQuest = "FishmanQuest"
						LevelQuest = 2
						NameMon = "Fishman Commando"
						CFrameQuest = CFrame.new(61122.5625, 18.4716396, 1568.16504, 0.893533468, 3.95251609e-09, 0.448996574, -2.34327455e-08, 1, 3.78297464e-08, -0.448996574, -4.43233645e-08, 0.893533468)
						CFrameMon = CFrame.new(61885.5039, 18.4828243, 1504.17896, 0.577502489, 0, -0.816389024, -0, 1.00000012, -0, 0.816389024, 0, 0.577502489)
						if _G.Auto_Farm_Level and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
						end
						SPAWNPOINT = "Fountain"
					elseif MyLevel == 450 or MyLevel <= 474 or _G.SelectMonster == "God's Guard" then -- God's Guards
						Ms = "God's Guard"
						NameQuest = "SkyExp1Quest"
						LevelQuest = 1
						NameMon = "God's Guards"
						CFrameQuest = CFrame.new(-7860.93555, 5545.61719, -380.700043, 0.406786203, -4.34480496e-09, -0.913523376, -3.57733176e-10, 1, -4.91539254e-09, 0.913523376, 2.32631137e-09, 0.406786203)
						CFrameMon = CFrame.new(-7860.93555, 5545.61719, -380.700043, 0.406786203, -4.34480496e-09, -0.913523376, -3.57733176e-10, 1, -4.91539254e-09, 0.913523376, 2.32631137e-09, 0.406786203)
						if _G.Auto_Farm_Level and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-4607.82275, 872.54248, -1667.55688))
						end
						SPAWNPOINT = "Sky"
					elseif MyLevel == 475 or MyLevel <= 524 or _G.SelectMonster == "Shanda" then -- Shandas
						Ms = "Shanda"
						NameQuest = "SkyExp1Quest"
						LevelQuest = 2
						NameMon = "Shandas"
						CFrameQuest = CFrame.new(-7860.93555, 5545.61719, -380.700043, 0.406786203, -4.34480496e-09, -0.913523376, -3.57733176e-10, 1, -4.91539254e-09, 0.913523376, 2.32631137e-09, 0.406786203)
						CFrameMon = CFrame.new(-7685.12354, 5601.05127, -443.171509, 0.150056243, 1.79768236e-08, -0.988677442, 6.67798661e-09, 1, 1.91962481e-08, 0.988677442, -9.48289181e-09, 0.150056243)
						if _G.Auto_Farm_Level and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
						end
						SPAWNPOINT = "Sky"
					elseif MyLevel == 525 or MyLevel <= 549 or _G.SelectMonster == "Royal Squad" then -- Royal Squad
						Ms = "Royal Squad"
						NameQuest = "SkyExp2Quest"
						LevelQuest = 1
						NameMon = "Royal Squad"
						CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
						CFrameMon = CFrame.new(-7775.55957, 5620.02686, -1361.8988, 0.954580486, 0, -0.297953099, 0, 1, 0, 0.297953099, 0, 0.954580486)
						SPAWNPOINT = "Sky2"
					elseif MyLevel == 550 or MyLevel <= 624 or _G.SelectMonster == "Royal Soldier" then -- Royal Soldier
						Ms = "Royal Soldier"
						NameQuest = "SkyExp2Quest"
						LevelQuest = 2
						NameMon = "Royal Soldier"
						CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
						CFrameMon = CFrame.new(-7864.44775, 5661.94092, -1708.22351, 0.998389959, 2.28686137e-09, -0.0567218624, 1.99431383e-09, 1, 7.54200258e-08, 0.0567218624, -7.54117195e-08, 0.998389959)
						SPAWNPOINT = "Sky2"
					elseif MyLevel == 625 or MyLevel <= 649 or _G.SelectMonster == "Galley Pirate" then -- Galley Pirate
						Ms = "Galley Pirate"
						NameQuest = "FountainQuest"
						LevelQuest = 1
						NameMon = "Galley Pirate"
						CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
						CFrameMon = CFrame.new(5595.06982, 41.5013695, 3961.47095, -0.992138803, -2.11610267e-08, -0.125142589, -1.34249509e-08, 1, -6.26613996e-08, 0.125142589, -6.04887518e-08, -0.992138803)
						SPAWNPOINT = "Fountain"
					elseif MyLevel >= 650 or _G.SelectMonster == "Galley Captain" then -- Galley Captain
						Ms = "Galley Captain"
						NameQuest = "FountainQuest"
						LevelQuest = 2
						NameMon = "Galley Captain"
						CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
						CFrameMon = CFrame.new(5658.5752, 38.5361786, 4928.93506, -0.996873081, 2.12391046e-06, -0.0790185928, 2.16989656e-06, 1, -4.96097414e-07, 0.0790185928, -6.66008248e-07, -0.996873081)
						SPAWNPOINT = "Fountain"
					end
				elseif World2 then
					if MyLevel == 700 or MyLevel <= 724 or _G.SelectMonster == "Raider" then -- Raider [Lv. 700]
						Ms = "Raider"
						NameQuest = "Area1Quest"
						LevelQuest = 1
						NameMon = "Raider"
						CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
						CFrameMon = CFrame.new(-737.026123, 39.1748352, 2392.57959, 0.272128761, 0, -0.962260842, -0, 1, -0, 0.962260842, 0, 0.272128761)
						SPAWNPOINT = "DressTown"
					elseif MyLevel == 725 or MyLevel <= 774 or _G.SelectMonster == "Mercenary" then -- Mercenary [Lv. 725]
						Ms = "Mercenary"
						NameQuest = "Area1Quest"
						LevelQuest = 2
						NameMon = "Mercenary"
						CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
						CFrameMon = CFrame.new(-973.731995, 95.8733215, 1836.46936, 0.999135971, 2.02326991e-08, -0.0415605344, -1.90767793e-08, 1, 2.82094952e-08, 0.0415605344, -2.73922804e-08, 0.999135971)
						SPAWNPOINT = "DressTown"
					elseif MyLevel == 775 or MyLevel <= 799 or _G.SelectMonster == "Swan Pirate" then -- Swan Pirate [Lv. 775]
						Ms = "Swan Pirate"
						NameQuest = "Area2Quest"
						LevelQuest = 1
						NameMon = "Swan Pirate"
						CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
						CFrameMon = CFrame.new(970.369446, 142.653198, 1217.3667, 0.162079468, -4.85452638e-08, -0.986777723, 1.03357589e-08, 1, -4.74980872e-08, 0.986777723, -2.50063148e-09, 0.162079468)
						SPAWNPOINT = "DressTown"
					elseif MyLevel == 800 or MyLevel <= 874 or _G.SelectMonster == "Factory Staff" then -- Factory Staff [Lv. 800]
						Ms = "Factory Staff"
						NameQuest = "Area2Quest"
						LevelQuest = 2
						NameMon = "Factory Staff"
						CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
						CFrameMon = CFrame.new(296.786499, 72.9948196, -57.1298141, -0.876037002, -5.32364979e-08, 0.482243896, -3.87658332e-08, 1, 3.99718729e-08, -0.482243896, 1.63222538e-08, -0.876037002)
						SPAWNPOINT = "DressTown"
					elseif MyLevel == 875 or MyLevel <= 899 or _G.SelectMonster == "Marine Lieutenant" then -- Marine Lieutenant [Lv. 875]
						Ms = "Marine Lieutenant"
						NameQuest = "MarineQuest3"
						LevelQuest = 1
						NameMon = "Marine Lieutenant"
						CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
						CFrameMon = CFrame.new(-2913.26367, 73.0011826, -2971.64282, 0.910507619, 0, 0.413492233, 0, 1.00000012, 0, -0.413492233, 0, 0.910507619)
						SPAWNPOINT = "Greenb"
					elseif MyLevel == 900 or MyLevel <= 949 or _G.SelectMonster == "Marine Captain" then -- Marine Captain [Lv. 900]
						Ms = "Marine Captain"
						NameQuest = "MarineQuest3"
						LevelQuest = 2
						NameMon = "Marine Captain"
						CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
						CFrameMon = CFrame.new(-1868.67688, 73.0011826, -3321.66333, -0.971402287, 1.06502087e-08, 0.237439692, 3.68856199e-08, 1, 1.06050372e-07, -0.237439692, 1.11775684e-07, -0.971402287)
						SPAWNPOINT = "Greenb"
					elseif MyLevel == 950 or MyLevel <= 974 or _G.SelectMonster == "Zombie" then -- Zombie [Lv. 950]
						Ms = "Zombie"
						NameQuest = "ZombieQuest"
						LevelQuest = 1
						NameMon = "Zombie"
						CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
						CFrameMon = CFrame.new(-5634.83838, 126.067039, -697.665039, -0.992770672, 6.77618939e-09, 0.120025545, 1.65461245e-08, 1, 8.04023372e-08, -0.120025545, 8.18070234e-08, -0.992770672)
						SPAWNPOINT = "Graveyard"
					elseif MyLevel == 975 or MyLevel <= 999 or _G.SelectMonster == "Vampire" then -- Vampire [Lv. 975]
						Ms = "Vampire"
						NameQuest = "ZombieQuest"
						LevelQuest = 2
						NameMon = "Vampire"
						CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
						CFrameMon = CFrame.new(-6030.32031, 6.4377408, -1313.5564, -0.856965423, 3.9138893e-08, -0.515373945, -1.12178942e-08, 1, 9.45958547e-08, 0.515373945, 8.68467822e-08, -0.856965423)
						SPAWNPOINT = "Graveyard"
					elseif MyLevel == 1000 or MyLevel <= 1049 or _G.SelectMonster == "Snow Trooper" then -- Snow Trooper [Lv. 1000] **
						Ms = "Snow Trooper"
						NameQuest = "SnowMountainQuest"
						LevelQuest = 1
						NameMon = "Snow Trooper"
						CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
						CFrameMon = CFrame.new(535.893433, 401.457062, -5329.6958, -0.999524176, 0, 0.0308452044, 0, 1, -0, -0.0308452044, 0, -0.999524176)
						SPAWNPOINT = "Snowy"
					elseif MyLevel == 1050 or MyLevel <= 1099 or _G.SelectMonster == "Winter Warrior" then -- Winter Warrior [Lv. 1050]
						Ms = "Winter Warrior"
						NameQuest = "SnowMountainQuest"
						LevelQuest = 2
						NameMon = "Winter Warrior"
						CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
						CFrameMon = CFrame.new(1223.7417, 454.575226, -5170.02148, 0.473996818, 2.56845354e-08, 0.880526543, -5.62456428e-08, 1, 1.10811016e-09, -0.880526543, -5.00510211e-08, 0.473996818)
						SPAWNPOINT = "Snowy"
					elseif MyLevel == 1100 or MyLevel <= 1124 or _G.SelectMonster == "Lab Subordinate" then -- Lab Subordinate [Lv. 1100]
						Ms = "Lab Subordinate"
						NameQuest = "IceSideQuest"
						LevelQuest = 1
						NameMon = "Lab Subordinate"
						CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
						CFrameMon = CFrame.new(-5769.2041, 37.9288292, -4468.38721, -0.569419742, -2.49055017e-08, 0.822046936, -6.96206541e-08, 1, -1.79282633e-08, -0.822046936, -6.74401548e-08, -0.569419742)
						SPAWNPOINT = "CircleIslandIce"
					elseif MyLevel == 1125 or MyLevel <= 1174 or _G.SelectMonster == "Horned Warrior" then -- Horned Warrior [Lv. 1125]
						Ms = "Horned Warrior"
						NameQuest = "IceSideQuest"
						LevelQuest = 2
						NameMon = "Horned Warrior"
						CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
						CFrameMon = CFrame.new(-6400.85889, 24.7645149, -5818.63574, -0.964845479, 8.65926566e-08, -0.262817472, 3.98261392e-07, 1, -1.13260398e-06, 0.262817472, -1.19745812e-06, -0.964845479)
						SPAWNPOINT = "CircleIslandIce"
					elseif MyLevel == 1175 or MyLevel <= 1199 or _G.SelectMonster == "Magma Ninja" then -- Magma Ninja [Lv. 1175]
						Ms = "Magma Ninja"
						NameQuest = "FireSideQuest"
						LevelQuest = 1
						NameMon = "Magma Ninja"
						CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
						CFrameMon = CFrame.new(-5496.65576, 58.6890411, -5929.76855, -0.885073781, 0, -0.465450764, 0, 1.00000012, -0, 0.465450764, 0, -0.885073781)
						SPAWNPOINT = "CircleIslandFire"
					elseif MyLevel == 1200 or MyLevel <= 1249 or _G.SelectMonster == "Lava Pirate" then -- Lava Pirate [Lv. 1200]
						Ms = "Lava Pirate"
						NameQuest = "FireSideQuest"
						LevelQuest = 2
						NameMon = "Lava Pirate"
						CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
						CFrameMon = CFrame.new(-5169.71729, 34.1234779, -4669.73633, -0.196780294, 0, 0.98044765, 0, 1.00000012, -0, -0.98044765, 0, -0.196780294)
						SPAWNPOINT = "CircleIslandFire"
					elseif MyLevel == 1250 or MyLevel <= 1274 or _G.SelectMonster == "Ship Deckhand" then -- Ship Deckhand [Lv. 1250]
						Ms = "Ship Deckhand"
						NameQuest = "ShipQuest1"
						LevelQuest = 1
						NameMon = "Ship Deckhand"
						CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
						CFrameMon = CFrame.new(1163.80872, 138.288452, 33058.4258, -0.998580813, 5.49076979e-08, -0.0532564968, 5.57436763e-08, 1, -1.42118655e-08, 0.0532564968, -1.71604082e-08, -0.998580813)
					if _G.Auto_Farm_Level and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
					end
						SPAWNPOINT = "Ship"
					elseif MyLevel == 1275 or MyLevel <= 1299 or _G.SelectMonster == "Ship Engineer"  then -- Ship Engineer [Lv. 1275]
						Ms = "Ship Engineer"
						NameQuest = "ShipQuest1"
						LevelQuest = 2
						NameMon = "Ship Engineer"
						CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
						CFrameMon = CFrame.new(916.666504, 44.0920448, 32917.207, -0.99746871, -4.85034697e-08, -0.0711069331, -4.8925461e-08, 1, 4.19294288e-09, 0.0711069331, 7.66126895e-09, -0.99746871)
					if _G.Auto_Farm_Level and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
					end
						SPAWNPOINT = "Ship"
					elseif MyLevel == 1300 or MyLevel <= 1324 or _G.SelectMonster == "Ship Steward" then -- Ship Steward [Lv. 1300]
						Ms = "Ship Steward"
						NameQuest = "ShipQuest2"
						LevelQuest = 1
						NameMon = "Ship Steward"
						CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
						CFrameMon = CFrame.new(918.743286, 129.591064, 33443.4609, -0.999792814, -1.7070947e-07, -0.020350717, -1.72559169e-07, 1, 8.91351277e-08, 0.020350717, 9.2628369e-08, -0.999792814)
					if _G.Auto_Farm_Level and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
					end
						SPAWNPOINT = "Ship"
					elseif MyLevel == 1325 or MyLevel <= 1349 or _G.SelectMonster == "Ship Officer" then -- Ship Officer [Lv. 1325]
						Ms = "Ship Officer"
						NameQuest = "ShipQuest2"
						LevelQuest = 2
						NameMon = "Ship Officer"
						CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
						CFrameMon = CFrame.new(955.384583, 181.120193, 33331.8906, 1, -1.07042253e-09, -3.66113085e-14, 1.07042253e-09, 1, 2.00931161e-09, 3.6609157e-14, -2.00931161e-09, 1)
					if _G.Auto_Farm_Level and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
					end
						SPAWNPOINT = "Ship"
					elseif MyLevel == 1350 or MyLevel <= 1374 or _G.SelectMonster == "Arctic Warrior" then -- Arctic Warrior [Lv. 1350]
						Ms = "Arctic Warrior"
						NameQuest = "FrostQuest"
						LevelQuest = 1
						NameMon = "Arctic Warrior"
						CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
						CFrameMon = CFrame.new(5995.07471, 57.3188477, -6183.47314, 0.702747107, -1.53454167e-07, -0.711440146, -1.08168464e-07, 1, -3.22542007e-07, 0.711440146, 3.03620908e-07, 0.702747107)
					if _G.Auto_Farm_Level and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-6508.5581054688, 89.034996032715, -132.83953857422))
					end
						SPAWNPOINT = "IceCastle"
					elseif MyLevel == 1375 or MyLevel <= 1424 or _G.SelectMonster == "Snow Lurker" then -- Snow Lurker [Lv. 1375]
						Ms = "Snow Lurker"
						NameQuest = "FrostQuest"
						LevelQuest = 2
						NameMon = "Snow Lurker"
						CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
						CFrameMon = CFrame.new(5518.00684, 60.5559731, -6828.80518, -0.650781393, -3.64292951e-08, 0.759265184, -4.07668654e-09, 1, 4.44854642e-08, -0.759265184, 2.58550248e-08, -0.650781393)
						SPAWNPOINT = "IceCastle"
					elseif MyLevel == 1425 or MyLevel <= 1449 or _G.SelectMonster == "Sea Soldier" then -- Sea Soldier [Lv. 1425]
						Ms = "Sea Soldier"
						NameQuest = "ForgottenQuest"
						LevelQuest = 1
						NameMon = "Sea Soldier"
						CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
						CFrameMon = CFrame.new(-3029.78467, 66.944252, -9777.38184, -0.998552859, 1.09555076e-08, 0.0537791774, 7.79564235e-09, 1, -5.89660658e-08, -0.0537791774, -5.84614881e-08, -0.998552859)
						SPAWNPOINT = "ForgottenIsland"
					elseif MyLevel >= 1450 or _G.SelectMonster == "Water Fighter" then -- Water Fighter [Lv. 1450]
						Ms = "Water Fighter"
						NameQuest = "ForgottenQuest"
						LevelQuest = 2
						NameMon = "Water Fighter"
						CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
						CFrameMon = CFrame.new(-3262.00098, 298.699615, -10553.6943, -0.233570755, -4.57538185e-08, 0.972339869, -5.80986068e-08, 1, 3.30992194e-08, -0.972339869, -4.87605725e-08, -0.233570755)
						SPAWNPOINT = "ForgottenIsland"
					end
				elseif World3 then
					if MyLevel == 1500 or MyLevel <= 1524 or _G.SelectMonster == "Pirate Millionaire" then
						Ms = "Pirate Millionaire"
						NameQuest = "PiratePortQuest"
						LevelQuest = 1
						NameMon = "Pirate Millionaire"
						CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
						CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
						SPAWNPOINT = "Default"
					elseif MyLevel == 1525 or MyLevel <= 1574 or _G.SelectMonster == "Pistol Billionaire" then
						Ms = "Pistol Billionaire"
						NameQuest = "PiratePortQuest"
						LevelQuest = 2
						NameMon = "Pistol Billionaire"
						CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
						CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
						SPAWNPOINT = "Default"
					elseif MyLevel == 1575 or MyLevel <= 1599 or _G.SelectMonster == "Dragon Crew Warrior" then
						Ms = "Dragon Crew Warrior"
						NameQuest = "AmazonQuest"
						LevelQuest = 1
						NameMon = "Dragon Crew Warrior"
						CFrameQuest = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
						CFrameMon = CFrame.new(6241.9951171875, 51.522083282471, -1243.9771728516)
						SPAWNPOINT = "Hydra3"
					elseif MyLevel == 1600 or MyLevel <= 1624 or _G.SelectMonster == "Dragon Crew Archer" then
						Ms = "Dragon Crew Archer"
						NameQuest = "AmazonQuest"
						LevelQuest = 2
						NameMon = "Dragon Crew Archer"
						CFrameQuest = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
						CFrameMon = CFrame.new(6488.9155273438, 383.38375854492, -110.66246032715)
						SPAWNPOINT = "Hydra3"
					elseif MyLevel == 1625 or MyLevel <= 1649 or _G.SelectMonster == "Female Islander" then
						Ms = "Female IslandeR"
						NameQuest = "AmazonQuest2"
						LevelQuest = 1
						NameMon = "Female Islander"
						CFrameQuest = CFrame.new(5448.86133, 601.516174, 751.130676, 0, 0, 1, 0, 1, -0, -1, 0, 0)
						CFrameMon = CFrame.new(4770.4990234375, 758.95520019531, 1069.8680419922)
						SPAWNPOINT = "Hydra1"
					elseif MyLevel == 1650 or MyLevel <= 1699 or _G.SelectMonster == "Giant Islander" then
						Ms = "Giant Islander"
						NameQuest = "AmazonQuest2"
						LevelQuest = 2
						NameMon = "Giant Islander"
						CFrameQuest = CFrame.new(5448.86133, 601.516174, 751.130676, 0, 0, 1, 0, 1, -0, -1, 0, 0)
						CFrameMon = CFrame.new(4530.3540039063, 656.75695800781, -131.60952758789)
						SPAWNPOINT = "Hydra1"
					elseif MyLevel == 1700 or MyLevel <= 1724 or _G.SelectMonster == "Marine Commodore" then
						Ms = "Marine Commodore"
						NameQuest = "MarineTreeIsland"
						LevelQuest = 1
						NameMon = "Marine Commodore"
						CFrameQuest = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
						CFrameMon = CFrame.new(2490.0844726563, 190.4232635498, -7160.0502929688)
						SPAWNPOINT = "GreatTree"
					elseif MyLevel == 1725 or MyLevel <= 1774 or _G.SelectMonster == "Marine Rear Admiral" then
						Ms = "Marine Rear Admiral"
						NameQuest = "MarineTreeIsland"
						LevelQuest = 2
						NameMon = "Marine Rear Admiral"
						CFrameQuest = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
						CFrameMon = CFrame.new(3951.3903808594, 229.11549377441, -6912.81640625)
						SPAWNPOINT = "GreatTree"
					elseif MyLevel == 1775 or MyLevel <= 1799 or _G.SelectMonster == "Fishman Raider" then
						Ms = "Fishman Raider"
						NameQuest = "DeepForestIsland3"
						LevelQuest = 1
						NameMon = "Fishman Raider"
						CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
						CFrameMon = CFrame.new(-10322.400390625, 390.94473266602, -8580.0908203125)
						SPAWNPOINT = "PineappleTown"
					elseif MyLevel == 1800 or MyLevel <= 1824 or _G.SelectMonster == "Fishman Captain" then
						Ms = "Fishman Captain"
						NameQuest = "DeepForestIsland3"
						LevelQuest = 2
						NameMon = "Fishman Captain"
						CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
						CFrameMon = CFrame.new(-11194.541992188, 442.02795410156, -8608.806640625)
						SPAWNPOINT = "PineappleTown"
					elseif MyLevel == 1825 or MyLevel <= 1849 or _G.SelectMonster == "Forest Pirate" then
						Ms = "Forest Pirate"
						NameQuest = "DeepForestIsland"
						LevelQuest = 1
						NameMon = "Forest Pirate"
						CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
						CFrameMon = CFrame.new(-13225.809570313, 428.19387817383, -7753.1245117188)
						SPAWNPOINT = "BigMansion"
					elseif MyLevel == 1850 or MyLevel <= 1899 or _G.SelectMonster == "Mythological Pirate" then
						Ms = "Mythological Pirate"
						NameQuest = "DeepForestIsland"
						LevelQuest = 2
						NameMon = "Mythological Pirate"
						CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
						CFrameMon = CFrame.new(-13869.172851563, 564.95251464844, -7084.4135742188)
						SPAWNPOINT = "BigMansion"
					elseif MyLevel == 1900 or MyLevel <= 1924 or _G.SelectMonster == "Jungle Pirate" then
						Ms = "Jungle Pirate"
						NameQuest = "DeepForestIsland2"
						LevelQuest = 1
						NameMon = "Jungle Pirate"
						CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
						CFrameMon = CFrame.new(-11982.221679688, 376.32522583008, -10451.415039063)
						SPAWNPOINT = "PineappleTown"
					elseif MyLevel == 1925 or MyLevel <= 1974 or _G.SelectMonster == "Musketeer Pirate" then
						Ms = "Musketeer Pirate"
						NameQuest = "DeepForestIsland2"
						LevelQuest = 2
						NameMon = "Musketeer Pirate"
						CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
						CFrameMon = CFrame.new(-13282.3046875, 496.23684692383, -9565.150390625)
						SPAWNPOINT = "PineappleTown"
					elseif MyLevel == 1975 or MyLevel <= 1999 or _G.SelectMonster == "Reborn Skeleton" then
						Ms = "Reborn Skeleton"
						NameQuest = "HauntedQuest1"
						LevelQuest = 1
						NameMon = "Reborn Skeleton"
						CFrameQuest = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
						CFrameMon = CFrame.new(-8761.3154296875, 164.85829162598, 6161.1567382813)
						SPAWNPOINT = "HauntedCastle"
					elseif MyLevel == 2000 or MyLevel <= 2024 or _G.SelectMonster == "Living Zombie" then
						Ms = "Living Zombie"
						NameQuest = "HauntedQuest1"
						LevelQuest = 2
						NameMon = "Living Zombie"
						CFrameQuest = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
						CFrameMon = CFrame.new(-10093.930664063, 237.38233947754, 6180.5654296875)
						SPAWNPOINT = "HauntedCastle"
					elseif MyLevel == 2025 or MyLevel <= 2049 or _G.SelectMonster == "Demonic Soul" then
						Ms = "Demonic Soul"
						NameQuest = "HauntedQuest2"
						LevelQuest = 1
						NameMon = "Demonic Soul"
						CFrameQuest = CFrame.new(-9514.78027, 171.162918, 6078.82373, 0.301918149, 7.4535027e-09, 0.953333855, -3.22802141e-09, 1, -6.79604995e-09, -0.953333855, -1.02553133e-09, 0.301918149)
						CFrameMon = CFrame.new(-9466.72949, 171.162918, 6132.01514)
						SPAWNPOINT = "HauntedCastle"
					elseif MyLevel == 2050 or MyLevel <= 2074 or _G.SelectMonster == "Posessed Mummy" then
						Ms = "Posessed Mummy" 
						NameQuest = "HauntedQuest2"
						LevelQuest = 2
						NameMon = "Posessed Mummy"
						CFrameQuest = CFrame.new(-9514.78027, 171.162918, 6078.82373, 0.301918149, 7.4535027e-09, 0.953333855, -3.22802141e-09, 1, -6.79604995e-09, -0.953333855, -1.02553133e-09, 0.301918149)
						CFrameMon = CFrame.new(-9589.93848, 4.85058546, 6190.27197)
						SPAWNPOINT = "HauntedCastle"
					elseif MyLevel == 2075 or MyLevel <= 2099 or _G.SelectMonster == "Peanut Scout" then
						Ms = "Peanut Scout"
						NameQuest = "NutsIslandQuest"
						LevelQuest = 1
						NameMon = "Peanut Scout"
						CFrameQuest = CFrame.new(-2103.9375, 38.139019012451, -10192.702148438)
						CFrameMon = CFrame.new(-2150.587890625, 122.49767303467, -10358.994140625)
						SPAWNPOINT = "Peanut"
					elseif MyLevel == 2100 or MyLevel <= 2124 or _G.SelectMonster == "Peanut President" then
						Ms = "Peanut President"
						NameQuest = "NutsIslandQuest"
						LevelQuest = 2
						NameMon = "Peanut President"
						CFrameQuest = CFrame.new(-2103.9375, 38.139019012451, -10192.702148438)
						CFrameMon = CFrame.new(-2150.587890625, 122.49767303467, -10358.994140625)
						SPAWNPOINT = "Peanut"
					elseif MyLevel == 2125 or MyLevel <= 2149 or _G.SelectMonster == "Ice Cream Chef" then
						Ms = "Ice Cream Chef"
						NameQuest = "IceCreamIslandQuest"
						LevelQuest = 1
						NameMon = "Ice Cream Chef"
						CFrameQuest = CFrame.new(-819.84533691406, 65.845329284668, -10965.487304688)
						CFrameMon = CFrame.new(-890.55895996094, 186.34135437012, -11127.306640625)
						SPAWNPOINT = "IceCream"
					elseif MyLevel == 2150 or MyLevel <= 2199 or _G.SelectMonster == "Ice Cream Commander" then
						Ms = "Ice Cream Commander"
						NameQuest = "IceCreamIslandQuest"
						LevelQuest = 2
						NameMon = "Ice Cream Commander"
						CFrameQuest = CFrame.new(-819.84533691406, 65.845329284668, -10965.487304688)
						CFrameMon = CFrame.new(-890.55895996094, 186.34135437012, -11127.306640625)
						SPAWNPOINT = "IceCream"
					elseif MyLevel == 2200 or MyLevel <= 2224 or _G.SelectMonster == "Cookie Crafter" then
						Ms = "Cookie Crafter"
						NameQuest = "CakeQuest1"
						LevelQuest = 1
						NameMon = "Cookie Crafter"
						CFrameQuest = CFrame.new(-2021.5509033203125, 37.798221588134766, -12028.103515625)
						CFrameMon = CFrame.new(-2273.00244140625, 90.22590637207031, -12151.62109375)
						SPAWNPOINT = "Loaf"
					elseif MyLevel == 2225 or MyLevel <= 2249 or _G.SelectMonster == "Cake Guard" then
						Ms = "Cake Guard"
						NameQuest = "CakeQuest1"
						LevelQuest = 2
						NameMon = "Cake Guard"
						CFrameQuest = CFrame.new(-2021.5509033203125, 37.798221588134766, -12028.103515625)
						CFrameMon = CFrame.new(-1442.373046875, 158.14111328125, -12277.37109375)
						SPAWNPOINT = "Loaf"
					elseif MyLevel == 2250 or MyLevel <= 2274 or _G.SelectMonster == "Baking Staff" then
						Ms = "Baking Staff"
						NameQuest = "CakeQuest2"
						LevelQuest = 1
						NameMon = "Baking Staff"
						CFrameQuest = CFrame.new(-1927.9107666015625, 37.79813003540039, -12843.78515625)
						CFrameMon = CFrame.new(-1837.2803955078125, 129.0594482421875, -12934.5498046875)
						SPAWNPOINT = "Loaf"
					elseif MyLevel == 2275 or MyLevel <= 2299 or _G.SelectMonster == "Head Baker" then
						Ms = "Head Baker"
						NameQuest = "CakeQuest2"
						LevelQuest = 2
						NameMon = "Head Baker"
						CFrameQuest = CFrame.new(-1927.9107666015625, 37.79813003540039, -12843.78515625)
						CFrameMon = CFrame.new(-2203.302490234375, 109.90937042236328, -12788.7333984375)
						SPAWNPOINT = "Loaf"
					elseif MyLevel == 2300 or MyLevel <= 2324 or _G.SelectMonster == "Cocoa Warrior" then
						Ms = "Cocoa Warrior"
						NameQuest = "ChocQuest1"
						LevelQuest = 1
						NameMon = "Cocoa Warrior"
						CFrameQuest = CFrame.new(231.13571166992188, 24.734268188476562, -12195.1162109375)
						CFrameMon = CFrame.new(231.13571166992188, 24.734268188476562, -12195.1162109375)
						SPAWNPOINT = "Chocolate"
					elseif MyLevel == 2325 or MyLevel <= 2349 or _G.SelectMonster == "Chocolate Bar Battler" then
						Ms = "Chocolate Bar Battler"
						NameQuest = "ChocQuest1"
						LevelQuest = 2
						NameMon = "Chocolate Bar Battler"
						CFrameQuest = CFrame.new(231.13571166992188, 24.734268188476562, -12195.1162109375)
						CFrameMon = CFrame.new(311.1222839355469, 149.17347717285156, -12279.9228515625)
						SPAWNPOINT = "Chocolate"
					elseif MyLevel == 2350 or MyLevel <= 2374 or _G.SelectMonster == "Sweet Thief" then
						Ms = "Sweet Thief"
						NameQuest = "ChocQuest2"
						LevelQuest = 1
						NameMon = "Sweet Thief"
						CFrameQuest = CFrame.new(147.52256774902344, 24.793832778930664, -12775.3583984375)
						CFrameMon = CFrame.new(42.193599700927734, 144.3453826904297, -12888.8125)
						SPAWNPOINT = "Chocolate"
					elseif MyLevel == 2375 or MyLevel <= 2399 or _G.SelectMonster == "Candy Rebel" then
						Ms = "Candy Rebel"
						NameQuest = "ChocQuest2"
						LevelQuest = 2
						NameMon = "Candy Rebel"
						CFrameQuest = CFrame.new(147.52256774902344, 24.793832778930664, -12775.3583984375)
						CFrameMon = CFrame.new(42.193599700927734, 144.3453826904297, -12888.8125)
						SPAWNPOINT = "Chocolate"
					elseif MyLevel == 2400 or MyLevel <= 2424 or _G.SelectMonster == "Candy Pirate" then
						Ms = "Candy Pirate"
						NameQuest = "CandyQuest1"
						LevelQuest = 1
						NameMon = "Candy Pirate"
						CFrameQuest = CFrame.new(-1147.2296142578125, 14.133421897888184, -14445.1162109375)
						CFrameMon = CFrame.new(-1488.756103515625, 131.76937866210938, -14374.365234375)
						SPAWNPOINT = "CandyCane"  
					elseif MyLevel == 2425 or MyLevel <= 2449 or _G.SelectMonster == "Snow Demon" then
						Ms = "Snow Demon"
						NameQuest = "CandyQuest1"
						LevelQuest = 2
						NameMon = "Snow Demon"
						CFrameQuest = CFrame.new(-1147.2296142578125, 14.133421897888184, -14445.1162109375)
						CFrameMon = CFrame.new(-923.905029296875, 100.98135375976562, -14330.78125)
						SPAWNPOINT = "CandyCane"   
					elseif MyLevel == 2450 or MyLevel <= 2474 or _G.SelectMonster == "Isle Outlaw" then
						Ms = "Isle Outlaw"
						NameQuest = "TikiQuest1"
						LevelQuest = 1
						NameMon = "Isle Outlaw"
						CFrameQuest = CFrame.new(-16547.4082, 56.1548653, -172.937408, -0.181595549, -7.60041203e-08, 0.983373284, -4.05321572e-08, 1, 6.98042797e-08, -0.983373284, -2.71820948e-08, -0.181595549)
						CFrameMon = CFrame.new(-16303.2246, 103.04068, -252.528397, -0.975547493, -2.41556144e-08, 0.219788775, -4.32304281e-09, 1, 9.07156448e-08, -0.219788775, 8.75472637e-08, -0.975547493)
						SPAWNPOINT = "TikiOutpost"
					elseif MyLevel == 2475 or MyLevel <= 2499 or _G.SelectMonster == "Island Boy" then
						Ms = "Island Boy"
						NameQuest = "TikiQuest1"
						LevelQuest = 2
						NameMon = "Island Boy"
						CFrameQuest = CFrame.new(-16547.4082, 56.1548653, -172.937408, -0.181595549, -7.60041203e-08, 0.983373284, -4.05321572e-08, 1, 6.98042797e-08, -0.983373284, -2.71820948e-08, -0.181595549)
						CFrameMon = CFrame.new(-16930.5508, 84.3850174, -185.271744, -0.963041961, -6.27662118e-08, -0.269351333, -4.70760142e-08, 1, -6.4711152e-08, 0.269351333, -4.96395671e-08, -0.963041961)
						SPAWNPOINT = "TikiOutpost"  
					elseif MyLevel == 2500 or MyLevel <= 2524 or _G.SelectMonster == "Sun-kissed Warrior" then
						Ms = "Sun-kissed Warrior"
						NameQuest = "TikiQuest2"
						LevelQuest = 1
						NameMon = "Sun-kissed Warrior"
						CFrameQuest = CFrame.new(-16539.541, 56.0037842, 1051.42029, 0.0053731557, -2.40092142e-08, 0.999985576, -3.64830015e-08, 1, 2.42055922e-08, -0.999985576, -3.6612537e-08, 0.0053731557)	
						CFrameMon = CFrame.new(-16336.0303, 107.23838, 1131.62488, 0.952998042, -4.06232665e-08, 0.302976489, 2.92190965e-08, 1, 4.21733155e-08, -0.302976489, -3.13383879e-08, 0.952998042)
						SPAWNPOINT = "TikiOutpost"
					elseif MyLevel >= 2525 or _G.SelectMonster == "Isle Champion" then
						Ms = "Isle Champion"
						NameQuest = "TikiQuest2"
						LevelQuest = 2
						NameMon = "Isle Champion"
						CFrameQuest = CFrame.new(-16539.541, 56.0037842, 1051.42029, 0.0053731557, -2.40092142e-08, 0.999985576, -3.64830015e-08, 1, 2.42055922e-08, -0.999985576, -3.6612537e-08, 0.0053731557)
						CFrameMon = CFrame.new(-16775.6895, 82.456459, 1031.00037, -0.566521764, 8.14919474e-08, 0.824046791, 4.23231263e-08, 1, -6.97957674e-08, -0.824046791, -4.66458294e-09, -0.566521764)
						SPAWNPOINT = "TikiOutpost"  
					end
				end
			end

			function CheckBossQuest()
				if _G.Select_Boss == "Saber Expert [Lv. 200] [Boss]" then
					MsBoss = "Saber Expert [Lv. 200] [Boss]"
					NameBoss = "Saber Expert"
					CFrameBoss = CFrame.new(-1458.89502, 29.8870335, -50.633564, 0.858821094, 1.13848939e-08, 0.512275636, -4.85649254e-09, 1, -1.40823326e-08, -0.512275636, 9.6063415e-09, 0.858821094)
				elseif _G.Select_Boss == "The Saw [Lv. 100] [Boss]" then
					MsBoss = "The Saw [Lv. 100] [Boss]"
					NameBoss = "The Saw"
					CFrameBoss = CFrame.new(-683.519897, 13.8534927, 1610.87854, -0.290192783, 6.88365773e-08, 0.956968188, 6.98413629e-08, 1, -5.07531119e-08, -0.956968188, 5.21077759e-08, -0.290192783)
				elseif _G.Select_Boss == "Greybeard [Lv. 750] [Raid Boss]" then
					MsBoss = "Greybeard [Lv. 750] [Raid Boss]"
					NameBoss = "Greybeard"
					CFrameBoss = CFrame.new(-4955.72949, 80.8163834, 4305.82666, -0.433646321, -1.03394289e-08, 0.901083171, -3.0443168e-08, 1, -3.17633075e-09, -0.901083171, -2.88092288e-08, -0.433646321)
				elseif _G.Select_Boss == "The Gorilla King [Lv. 25] [Boss]" then
					MsBoss = "The Gorilla King [Lv. 25] [Boss]"
					NameBoss = "The Gorilla King"
					NameQuestBoss = "JungleQuest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
					CFrameBoss = CFrame.new(-1223.52808, 6.27936459, -502.292664, 0.310949147, -5.66602516e-08, 0.950426519, -3.37275488e-08, 1, 7.06501808e-08, -0.950426519, -5.40241736e-08, 0.310949147)
				elseif _G.Select_Boss == "Bobby [Lv. 55] [Boss]" then
					MsBoss = "Bobby [Lv. 55] [Boss]"
					NameBoss = "Bobby"
					NameQuestBoss = "BuggyQuest1"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
					CFrameBoss = CFrame.new(-1147.65173, 32.5966301, 4156.02588, 0.956680477, -1.77109952e-10, -0.29113996, 5.16530874e-10, 1, 1.08897802e-09, 0.29113996, -1.19218679e-09, 0.956680477)
				elseif _G.Select_Boss == "Yeti [Lv. 110] [Boss]" then
					MsBoss = "Yeti [Lv. 110] [Boss]"
					NameBoss = "Yeti"
					NameQuestBoss = "SnowQuest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(1384.90247, 87.3078308, -1296.6825, 0.280209213, 2.72035177e-08, -0.959938943, -6.75690828e-08, 1, 8.6151708e-09, 0.959938943, 6.24481444e-08, 0.280209213)
					CFrameBoss = CFrame.new(1221.7356, 138.046906, -1488.84082, 0.349343032, -9.49245944e-08, 0.936994851, 6.29478194e-08, 1, 7.7838429e-08, -0.936994851, 3.17894653e-08, 0.349343032)
				elseif _G.Select_Boss == "Mob Leader [Lv. 120] [Boss]" then
					MsBoss = "Mob Leader [Lv. 120] [Boss]"
					NameBoss = "Mob Leader"
					CFrameBoss = CFrame.new(-2848.59399, 7.4272871, 5342.44043, -0.928248107, -8.7248246e-08, 0.371961564, -7.61816636e-08, 1, 4.44474857e-08, -0.371961564, 1.29216433e-08, -0.92824)
				elseif _G.Select_Boss == "Vice Admiral [Lv. 130] [Boss]" then
					MsBoss = "Vice Admiral [Lv. 130] [Boss]"
					NameBoss = "Vice Admiral"
					NameQuestBoss = "MarineQuest2"
					LevelQuestBoss = 2
					CFrameQuestBoss = CFrame.new(-5035.42285, 28.6520386, 4324.50293, -0.0611100644, -8.08395768e-08, 0.998130739, -1.57416586e-08, 1, 8.00271849e-08, -0.998130739, -1.08217701e-08, -0.0611100644)
					CFrameBoss = CFrame.new(-5078.45898, 99.6520691, 4402.1665, -0.555574954, -9.88630566e-11, 0.831466436, -6.35508286e-08, 1, -4.23449258e-08, -0.831466436, -7.63661632e-08, -0.555574954)
				elseif _G.Select_Boss == "Warden [Lv. 175] [Boss]" then
					MsBoss = "Warden [Lv. 175] [Boss]"
					NameBoss = "Warden"
					NameQuestBoss = "ImpelQuest"
					LevelQuestBoss = 1
					CFrameQuestBoss = CFrame.new(4851.35059, 5.68744135, 743.251282, -0.538484037, -6.68303741e-08, -0.842635691, 1.38001752e-08, 1, -8.81300792e-08, 0.842635691, -5.90851599e-08, -0.538484037)
					CFrameBoss = CFrame.new(5232.5625, 5.26856995, 747.506897, 0.943829298, -4.5439414e-08, 0.330433697, 3.47818627e-08, 1, 3.81658154e-08, -0.330433697, -2.45289105e-08, 0.943829298)
				elseif _G.Select_Boss == "Chief Warden [Lv. 200] [Boss]" then
					MsBoss = "Chief Warden [Lv. 200] [Boss]"
					NameBoss = "Chief Warden"
					NameQuestBoss = "ImpelQuest"
					LevelQuestBoss = 2
					CFrameQuestBoss = CFrame.new(4851.35059, 5.68744135, 743.251282, -0.538484037, -6.68303741e-08, -0.842635691, 1.38001752e-08, 1, -8.81300792e-08, 0.842635691, -5.90851599e-08, -0.538484037)
					CFrameBoss = CFrame.new(5232.5625, 5.26856995, 747.506897, 0.943829298, -4.5439414e-08, 0.330433697, 3.47818627e-08, 1, 3.81658154e-08, -0.330433697, -2.45289105e-08, 0.943829298)
				elseif _G.Select_Boss == "Swan [Lv. 225] [Boss]" then
					MsBoss = "Swan [Lv. 225] [Boss]"
					NameBoss = "Swan"
					NameQuestBoss = "ImpelQuest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(4851.35059, 5.68744135, 743.251282, -0.538484037, -6.68303741e-08, -0.842635691, 1.38001752e-08, 1, -8.81300792e-08, 0.842635691, -5.90851599e-08, -0.538484037)
					CFrameBoss = CFrame.new(5232.5625, 5.26856995, 747.506897, 0.943829298, -4.5439414e-08, 0.330433697, 3.47818627e-08, 1, 3.81658154e-08, -0.330433697, -2.45289105e-08, 0.943829298)
				elseif _G.Select_Boss == "Magma Admiral [Lv. 350] [Boss]" then
					MsBoss = "Magma Admiral [Lv. 350] [Boss]"
					NameBoss = "Magma Admiral"
					NameQuestBoss = "MagmaQuest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-5317.07666, 12.2721891, 8517.41699, 0.51175487, -2.65508806e-08, -0.859131515, -3.91131572e-08, 1, -5.42026761e-08, 0.859131515, 6.13418294e-08, 0.51175487)
					CFrameBoss = CFrame.new(-5530.12646, 22.8769703, 8859.91309, 0.857838571, 2.23414389e-08, 0.513919294, 1.53689133e-08, 1, -6.91265853e-08, -0.513919294, 6.71978384e-08, 0.857838571)
				elseif _G.Select_Boss == "Fishman Lord [Lv. 425] [Boss]" then
					MsBoss = "Fishman Lord [Lv. 425] [Boss]"
					NameBoss = "Fishman Lord"
					NameQuestBoss = "FishmanQuest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(61123.0859, 18.5066795, 1570.18018, 0.927145958, 1.0624845e-07, 0.374700129, -6.98219367e-08, 1, -1.10790765e-07, -0.374700129, 7.65569368e-08, 0.927145958)
					CFrameBoss = CFrame.new(61351.7773, 31.0306778, 1113.31409, 0.999974668, 0, -0.00714713801, 0, 1.00000012, 0, 0.00714714266, 0, 0.999974549)
				elseif _G.Select_Boss == "Wysper [Lv. 500] [Boss]" then
					MsBoss = "Wysper [Lv. 500] [Boss]"
					NameBoss = "Wysper"
					NameQuestBoss = "SkyExp1Quest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-7862.94629, 5545.52832, -379.833954, 0.462944925, 1.45838088e-08, -0.886386991, 1.0534996e-08, 1, 2.19553424e-08, 0.886386991, -1.95022007e-08, 0.462944925)
					CFrameBoss = CFrame.new(-7925.48389, 5550.76074, -636.178345, 0.716468513, -1.22915289e-09, 0.697619379, 3.37381434e-09, 1, -1.70304748e-09, -0.697619379, 3.57381835e-09, 0.716468513)
				elseif _G.Select_Boss == "Thunder God [Lv. 575] [Boss]" then
					MsBoss = "Thunder God [Lv. 575] [Boss]"
					NameBoss = "Thunder God"
					NameQuestBoss = "SkyExp2Quest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-7902.78613, 5635.99902, -1411.98706, -0.0361216255, -1.16895912e-07, 0.999347389, 1.44533963e-09, 1, 1.17024491e-07, -0.999347389, 5.6715117e-09, -0.0361216255)
					CFrameBoss = CFrame.new(-7917.53613, 5616.61377, -2277.78564, 0.965189934, 4.80563429e-08, -0.261550069, -6.73089886e-08, 1, -6.46515304e-08, 0.261550069, 8.00056768e-08, 0.965189934)
				elseif _G.Select_Boss == "Cyborg [Lv. 675] [Boss]" then
					MsBoss = "Cyborg [Lv. 675] [Boss]"
					NameBoss = "Cyborg"
					NameQuestBoss = "FountainQuest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(5253.54834, 38.5361786, 4050.45166, -0.0112687312, -9.93677887e-08, -0.999936521, 2.55291371e-10, 1, -9.93769547e-08, 0.999936521, -1.37512213e-09, -0.0112687312)
					CFrameBoss = CFrame.new(6041.82813, 52.7112198, 3907.45142, -0.563162148, 1.73805248e-09, -0.826346457, -5.94632716e-08, 1, 4.26280238e-08, 0.826346457, 7.31437524e-08, -0.563162148)
				-- New World
				elseif _G.Select_Boss == "Diamond [Lv. 750] [Boss]" then
					MsBoss = "Diamond [Lv. 750] [Boss]"
					NameBoss = "Diamond"
					NameQuestBoss = "Area1Quest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
					CFrameBoss = CFrame.new(-1736.26587, 198.627731, -236.412857, -0.997808516, 0, -0.0661673471, 0, 1, 0, 0.0661673471, 0, -0.997808516)
				elseif _G.Select_Boss == "Jeremy [Lv. 850] [Boss]" then
					MsBoss = "Jeremy [Lv. 850] [Boss]"
					NameBoss = "Jeremy"
					NameQuestBoss = "Area2Quest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
					CFrameBoss = CFrame.new(2203.76953, 448.966034, 752.731079, -0.0217453763, 0, -0.999763548, 0, 1, 0, 0.999763548, 0, -0.0217453763)
				elseif _G.Select_Boss == "Fajita [Lv. 925] [Boss]" then
					MsBoss = "Fajita [Lv. 925] [Boss]"
					NameBoss = "Fajita"
					NameQuestBoss = "MarineQuest3"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
					CFrameBoss = CFrame.new(-2297.40332, 115.449463, -3946.53833, 0.961227536, -1.46645796e-09, -0.275756449, -2.3212845e-09, 1, -1.34094433e-08, 0.275756449, 1.35296352e-08, 0.961227536)
				elseif _G.Select_Boss == "Don Swan [Lv. 1000] [Boss]" then
					MsBoss = "Don Swan [Lv. 1000] [Boss]"
					NameBoss = "Don Swan"
					CFrameBoss = CFrame.new(2288.802, 15.1870775, 863.034607, 0.99974072, -8.41247214e-08, -0.0227668174, 8.4774733e-08, 1, 2.75850098e-08, 0.0227668174, -2.95079072e-08, 0.99974072)
				elseif _G.Select_Boss == "Smoke Admiral [Lv. 1150] [Boss]" then
					MsBoss = "Smoke Admiral [Lv. 1150] [Boss]"
					NameBoss = "Smoke Admiral"
					NameQuestBoss = "IceSideQuest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-6059.96191, 15.9868021, -4904.7373, -0.444992423, -3.0874483e-09, 0.895534337, -3.64098796e-08, 1, -1.4644522e-08, -0.895534337, -3.91229982e-08, -0.444992423)
					CFrameBoss = CFrame.new(-5115.72754, 23.7664986, -5338.2207, 0.251453817, 1.48345061e-08, -0.967869282, 4.02796978e-08, 1, 2.57916977e-08, 0.967869282, -4.54708946e-08, 0.251453817)
				elseif _G.Select_Boss == "Cursed Captain [Lv. 1325] [Raid Boss]" then
					MsBoss = "Cursed Captain [Lv. 1325] [Raid Boss]"
					NameBoss = "Cursed Captain"
					CFrameBoss = CFrame.new(916.928589, 181.092773, 33422, -0.999505103, 9.26310495e-09, 0.0314563364, 8.42916226e-09, 1, -2.6643713e-08, -0.0314563364, -2.63653774e-08, -0.999505103)
				elseif _G.Select_Boss == "Darkbeard [Lv. 1000] [Raid Boss]" then
					MsBoss = "Darkbeard [Lv. 1000] [Raid Boss]"
					NameBoss = "Darkbeard"
					CFrameBoss = CFrame.new(3876.00366, 24.6882591, -3820.21777, -0.976951957, 4.97356325e-08, 0.213458836, 4.57335361e-08, 1, -2.36868622e-08, -0.213458836, -1.33787044e-08, -0.976951957)
				elseif _G.Select_Boss == "Order [Lv. 1250] [Raid Boss]" then
					MsBoss = "Order [Lv. 1250] [Raid Boss]"
					NameBoss = "Order"
					CFrameBoss = CFrame.new(-6221.15039, 16.2351036, -5045.23584, -0.380726993, 7.41463495e-08, 0.924687505, 5.85604774e-08, 1, -5.60738549e-08, -0.924687505, 3.28013137e-08, -0.380726993)
				elseif _G.Select_Boss == "Awakened Ice Admiral [Lv. 1400] [Boss]" then
					MsBoss = "Awakened Ice Admiral [Lv. 1400] [Boss]"
					NameBoss = "Awakened Ice Admiral"
					NameQuestBoss = "FrostQuest"
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(5669.33203, 28.2118053, -6481.55908, 0.921275556, -1.25320829e-08, 0.388910472, 4.72230788e-08, 1, -7.96414241e-08, -0.388910472, 9.17372489e-08, 0.921275556)
					CFrameBoss = CFrame.new(6407.33936, 340.223785, -6892.521, 0.49051559, -5.25310213e-08, -0.871432424, -2.76146022e-08, 1, -7.58250565e-08, 0.871432424, 6.12576301e-08, 0.49051559)
				elseif _G.Select_Boss == "Tide Keeper [Lv. 1475] [Boss]" then
					MsBoss = "Tide Keeper [Lv. 1475] [Boss]"
					 NameBoss = "Tide Keeper"
					NameQuestBoss = "ForgottenQuest"             
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-3053.89648, 236.881363, -10148.2324, -0.985987961, -3.58504737e-09, 0.16681771, -3.07832915e-09, 1, 3.29612559e-09, -0.16681771, 2.73641976e-09, -0.985987961)
					CFrameBoss = CFrame.new(-3570.18652, 123.328949, -11555.9072, 0.465199202, -1.3857326e-08, 0.885206044, 4.0332897e-09, 1, 1.35347511e-08, -0.885206044, -2.72606271e-09, 0.465199202)
				-- Thire World
				elseif _G.Select_Boss == "Stone [Lv. 1550] [Boss]" then
					MsBoss = "Stone [Lv. 1550] [Boss]"
					NameBoss = "Stone"
					NameQuestBoss = "PiratePortQuest"             
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-290, 44, 5577)
					CFrameBoss = CFrame.new(-1085, 40, 6779)
				elseif _G.Select_Boss == "Island Empress [Lv. 1675] [Boss]" then
					MsBoss = "Island Empress [Lv. 1675] [Boss]"
					 NameBoss = "Island Empress"
					NameQuestBoss = "AmazonQuest2"             
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(5443, 602, 752)
					CFrameBoss = CFrame.new(5659, 602, 244)
				elseif _G.Select_Boss == "Kilo Admiral [Lv. 1750] [Boss]" then
					MsBoss = "Kilo Admiral [Lv. 1750] [Boss]"
					NameBoss = "Kilo Admiral"
					NameQuestBoss = "MarineTreeIsland"             
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(2178, 29, -6737)
					CFrameBoss =CFrame.new(2846, 433, -7100)
				elseif _G.Select_Boss == "Captain Elephant [Lv. 1875] [Boss]" then
					MsBoss = "Captain Elephant [Lv. 1875] [Boss]"
					NameBoss = "Captain Elephant"
					NameQuestBoss = "DeepForestIsland"             
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-13232, 333, -7631)
					CFrameBoss = CFrame.new(-13221, 325, -8405)
				elseif _G.Select_Boss == "Beautiful Pirate [Lv. 1950] [Boss]" then
					MsBoss = "Beautiful Pirate [Lv. 1950] [Boss]"
					NameBoss = "Beautiful Pirate"
					NameQuestBoss = "DeepForestIsland2"             
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-12686, 391, -9902)
					CFrameBoss = CFrame.new(5182, 23, -20)
				elseif _G.Select_Boss == "Cake Queen [Lv. 2175] [Boss]" then
					MsBoss = "Cake Queen [Lv. 2175] [Boss]"
					NameBoss = "Cake Queen"
					NameQuestBoss = "IceCreamIslandQuest"             
					LevelQuestBoss = 3
					CFrameQuestBoss = CFrame.new(-716, 382, -11010)
					CFrameBoss = CFrame.new(-821, 66, -10965)
				elseif _G.Select_Boss == "rip_indra True Form [Lv. 5000] [Raid Boss]" then
					MsBoss = "rip_indra True Form [Lv. 5000] [Raid Boss]"
					NameBoss = "rip_indra True Form"
					CFrameBoss = CFrame.new(-5359, 424, -2735)
				elseif _G.Select_Boss == "Longma [Lv. 2000] [Boss]" then
					MsBoss = "Longma [Lv. 2000] [Boss]"
					NameBoss = "Longma"
					CFrameBoss = CFrame.new(-10248.3936, 353.79129, -9306.34473)
				elseif _G.Select_Boss == "Soul Reaper [Lv. 2100] [Raid Boss]" then
					MsBoss = "Soul Reaper [Lv. 2100] [Raid Boss]"
					NameBoss = "Soul Reaper"
					CFrameBoss = CFrame.new(-9515.62109, 315.925537, 6691.12012)
				end
			end		
	
		 function Hop()
				local PlaceID = game.PlaceId
				local AllIDs = {}
				local foundAnything = ""
				local actualHour = os.date("!*t").hour
				local Deleted = false
				function TPReturner()
					local Site;
					if foundAnything == "" then
						Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
					else
						Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
					end
					local ID = ""
					if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
						foundAnything = Site.nextPageCursor
					end
					local num = 0;
					for i,v in pairs(Site.data) do
						local Possible = true
						ID = tostring(v.id)
						if tonumber(v.maxPlayers) > tonumber(v.playing) then
							for _,Existing in pairs(AllIDs) do
								if num ~= 0 then
									if ID == tostring(Existing) then
										Possible = false
									end
								else
									if tonumber(actualHour) ~= tonumber(Existing) then
										local delFile = pcall(function()
											AllIDs = {}
											table.insert(AllIDs, actualHour)
										end)
									end
								end
								num = num + 1
							end
							if Possible == true then
								table.insert(AllIDs, ID)
								wait()
								pcall(function()
									wait()
									game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
								end)
								wait(4)
							end
						end
					end
				end
				function Teleport() 
					while wait() do
						pcall(function()
							TPReturner()
							if foundAnything ~= "" then
								TPReturner()
							end
						end)
					end
				end
				Teleport()
			end                   
		  function isnil(thing)
				return (thing == nil)
			end
			local function round(n)
				return math.floor(tonumber(n) + 0.5)
			end
			Number = math.random(1, 1000000)
			function UpdatePlayerChams()
				for i,v in pairs(game:GetService'Players':GetChildren()) do
					pcall(function()
						if not isnil(v.Character) then
							if ESPPlayer then
								if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp'..Number) then
									local bill = Instance.new('BillboardGui',v.Character.Head)
									bill.Name = 'NameEsp'..Number
									bill.ExtentsOffset = Vector3.new(0, 1, 0)
									bill.Size = UDim2.new(1,200,1,30)
									bill.Adornee = v.Character.Head
									bill.AlwaysOnTop = true
									local name = Instance.new('TextLabel',bill)
									name.Font = "GothamSemibold"
									name.FontSize = "Size14"
									name.TextWrapped = true
									name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
									name.Size = UDim2.new(1,0,1,0)
									name.TextYAlignment = 'Top'
									name.BackgroundTransparency = 1
									name.TextStrokeTransparency = 0.5
									if v.Team == game.Players.LocalPlayer.Team then
										name.TextColor3 = Color3.new(0,255,0)
									else
										name.TextColor3 = Color3.new(255,0,0)
									end
								else
									v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..' | '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M \n Health : ' .. round(v.Character.Humanoid.Health*100/v.Character.Humanoid.MaxHealth) .. '% Energy : ' .. round(v.Character.Energy.Value*100/v.Character.Energy.MaxValue) ..'%')
								end
							else
								if v.Character.Head:FindFirstChild('NameEsp'..Number) then
									v.Character.Head:FindFirstChild('NameEsp'..Number):Destroy()
								end
							end
						end
					end)
				 end
			  end
			function UpdateDiamondChestESP()
				for i,v in pairs(game:GetService("Workspace").Map.MysticIsland.Chests:GetChildren()) do
					pcall(function()
						if DiamondChestESP then 
							if v.Name == "DiamondChest" then
								if not v:FindFirstChild('NameEsp') then
									local bill = Instance.new('BillboardGui',v)
									bill.Name = 'NameEsp'
									bill.ExtentsOffset = Vector3.new(0, 1, 0)
									bill.Size = UDim2.new(1,200,1,30)
									bill.Adornee = v
									bill.AlwaysOnTop = true
									local name = Instance.new('TextLabel',bill)
									name.Font = "GothamSemibold"
									name.FontSize = "Size14"
									name.TextWrapped = true
									name.Size = UDim2.new(1, 1, 1)
									name.TextColor3 = Color3.fromRGB(0, 85, 255)
									name.TextYAlignment = 'Top'
									name.BackgroundTransparency = 1
									name.TextStrokeTransparency = 0.5
								else
									v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
								end
							end
						else
							if v:FindFirstChild('NameEsp') then
								v:FindFirstChild('NameEsp'):Destroy()
							end
						end
					end)
				end
			end
			function UpdateFragChestESP()
				for i,v in pairs(game:GetService("Workspace").Map.MysticIsland.Chests:GetChildren()) do
					pcall(function()
						if FragESP then 
							if v.Name == "FragChest" then
								if not v:FindFirstChild('NameEsp') then
									local bill = Instance.new('BillboardGui',v)
									bill.Name = 'NameEsp'
									bill.ExtentsOffset = Vector3.new(0, 1, 0)
									bill.Size = UDim2.new(1,200,1,30)
									bill.Adornee = v
									bill.AlwaysOnTop = true
									local name = Instance.new('TextLabel',bill)
									name.Font = "GothamSemibold"
									name.FontSize = "Size14"
									name.TextWrapped = true
									name.Size = UDim2.new(1, 1, 1)
									name.TextColor3 = Color3.fromRGB(170, 0, 255)
									name.TextYAlignment = 'Top'
									name.BackgroundTransparency = 1
									name.TextStrokeTransparency = 0.5
								else
									v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
								end
							end
						else
							if v:FindFirstChild('NameEsp') then
								v:FindFirstChild('NameEsp'):Destroy()
							end
						end
					end)
				end
			end
			function UpdateMirageIslandChams() 
				for i,v in pairs(game:GetService("Workspace").Map:GetChildren()) do
					pcall(function()
						if MirageIslandESP then
							if string.find(v.Name,"MysticIsland") then   
								if not v.Center:FindFirstChild('NameEsp'..Number) then
									local bill = Instance.new('BillboardGui',v.Center)
									bill.Name = 'NameEsp'..Number
									bill.ExtentsOffset = Vector3.new(0, 1, 0)
									bill.Size = UDim2.new(1,200,1,30)
									bill.Adornee = v.Center
									bill.AlwaysOnTop = true
									local name = Instance.new('TextLabel',bill)
									name.Font = "GothamSemibold"
									name.FontSize = "Size14"
									name.TextWrapped = true
									name.Size = UDim2.new(1,0,1,0)
									name.TextYAlignment = 'Top'
									name.BackgroundTransparency = 1
									name.TextStrokeTransparency = 0.5
									name.TextColor3 = Color3.fromRGB(255, 0, 0)
									name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Center.Position).Magnitude/3) ..' M')
								else
									v.Center['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Center.Position).Magnitude/3) ..' M')
								end
							end
						else
							if v.Center:FindFirstChild('NameEsp'..Number) then
								v.Center:FindFirstChild('NameEsp'..Number):Destroy()
							end
						end
					end)
				end
			end
			function UpdatenpcspawnESP()
				for i,v in pairs(game:GetService("Workspace").Map.MysticIsland.npcspawn:GetChildren()) do
					pcall(function()
						if npcspawnESP then 
							if v.Name ~= "npcSpawn" then
								if not v:FindFirstChild('NameEsp') then
									local bill = Instance.new('BillboardGui',v)
									bill.Name = 'NameEsp'
									bill.ExtentsOffset = Vector3.new(0, 1, 0)
									bill.Size = UDim2.new(1,200,1,30)
									bill.Adornee = v
									bill.AlwaysOnTop = true
									local name = Instance.new('TextLabel',bill)
									name.Font = "GothamSemibold"
									name.FontSize = "Size14"
									name.TextWrapped = true
									name.Size = UDim2.new(1, 1, 1)
									name.TextColor3 = Color3.fromRGB(80, 245, 245)
									name.TextYAlignment = 'Top'
									name.BackgroundTransparency = 1
									name.TextStrokeTransparency = 0.5
								else
									v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
								end
							end
						else
							if v:FindFirstChild('NameEsp') then
								v:FindFirstChild('NameEsp'):Destroy()
							end
						end
					end)
				end
			end
			function UpdateSeaBeastsESP()
				for i,v in pairs(game:GetService("Workspace").SeaBeasts:GetChildren()) do
					pcall(function()
						if SeaBeastsESP then
							if string.find(v.Name,"SeaBeast") then
								if not v.HumanoidRootPart:FindFirstChild('NameEsp'..Number) then
									local bill = Instance.new('BillboardGui',v.HumanoidRootPart)
									bill.Name = 'NameEsp'..Number
									bill.ExtentsOffset = Vector3.new(0, 1, 0)
									bill.Size = UDim2.new(1,200,1,30)
									bill.Adornee = v.HumanoidRootPart
									bill.AlwaysOnTop = true
									local name = Instance.new('TextLabel',bill)
									name.Font = "GothamSemibold"
									name.FontSize = "Size14"
									name.TextWrapped = true
									name.Size = UDim2.new(1,0,1,0)
									name.TextYAlignment = 'Top'
									name.BackgroundTransparency = 1
									name.TextStrokeTransparency = 0.5
									name.TextColor3 = Color3.fromRGB(255, 0, 0)
									name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.HumanoidRootPart.Position).Magnitude/3) ..' M')
								else
									v.HumanoidRootPart['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.HumanoidRootPart.Position).Magnitude/3) ..' M')
								end
							end
						else
							if v.HumanoidRootPart:FindFirstChild('NameEsp'..Number) then
								v.HumanoidRootPart:FindFirstChild('NameEsp'..Number):Destroy()
							end
						end
					end)
				end
			end
		  function UpdateIslandESP() 
				for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
					pcall(function()
						if IslandESP then 
							if v.Name ~= "Sea" then
								if not v:FindFirstChild('NameEsp') then
									local bill = Instance.new('BillboardGui',v)
									bill.Name = 'NameEsp'
									bill.ExtentsOffset = Vector3.new(0, 1, 0)
									bill.Size = UDim2.new(1,200,1,30)
									bill.Adornee = v
									bill.AlwaysOnTop = true
									local name = Instance.new('TextLabel',bill)
									name.Font = "GothamSemibold"
									name.FontSize = "Size14"
									name.TextWrapped = true
									name.Size = UDim2.new(1,0,1,0)
									name.TextYAlignment = 'Top'
									name.BackgroundTransparency = 1
									name.TextStrokeTransparency = 0.5
									name.TextColor3 = Color3.fromRGB(80, 245, 245)
								else
									v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
								end
							end
						else
							if v:FindFirstChild('NameEsp') then
								v:FindFirstChild('NameEsp'):Destroy()
							end
						end
					end)
				end
			end
			function UpdateChestEsp() 
				for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
					pcall(function()
						if string.find(v.Name,"Chest") then
							if ChestESP then
								if string.find(v.Name,"Chest") then
									if not v:FindFirstChild('NameEsp'..Number) then
										local bill = Instance.new('BillboardGui',v)
										bill.Name = 'NameEsp'..Number
										bill.ExtentsOffset = Vector3.new(0, 1, 0)
										bill.Size = UDim2.new(1,200,1,30)
										bill.Adornee = v
										bill.AlwaysOnTop = true
										local name = Instance.new('TextLabel',bill)
										name.Font = "GothamSemibold"
										name.FontSize = "Size14"
										name.TextWrapped = true
										name.Size = UDim2.new(1,0,1,0)
										name.TextYAlignment = 'Top'
										name.BackgroundTransparency = 1
										name.TextStrokeTransparency = 0.5
									if v.Name == "Chest1" then
										name.Text = ("Chest 1" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
										name.TextColor3 = Color3.fromRGB(85, 85, 127)
									end
									if v.Name == "Chest2" then
										name.Text = ("Chest 2" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
										name.TextColor3 = Color3.fromRGB(255, 255, 0)
									end
								if v.Name == "Chest3" then
									name.Text = ("Chest 3" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
									name.TextColor3 = Color3.fromRGB(0, 0, 255)
								end
								else
									v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
								end
							end
						else
							if v:FindFirstChild('NameEsp'..Number) then
							v:FindFirstChild('NameEsp'..Number):Destroy()
							end
						end
						end
					end)
				end
			end
			function UpdateBfEsp() 
				for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
					pcall(function()
						if DevilFruitESP then
							if string.find(v.Name, "Fruit") then   
								if not v.Handle:FindFirstChild('NameEsp'..Number) then
									local bill = Instance.new('BillboardGui',v.Handle)
									bill.Name = 'NameEsp'..Number
									bill.ExtentsOffset = Vector3.new(0, 1, 0)
									bill.Size = UDim2.new(1,200,1,30)
									bill.Adornee = v.Handle
									bill.AlwaysOnTop = true
									local name = Instance.new('TextLabel',bill)
									name.Font = "GothamSemibold"
									name.FontSize = "Size14"
									name.TextWrapped = true
									name.Size = UDim2.new(1,0,1,0)
									name.TextYAlignment = 'Top'
									name.BackgroundTransparency = 1
									name.TextStrokeTransparency = 0.5
									name.TextColor3 = Color3.fromRGB(255, 0, 0)
									name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
								else
									v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
								end
							end
						else
							if v.Handle:FindFirstChild('NameEsp'..Number) then
								v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
							end
						end
					end)
				end
			end
			function UpdateFlowerEsp() 
				for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
					pcall(function()
						if v.Name == "Flower2" or v.Name == "Flower1" then
							if FlowerESP then 
								if not v:FindFirstChild('NameEsp'..Number) then
									local bill = Instance.new('BillboardGui',v)
									bill.Name = 'NameEsp'..Number
									bill.ExtentsOffset = Vector3.new(0, 1, 0)
									bill.Size = UDim2.new(1,200,1,30)
									bill.Adornee = v
									bill.AlwaysOnTop = true
									local name = Instance.new('TextLabel',bill)
									name.Font = "GothamSemibold"
									name.FontSize = "Size14"
									name.TextWrapped = true
									name.Size = UDim2.new(1,0,1,0)
									name.TextYAlignment = 'Top'
									name.BackgroundTransparency = 1
									name.TextStrokeTransparency = 0.5
									name.TextColor3 = Color3.fromRGB(255, 0, 0)
								if v.Name == "Flower1" then 
									name.Text = ("Blue Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
									name.TextColor3 = Color3.fromRGB(0, 0, 255)
								end
								if v.Name == "Flower2" then
									name.Text = ("Red Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
									name.TextColor3 = Color3.fromRGB(255, 0, 0)
								end
							else
								v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
							end
							else
								if v:FindFirstChild('NameEsp'..Number) then
									v:FindFirstChild('NameEsp'..Number):Destroy()
								end
							end
						end   
					end)
				end
			end
			function UpdateRealFruitChams() 
				for i,v in pairs(game.Workspace.AppleSpawner:GetChildren()) do
					if v:IsA("Tool") then
						if RealFruitESP then 
							if not v.Handle:FindFirstChild('NameEsp'..Number) then
								local bill = Instance.new('BillboardGui',v.Handle)
								bill.Name = 'NameEsp'..Number
								bill.ExtentsOffset = Vector3.new(0, 1, 0)
								bill.Size = UDim2.new(1,200,1,30)
								bill.Adornee = v.Handle
								bill.AlwaysOnTop = true
								local name = Instance.new('TextLabel',bill)
								name.Font = "GothamSemibold"
								name.FontSize = "Size14"
								name.TextWrapped = true
								name.Size = UDim2.new(1,0,1,0)
								name.TextYAlignment = 'Top'
								name.BackgroundTransparency = 1
								name.TextStrokeTransparency = 0.5
								name.TextColor3 = Color3.fromRGB(255, 0, 0)
								name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
							else
								v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..' '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
							end
						else
							if v.Handle:FindFirstChild('NameEsp'..Number) then
								v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
							end
						end 
					end
				end
				for i,v in pairs(game.Workspace.PineappleSpawner:GetChildren()) do
					if v:IsA("Tool") then
						if RealFruitESP then 
							if not v.Handle:FindFirstChild('NameEsp'..Number) then
								local bill = Instance.new('BillboardGui',v.Handle)
								bill.Name = 'NameEsp'..Number
								bill.ExtentsOffset = Vector3.new(0, 1, 0)
								bill.Size = UDim2.new(1,200,1,30)
								bill.Adornee = v.Handle
								bill.AlwaysOnTop = true
								local name = Instance.new('TextLabel',bill)
								name.Font = "GothamSemibold"
								name.FontSize = "Size14"
								name.TextWrapped = true
								name.Size = UDim2.new(1,0,1,0)
								name.TextYAlignment = 'Top'
								name.BackgroundTransparency = 1
								name.TextStrokeTransparency = 0.5
								name.TextColor3 = Color3.fromRGB(255, 174, 0)
								name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
							else
								v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..' '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
							end
						else
							if v.Handle:FindFirstChild('NameEsp'..Number) then
								v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
							end
						end 
					end
				end
				for i,v in pairs(game.Workspace.BananaSpawner:GetChildren()) do
					if v:IsA("Tool") then
						if RealFruitESP then 
							if not v.Handle:FindFirstChild('NameEsp'..Number) then
								local bill = Instance.new('BillboardGui',v.Handle)
								bill.Name = 'NameEsp'..Number
								bill.ExtentsOffset = Vector3.new(0, 1, 0)
								bill.Size = UDim2.new(1,200,1,30)
								bill.Adornee = v.Handle
								bill.AlwaysOnTop = true
								local name = Instance.new('TextLabel',bill)
								name.Font = "GothamSemibold"
								name.FontSize = "Size14"
								name.TextWrapped = true
								name.Size = UDim2.new(1,0,1,0)
								name.TextYAlignment = 'Top'
								name.BackgroundTransparency = 1
								name.TextStrokeTransparency = 0.5
								name.TextColor3 = Color3.fromRGB(251, 255, 0)
								name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
							else
								v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..' '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
							end
						else
							if v.Handle:FindFirstChild('NameEsp'..Number) then
								v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
							end
						end 
					end
				end
			end
		
			function AutoHaki()
				if not game:GetService("Players").LocalPlayer.Character:FindFirstChild("HasBuso") then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buso")
				end
			end
		
			function UnEquipWeapon(Weapon)
				if game.Players.LocalPlayer.Character:FindFirstChild(Weapon) then
					_G.NotAutoEquip = true
					wait(.5)
					game.Players.LocalPlayer.Character:FindFirstChild(Weapon).Parent = game.Players.LocalPlayer.Backpack
					wait(.1)
					_G.NotAutoEquip = false
				end
			end
		
			function EquipWeapon(ToolSe)
				if not _G.NotAutoEquip then
					if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
						Tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
						wait(.1)
						game.Players.LocalPlayer.Character.Humanoid:EquipTool(Tool)
					end
				end
			end
		
			function GetDistance(target)
				return math.floor((target.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude)
			end
		
		function Click()
			local VirtualUser = game:GetService('VirtualUser')
			VirtualUser:CaptureController()
			VirtualUser:ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
		end
		
			-- Get Weapon Sword
			spawn(function()
				while wait() do
					for i ,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
						if v:IsA("Tool") then
							if v.ToolTip == "Sword" then
								SelectToolWeaponSword = v.Name
							end
						end
					end
					for i ,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
						if v:IsA("Tool") then
							if v.ToolTip == "Sword" then
								SelectToolWeaponSword = v.Name
							end
						end
					end
				end
			end)
		
			-- Get Weapon Gun
			spawn(function()
				while wait() do
					for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
						if v:IsA("Tool") then
							if v:FindFirstChild("RemoteFunctionShoot") then 
								SelectToolWeaponGun = v.Name
							end
						end
					end
					for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
						if v:IsA("Tool") then
							if v:FindFirstChild("RemoteFunctionShoot") then 
								SelectToolWeaponGun = v.Name
							end
						end
					end
				end
			end)
		
			-- Get Weapon Melee
			spawn(function()
				while wait() do
					for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
						if v:IsA("Tool") then
							if v:FindFirstChild("Melee") then 
								SelectToolWeaponMelee = v.Name
							end
						end
					end
					for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
						if v:IsA("Tool") then
							if v:FindFirstChild("Melee") then 
								SelectToolWeaponMelee = v.Name
							end
						end
					end
				end
			end)
		
		-- [CheckMasteryWeapon]
		
		function CheckMasteryWeapon(NameWe,MasNum)
			if game.Players.LocalPlayer.Backpack:FindFirstChild(NameWe) then
				if tonumber(game.Players.LocalPlayer.Backpack:FindFirstChild(NameWe).Level.Value) < tonumber(MasNum) then
					return "true DownTo"
				elseif tonumber(game.Players.LocalPlayer.Backpack:FindFirstChild(NameWe).Level.Value) >= tonumber(MasNum) then
					return "true UpTo"
				end
			end
			if game.Players.LocalPlayer.Character:FindFirstChild(NameWe) then
				if tonumber(game.Players.LocalPlayer.Character:FindFirstChild(NameWe).Level.Value) < tonumber(MasNum) then
					return "true DownTo"
				elseif tonumber(game.Players.LocalPlayer.Character:FindFirstChild(NameWe).Level.Value) >= tonumber(MasNum) then
					return "true UpTo"
				end
			end
			return "else"
		end
		
		--[GetWeaponInventory]
		
		function GetWeaponInventory(Weaponname)
			for i,v in pairs(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getInventory")) do
				if type(v) == "table" then
					if v.Type == "Sword" then
						if v.Name == Weaponname then
							return true
						end
					end
				end
			end
			return false
		end
		
		-- [GetMaterial]
		
		function GetMaterial(matname)
			for i,v in pairs(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getInventory")) do
				if type(v) == "table" then
					if v.Type == "Material" then
						if v.Name == matname then
							return v.Count
						end
					end
				end
			end
			return 0
		end

-- [Isnetwork Owner]

function InMyNetWork(object)
	if isnetworkowner then
		return isnetworkowner(object)
	else
		if (object.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 200 then 
			return true
		end
		return false
	end
end

-- [Function (Abandoned Quest , Others)]

function Com(com,...)
	local Remote = game:GetService('ReplicatedStorage').Remotes:FindFirstChild("Comm"..com)
	if Remote:IsA("RemoteEvent") then
		Remote:FireServer(...)
	elseif Remote:IsA("RemoteFunction") then
		Remote:InvokeServer(...)
	end
end

	-- [CheckMaterial]
	
	local function CheckMaterial(v1)
		if World1 then 
			if (v1=="Magma Ore") then 
				MaterialMob={"Military Soldier [Lv. 300]","Military Spy [Lv. 325]"}
				CFrameMon=CFrame.new( -5815,84,8820)
			elseif ((v1=="Leather") or (v1=="Scrap Metal")) then 
				MaterialMob={"Brute [Lv. 45]"}
				CFrameMon=CFrame.new( -1145,15,4350)
			elseif (v1=="Angel Wings") then 
				MaterialMob={"God's Guard [Lv. 450]"}
				CFrameMon=CFrame.new( -4698,845, -1912)
			elseif (v1=="Fish Tail") then 
				MaterialMob={"Fishman Warrior [Lv. 375]","Fishman Commando [Lv. 400]"}
				CFrameMon=CFrame.new(61123,19,1569);
			end 
		end 
		if World2 then 
			if (v1=="Magma Ore") then 
				MaterialMob={"Magma Ninja [Lv. 1175]"}
				CFrameMon=CFrame.new( -5428,78, -5959)
			elseif (v1=="Scrap Metal") then
				MaterialMob={"Swan Pirate [Lv. 775]"}
				CFrameMon=CFrame.new(878,122,1235)
			elseif (v1=="Radioactive Material") then 
				MaterialMob={"Factory Staff [Lv. 800]"}
				CFrameMon=CFrame.new(295,73, -56)
			elseif (v1=="Vampire Fang") then 
				MaterialMob={"Vampire [Lv. 975]"}
				CFrameMon=CFrame.new( -6033,7, -1317)
			elseif (v1=="Mystic Droplet") then 
				MaterialMob={"Water Fighter [Lv. 1450]","Sea Soldier [Lv. 1425]"}
				CFrameMon=CFrame.new( -3385,239, -10542)
			end 
		end 
		if World3 then 
			if (v1=="Mini Tusk") then 
				MaterialMob={"Mythological Pirate [Lv. 1850]"}
				CFrameMon=CFrame.new( -13545,470, -6917)
			elseif (v1=="Fish Tail") then 
				MaterialMob={"Fishman Raider [Lv. 1775]","Fishman Captain [Lv. 1800]"}
				CFrameMon=CFrame.new( -10993,332, -8940)
			elseif (v1=="Scrap Metal") then 
				MaterialMob={"Jungle Pirate [Lv. 1900]"}
				CFrameMon=CFrame.new( -12107,332, -10549)
			elseif (v1=="Dragon Scale") then 
				MaterialMob={"Dragon Crew Archer [Lv. 1600]","Dragon Crew Warrior [Lv. 1575]"}
				CFrameMon=CFrame.new(6594,383,139)
			elseif (v1=="Conjured Cocoa") then 
				MaterialMob={"Cocoa Warrior [Lv. 2300]","Chocolate Bar Battler [Lv. 2325]","Sweet Thief [Lv. 2350]","Candy Rebel [Lv. 2375]"}
				CFrameMon=CFrame.new(620.6344604492188,78.93644714355469, -12581.369140625)
			elseif (v1=="Demonic Wisp") then MaterialMob={"Demonic Soul [Lv. 2025]"}
				CFrameMon=CFrame.new( -9507,172,6158)
			elseif (v1=="Gunpowder") then MaterialMob={"Pistol Billionaire [Lv. 1525]"}
				CFrameMon=CFrame.new( -469,74,5904)
			end 
		end 
	end
	
	-- [CheckMaterial]
	
	local function CheckMaterial(v1)
		if World1 then 
			if (v1=="Magma Ore") then 
				MaterialMob = {"Military Soldier [Lv. 300]","Military Spy [Lv. 325]"};
				CFrameMon=CFrame.new( -5815,84,8820);
			elseif ((v1=="Leather") or (v1=="Scrap Metal")) then 
				MaterialMob = {"Brute [Lv. 45]"};
				CFrameMon=CFrame.new( -1145,15,4350);
			elseif (v1=="Angel Wings") then 
				MaterialMob = {"God's Guard [Lv. 450]"};
				CFrameMon=CFrame.new( -4698,845, -1912);
			elseif (v1=="Fish Tail") then 
				MaterialMob = {"Fishman Warrior [Lv. 375]","Fishman Commando [Lv. 400]"};
				CFrameMon=CFrame.new(61123,19,1569);
			end 
		end 
		if World2 then 
			if (v1=="Magma Ore") then 
				MaterialMob={"Magma Ninja [Lv. 1175]"};
				CFrameMon=CFrame.new( -5428,78, -5959);
			elseif (v1=="Scrap Metal") then
				MaterialMob={"Swan Pirate [Lv. 775]"};
				CFrameMon=CFrame.new(878,122,1235);
			elseif (v1=="Radioactive Material") then 
				MaterialMob={"Factory Staff [Lv. 800]"};
				CFrameMon=CFrame.new(295,73, -56);
			elseif (v1=="Vampire Fang") then 
				MaterialMob={"Vampire [Lv. 975]"};
				CFrameMon=CFrame.new( -6033,7, -1317);
			elseif (v1=="Mystic Droplet") then 
				MaterialMob={"Water Fighter [Lv. 1450]","Sea Soldier [Lv. 1425]"};
				CFrameMon=CFrame.new( -3385,239, -10542);
			end 
		end 
		if World3 then 
			if (v1=="Mini Tusk") then 
				MaterialMob={"Mythological Pirate [Lv. 1850]"};
				CFrameMon=CFrame.new( -13545,470, -6917);
			elseif (v1=="Fish Tail") then 
				MaterialMob={"Fishman Raider [Lv. 1775]","Fishman Captain [Lv. 1800]"};
				CFrameMon=CFrame.new( -10993,332, -8940);
			elseif (v1=="Scrap Metal") then 
				MaterialMob={"Jungle Pirate [Lv. 1900]"};
				CFrameMon=CFrame.new( -12107,332, -10549);
			elseif (v1=="Dragon Scale") then 
				MaterialMob={"Dragon Crew Archer [Lv. 1600]","Dragon Crew Warrior [Lv. 1575]"};
				CFrameMon=CFrame.new(6594,383,139);
			elseif (v1=="Conjured Cocoa") then 
				MaterialMob={"Cocoa Warrior [Lv. 2300]","Chocolate Bar Battler [Lv. 2325]","Sweet Thief [Lv. 2350]","Candy Rebel [Lv. 2375]"};
				CFrameMon=CFrame.new(620.6344604492188,78.93644714355469, -12581.369140625);
			elseif (v1=="Demonic Wisp") then MaterialMob ={ "Demonic Soul [Lv. 2025]"};
				CFrameMon=CFrame.new( -9507,172,6158);
			elseif (v1=="Gunpowder") then MaterialMob={"Pistol Billionaire [Lv. 1525]"};
				CFrameMon=CFrame.new( -469,74,5904);
			end 
		end 
	end

-- [Get FightingStyle]

function GetFightingStyle(Style)
	ReturnText = ""
	for i ,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
		if v:IsA("Tool") then
			if v.ToolTip == Style then
				ReturnText = v.Name
			end
		end
	end
	for i ,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
		if v:IsA("Tool") then
			if v.ToolTip == Style then
				ReturnText = v.Name
			end
		end
	end
	if ReturnText ~= "" then
		return ReturnText
	else
		return "Not Have"
	end
end
	
		-- Tween
	
		function TP(Pos)
			Distance = (Pos.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
			if game.Players.LocalPlayer.Character.Humanoid.Sit == true then game.Players.LocalPlayer.Character.Humanoid.Sit = false end
			pcall(function() tween = game:GetService("TweenService"):Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(Distance/_G.TweenSpeed, Enum.EasingStyle.Linear),{CFrame = Pos}) end)
			tween:Play()
			if Distance <= 250 then
				tween:Cancel()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = Pos
			end
			if _G.StopTween == true then
				tween:Cancel()
				_G.Clip = false
			end
		end
	
		function TP2(targetPos, targetCFrame)
			local tweenfunc = {}
			local tween_s = game:service"TweenService"
			local info = TweenInfo.new((targetPos - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).Magnitude/_G.TweenSpeed, Enum.EasingStyle.Linear)
			local tween = tween_s:Create(game:GetService("Players").LocalPlayer.Character["HumanoidRootPart"], info, {CFrame = targetCFrame * CFrame.fromAxisAngle(Vector3.new(1,0,0), math.rad(0))})
			tween:Play()
			function tweenfunc:Stop()
				tween:Cancel()
			end 
			if not tween then return tween end
			return tweenfunc
		end
	
		function tweenteleport(Speed,Part)
			local Distancex = (Vector3.new(Part) - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
		local Speexd = Speed
		tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
		tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(Part)})
		tweenx:Play()
		wait(Distancex/Speexd)
		end
		game:GetService("RunService").Heartbeat:Connect(function()
		pcall(function()
		CheckLevel()
		if not game.Workspace:FindFirstChild(NameMon) then
		   local part = Instance.new("Part")
		   part.Name = NameMon
		   part.Position = Vector3.new(0, 10, 0)
		   part.Anchored = true
		   part.CFrame = CFrameQuest
		   part.Transparency = 1
		   part.Parent = game.Workspace
		end
		CheckLevel()
		if not game.Workspace:FindFirstChild(Ms) then
		   local part = Instance.new("Part")
		   part.Name = Ms
		   part.Position = Vector3.new(0, 10, 0)
		   part.Anchored = true
		   part.CFrame = CFrameMon
		   part.Transparency = 1
		   part.Parent = game.Workspace
		end
		end)
		end)
		
		 function StopTween(target)
			 if not target then
				 _G.StopTween = true
				 wait()
				 TP(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
				 wait()
				 if game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
					 game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip"):Destroy()
				 end
				 _G.StopTween = false
				 _G.Clip = false
			 end
		 end
		 
			function Moon()
				if World3 then
					local Moon = {
					['8'] = "http://www.roblox.com/asset/?id=9709149431", -- 🌕
					['7'] = "http://www.roblox.com/asset/?id=9709149052", -- 🌖
					['6'] = "http://www.roblox.com/asset/?id=9709143733", -- 🌗
					['5'] = "http://www.roblox.com/asset/?id=9709150401", -- 🌘
					['4'] = "http://www.roblox.com/asset/?id=9709135895",  -- 🌑
					['3'] = "http://www.roblox.com/asset/?id=9709139597", -- 🌒
					['2'] = "http://www.roblox.com/asset/?id=9709150086", -- 🌓
					['1'] = "http://www.roblox.com/asset/?id=9709149680", -- 🌔
					};
					for i,v in pairs(Moon) do
						if game:GetService("Lighting").Sky.MoonTextureId == v then
							MoonPercent = i / 8 * 100
						end
					end
					
					for i,v in pairs(game.Players:GetPlayers()) do
						PlayersMin = i
					end
					
					if game:GetService("Lighting").Sky.MoonTextureId == Moon['1'] then
						MoonIcon = '🌔'
					elseif game:GetService("Lighting").Sky.MoonTextureId == Moon['2'] then
						MoonIcon = '🌓'
					elseif game:GetService("Lighting").Sky.MoonTextureId == Moon['3'] then
						MoonIcon = '🌒'
					elseif game:GetService("Lighting").Sky.MoonTextureId == Moon['4'] then
						MoonIcon = '🌑'
					elseif game:GetService("Lighting").Sky.MoonTextureId == Moon['5'] then
						MoonIcon = '🌘'
					elseif game:GetService("Lighting").Sky.MoonTextureId == Moon['6'] then
						MoonIcon = '🌗'
					elseif game:GetService("Lighting").Sky.MoonTextureId == Moon['7'] then
						MoonIcon = '🌖'
					elseif game:GetService("Lighting").Sky.MoonTextureId == Moon['8'] then
						MoonIcon = '🌕'
					end
					if game.Workspace._WorldOrigin.Locations:FindFirstChild('Mirage Island') then
						MirageMessage = '```Mirage is spawing : ✔```'
					else
						MirageMessage = '```Mirage isn\'t spawn : ❌```'
					end
					
					MoonMessage = '```'..tostring(MoonPercent..'%'..' : '..MoonIcon)..'```'
					JoinServer = 'game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId,'..'\''..tostring(game.JobId)..'\''..')'
					
					local url = "https://discord.com/api/webhooks/1077795090652733491/G26JuPnE0YKk8B8PHSaPtdrUSkoA-ED7YujDm5KQaQUVyBkQQHlyLGxzTFkSAx-ShCNG" -- ur webhook url
					local data = {
						["username"] = 'Pado Hub', -- Webhook name here
						['content'] = '', -- ping everyone if you want to ping role use this <@&1007291553074647132> 
						["avatar_url"] = "https://cdn.discordapp.com/attachments/1031070093486075944/1077797553128620062/11804855180.png", -- ur discord logo url
						["embeds"] = {
							{
								["description"] = "**__Moon and Mirage Webhook__**",
								["color"] = tonumber(0xff0000), -- color id		
								["type"] = "rich",
								["fields"] =  {
									{
										["name"] = "[👥] Players Active",
										["value"] = '```'..tostring(PlayersMin)..'/12```'
									},
									{
										["name"] = "[📃] JobID",
										["value"] = '```'..tostring(game.JobId)..'```'
									},
									{
										["name"] = "[📁] Join Server",
										["value"] = '```'..JoinServer..'```',
									},
									{
										["name"] = "[🕑] Moon Check",
										["value"] = MoonMessage,
									},
									{   ["name"] = "[🏝️] Mirage Check",
										["value"] = MirageMessage,
									}
								},
								["footer"] = {
									["text"] = "Webhook", -- you can remove this but it will hurt
								},
								["timestamp"] = DateTime.now():ToIsoDate(),
							}
						},
					}
					local newdata = game:GetService("HttpService"):JSONEncode(data)
					local headers = {["content-type"] = "application/json"}
					request = http_request or request or HttpPost or syn.request
					local abcdef = {Url = url, Body = newdata, Method = "POST", Headers = headers}
					request(abcdef)
					end
					end
	
			function DoughKing()
				if World3 then
					for i,v in pairs(game.Players:GetPlayers()) do
						PlayersMin = i
					end
		
					if game.ReplicatedStorage:FindFirstChild("Dough King [Lv. 2300] [Raid Boss]") then
						DoughKingMessage = '```Dough King is spawing : ✔```'
					else
						DoughKingMessage = '```Dough King isn\'t spawn : ❌```'
					end
					
					JoinServer = 'game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId,'..'\''..tostring(game.JobId)..'\''..')'
					
					local url = "https://discord.com/api/webhooks/1082287404880236605/S4EbRMlZ54KYiEz9T2LQ24OOudIJ9xq0_XLbzKLLCYdGPwKFV8uyZqLptlVOoFDa0N5C" -- ur webhook url
					local data = {
						["username"] = 'Pado Hub', -- Webhook name here
						['content'] = '', -- ping everyone if you want to ping role use this <@&1007291553074647132> 
						["avatar_url"] = "https://cdn.discordapp.com/attachments/1031070093486075944/1077797553128620062/11804855180.png", -- ur discord logo url
						["embeds"] = {
							{
								["description"] = "**__Webhook__**",
								["color"] = tonumber(0xff0000), -- color id		
								["type"] = "rich",
								["fields"] =  {
									{
										["name"] = "[👥] Players Active",
										["value"] = '```'..tostring(PlayersMin)..'/12```'
									},
									{
										["name"] = "[📃] JobID",
										["value"] = '```'..tostring(game.JobId)..'```'
									},
									{
										["name"] = "[📁] Join Server",
										["value"] = '```'..JoinServer..'```',
									},
									{   ["name"] = "[⚔️] Dough King Check",
										["value"] = DoughKingMessage,
									}
								},
								["footer"] = {
									["text"] = "Webhook", -- you can remove this but it will hurt
								},
								["timestamp"] = DateTime.now():ToIsoDate(),
							}
						},
					}
					local newdata = game:GetService("HttpService"):JSONEncode(data)
					local headers = {["content-type"] = "application/json"}
					request = http_request or request or HttpPost or syn.request
					local abcdef = {Url = url, Body = newdata, Method = "POST", Headers = headers}
					request(abcdef)
					end
				end
	
		 -- Back legv skill 
		
		 spawn(function()
			pcall(function()
				while wait(1) do
				 if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 150 or game.Players.LocalPlayer.Character:FindFirstChild("Death Step") and game.Players.LocalPlayer.Character:FindFirstChild("Death Step").Level.Value >= 400 then
					if _G.AutoBacklegv then
						game:service('VirtualInputManager'):SendKeyEvent(true, "V", false, game)
						game:service('VirtualInputManager'):SendKeyEvent(false, "V", false, game)
					end
				end
			end
		end)
	end)
	
		-- Body Clip

		spawn(function()
			game:GetService("RunService").Heartbeat:Connect(function()
				if _G.AutoPirateRaids or _G.AutoFarmtribe or Auto_Quest_Yama_3 or Tushita_Quest3 or Tushita_Quest2 or Observation or _G.Farm_Ob_Color or _G.Auto_Acidum_Rifle or _G.Auto_Soul_Reaper or _G.Auto_Dragon_Trident or _G.Auto_Spikey_Trident or _G.Triple_A or _G.AutoFarmCandy or _G.AutoHearts or _G.AutoFarmMaterial or _G.Mirage or _G.AutoFajita or _G.AutoLongsword or _G.BlackSpikeyCoat or _G.Position_Spawn or _G.AutoFarmChiefWardenIsland or _G.AutoFarmFishmanIsland or _G.Auto_Twin_Hook or _G.AutoYama or _G.AutoFarmCavander or _G.AutoNew or _G.HolyTorch or _G.AutoFarmKaitan or _G.AutoTushitaSword or _G.AutoOderSword or _G.AutoAdvanceDungeon or _G.AutoKaitan or _G.Auto_Farm_Level or _G.AutoSerpentBow or _G.AutoNewWorld2 or _G.AutoKaitan or _G.AutoQuestSoulGuitar or _G.AutoSeaBest or _G.AutoSaber or _G.AutoFarmSelectMonster or _G.AutoMysticIsland or _G.AutoFactory or _G.Auto_Open_Dough_Dungeon or _G.BlackBeard or _G.BlackBeardHop or _G.Auto_Raid_Hop or _G.Auto_Raid or _G.Next_Islands or _G.AutoPlayerHunter or _G.Auto_Kill_PlyDown or _G.Raid or _G.AutoEliteHunter or _G.BlackBeard or _G.Tushitahop or _G.AutoHakiRainbow or _G.AutoElectricClaw or _G.TeleportNPC or _G.AutoPole or _G.AutoMobAura or _G.AutoDoughtBoss or _G.Auto_DungeonMobAura or _G.AutoFarmChest or _G.AutoFarmBossHallow or _G.AutoFarmSwanGlasses or _G.AutoLongSword or _G.AutoBlackSpikeycoat or _G.AutoElectricClaw or _G.AutoFarmGunMastery or _G.AutoHolyTorch or _G.AutoLawRaid or _G.AutoFarmBoss or _G.AutoTwinHooks or _G.AutoOpenSwanDoor or _G.AutoDragon_Trident or _G.AutoSaber or _G.AutoFarmFruitMastery or _G.AutoFarmGunMastery or _G.TeleportIsland or _G.Auto_EvoRace or _G.AutoFarmAllMsBypassType or _G.AutoObservationv2 or _G.AutoMusketeerHat or _G.AutoEctoplasm or _G.AutoRengoku or _G.Auto_Rainbow_Haki or _G.AutoObservation or _G.AutoDarkDagger or _G.Safe_Mode or _G.MasteryFruit or _G.AutoBudySword or _G.AutoBounty or _G.AutoAllBoss or _G.Auto_Bounty or _G.AutoSharkman or _G.Auto_Mastery_Fruit or _G.Auto_Mastery_Gun or _G.Auto_Dungeon or _G.Auto_Cavender or _G.Auto_Pole or _G.Auto_Kill_Ply or _G.Auto_Factory or _G.AutoSecondSea or _G.TeleportPly or _G.AutoBartilo or _G.Auto_DarkBoss or _G.Auto_Bone or Grab_Chest or _G.AutoFarmBounty or _G.Clip or _G.AutoElitehunter or _G.AutoThirdSea then					
					if not game:GetService("Workspace"):FindFirstChild("LOL") then
						local LOL = Instance.new("Part")
						LOL.Name = "LOL"
						LOL.Parent = game.Workspace
						LOL.Anchored = true
						LOL.Transparency = 1
						LOL.Size = Vector3.new(30,-0.5,30)
					elseif game:GetService("Workspace"):FindFirstChild("LOL") then
						game.Workspace["LOL"].CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0, -3.6, 0)
					end
				else
					if game:GetService("Workspace"):FindFirstChild("LOL") then
						game:GetService("Workspace"):FindFirstChild("LOL"):Destroy()
					end
				end
			end)
		end)
		
		spawn(function() -- Tween 
			pcall(function()
				game:GetService("RunService").Stepped:Connect(function()
					if _G.AutoPirateRaids or _G.AutoFarmtribe or Auto_Quest_Yama_3 or Tushita_Quest3 or Tushita_Quest2 or Observation or _G.Farm_Ob_Color or _G.Auto_Acidum_Rifle or _G.Auto_Soul_Reaper or _G.Auto_Dragon_Trident or _G.Auto_Spikey_Trident or _G.Triple_A or _G.AutoFarmCandy or _G.AutoHearts or _G.AutoFarmMaterial or _G.Mirage or _G.AutoFajita or _G.AutoLongsword or _G.BlackSpikeyCoat or _G.Position_Spawn or _G.AutoFarmChiefWardenIsland or _G.AutoFarmFishmanIsland or _G.Auto_Twin_Hook or _G.AutoYama or _G.AutoFarmCavander or _G.AutoNew or _G.HolyTorch or _G.AutoFarmKaitan or _G.AutoTushitaSword or _G.AutoOderSword or _G.AutoAdvanceDungeon or _G.AutoKaitan or _G.Auto_Farm_Level or _G.AutoSerpentBow or _G.AutoNewWorld2 or _G.AutoKaitan or _G.AutoQuestSoulGuitar or _G.AutoSeaBest or _G.AutoSaber or _G.AutoFarmSelectMonster or _G.AutoMysticIsland or _G.AutoFactory or _G.Auto_Open_Dough_Dungeon or _G.BlackBeard or _G.BlackBeardHop or _G.Auto_Raid_Hop or _G.Auto_Raid or _G.Next_Islands or _G.AutoPlayerHunter or _G.Auto_Kill_PlyDown or _G.Raid or _G.AutoEliteHunter or _G.BlackBeard or _G.Tushitahop or _G.AutoHakiRainbow or _G.AutoElectricClaw or _G.TeleportNPC or _G.AutoPole or _G.AutoMobAura or _G.AutoDoughtBoss or _G.Auto_DungeonMobAura or _G.AutoFarmChest or _G.AutoFarmBossHallow or _G.AutoFarmSwanGlasses or _G.AutoLongSword or _G.AutoBlackSpikeycoat or _G.AutoElectricClaw or _G.AutoFarmGunMastery or _G.AutoHolyTorch or _G.AutoLawRaid or _G.AutoFarmBoss or _G.AutoTwinHooks or _G.AutoOpenSwanDoor or _G.AutoDragon_Trident or _G.AutoSaber or _G.AutoFarmFruitMastery or _G.AutoFarmGunMastery or _G.TeleportIsland or _G.Auto_EvoRace or _G.AutoFarmAllMsBypassType or _G.AutoObservationv2 or _G.AutoMusketeerHat or _G.AutoEctoplasm or _G.AutoRengoku or _G.Auto_Rainbow_Haki or _G.AutoObservation or _G.AutoDarkDagger or _G.Safe_Mode or _G.MasteryFruit or _G.AutoBudySword or _G.AutoBounty or _G.AutoAllBoss or _G.Auto_Bounty or _G.AutoSharkman or _G.Auto_Mastery_Fruit or _G.Auto_Mastery_Gun or _G.Auto_Dungeon or _G.Auto_Cavender or _G.Auto_Pole or _G.Auto_Kill_Ply or _G.Auto_Factory or _G.AutoSecondSea or _G.TeleportPly or _G.AutoBartilo or _G.Auto_DarkBoss or _G.Auto_Bone or Grab_Chest or _G.AutoFarmBounty or _G.Clip or _G.AutoElitehunter or _G.AutoThirdSea then					
					  if not game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
						local Noclip = Instance.new("BodyVelocity")
						Noclip.Name = "BodyClip"
						Noclip.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
						Noclip.MaxForce = Vector3.new(100000,100000,100000)
						Noclip.Velocity = Vector3.new(0,0,0)
					end
					for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
						if v:IsA("BasePart") then
							v.CanCollide = false  
						end
					end
				else	
					if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
							game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip"):Destroy()
						end
					end
				end)
			end)
		end)

     -- logo meun 
     
		local PADOXHUBMODILE = Instance.new("ScreenGui")
		local MODILEGUIPADOXHUB = Instance.new("TextButton")
		local MODILEGUIPADOXHUBHUI = Instance.new("UICorner")
		local MODILEMAGE = Instance.new("ImageLabel")
		
		MODILEGUIPADOXHUBHUI.Name = "MODILEGUIPADOXHUBHUI"
		MODILEGUIPADOXHUBHUI.Parent = MODILEGUIPADOXHUB
		
		MODILEMAGE.Name = "MODILEMAGE"
		MODILEMAGE.Parent = MODILEGUIPADOXHUB
		MODILEMAGE.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		MODILEMAGE.BackgroundTransparency = 1.000
		MODILEMAGE.BorderSizePixel = 0
		MODILEMAGE.Position = UDim2.new(-0.005, 0,-0.001, 0)
		MODILEMAGE.Size = UDim2.new(0, 50, 0, 50)
		MODILEMAGE.Image = "http://www.roblox.com/asset/?id=11804855180"
		
		PADOXHUBMODILE.Name = "PADOXHUBMODILE"
		PADOXHUBMODILE.Parent = game.CoreGui
		PADOXHUBMODILE.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
		
		MODILEGUIPADOXHUB.Name = "MODILEGUIPADOXHUB"
		MODILEGUIPADOXHUB.Parent = PADOXHUBMODILE
		MODILEGUIPADOXHUB.BackgroundColor3 = Color3.fromRGB(30,20,20)
		MODILEGUIPADOXHUB.Position = UDim2.new(0, 0, 0.491228074, 0)
		MODILEGUIPADOXHUB.Size = UDim2.new(0, 50, 0, 50)
		MODILEGUIPADOXHUB.BackgroundTransparency = 1
		MODILEGUIPADOXHUB.BorderSizePixel = 0
		MODILEGUIPADOXHUB.Draggable = true
		MODILEGUIPADOXHUB.MouseButton1Click:Connect(function()
			game:GetService("VirtualInputManager"):SendKeyEvent(true,305,false,game)
			game:GetService("VirtualInputManager"):SendKeyEvent(false,305,false,game)
		end)
		
		-- UI
		
		    local Update = loadstring(game:HttpGet"https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Gui")()
		    local PadoUi = Update:Window("Pado",Enum.KeyCode.RightControl);
			local Main = PadoUi:Tab("General","6034744031")
			local Quest = PadoUi:Tab("Quest","6035056512")
			local AutoMisc = PadoUi:Tab("Settings","6034754439")
			local Race = PadoUi:Tab("Race","6035107920")
			local Combat = PadoUi:Tab("Combat","6022668881")
			local Stats = PadoUi:Tab("Stats","6035121912")
			local Teleport = PadoUi:Tab("Teleport","6035190846")
			local Dungeon = PadoUi:Tab("Dungeon","6035067839")
			local DevilFruit = PadoUi:Tab("Devil Fruit","6035145359")
			local Shop = PadoUi:Tab("Shop","6035161534")
			local Misc = PadoUi:Tab("Misc","6034509993")

			Main:Seperator("List Farm") -- Select Mon Auto Farm 
		
			if World1 then
				tableMon = {"Bandit","Monkey","Gorilla","Pirate","Brute","Desert Bandit","Desert Officer","Snow Bandit","Snowman","Chief Petty Officer","Sky Bandit","Dark Master","Toga Warrior","Gladiator","Military Soldier","Military Spy","Fishman Warrior","Fishman Commando","God's Guard","Shanda","Royal Squad","Royal Soldier","Galley Pirate","Galley Captain"}
			elseif World2 then
				tableMon = {"Raider","Mercenary","Swan Pirate","Factory Staff","Marine Lieutenant","Marine Captain","Zombie","Vampire","Snow Trooper","Winter Warrior","Lab Subordinate","Horned Warrior","Magma Ninja","Lava Pirate","Ship Deckhand","Ship Engineer","Ship Steward","Ship Officer","Arctic Warrior","Snow Lurker","Sea Soldier","Water Fighter"}
			elseif World3 then
				tableMon = {"Pirate Millionaire","Dragon Crew Warrior","Dragon Crew Archer","Female Islander","Giant Islander","Marine Commodore","Marine Rear Admiral","Fishman Raider","Fishman Captain","Forest Pirate","Mythological Pirate","Jungle Pirate","Musketeer Pirate","Reborn Skeleton","Living Zombie","Demonic Soul","Posessed Mummy","Peanut Scout","Peanut President","Ice Cream Chef","Baking Staff","Head Baker","Cocoa Warrior","Chocolate Bar Battler","Sweet Thief","Candy Rebel","Candy Pirate","Snow Demon","Isle Outlaw","Island Boy","Sun-kissed Warrior","Isle Champion"}
			end
		
		Main:Dropdown("Select Monster", tableMon, function(value)
			_G.SelectMonster = value
		end)
		
		_G.Select_Mode_Farm = "Normal Mode"
		
			Main:Dropdown("Select Mode Farm",{"Easy Mode","Normal Mode","Hard Mode","Fast Mode","No Quest","Mob Aura"},function(value)
					_G.Select_Mode_Farm = value
				end)
                                                                                                                                                                                                                                                                                                                                                                                                                                              
				_G.Method = "X-Y-Z"
	
				Main:Dropdown("Select Farm Method", {
					"Behind","Below","Upper","X-Y-Z"
				   },function(value)
					_G.Method = value
				end)

	spawn(function()
		while wait(1) do
			pcall(function()
				if _G.Method == "Behind" then
					Farm_Mode = CFrame.new(0,0,28)
				elseif _G.Method == "Below" then
				    Farm_Mode = CFrame.new(0,-28,0) * CFrame.Angles(math.rad(90),0,0)
				elseif _G.Method == "Upper" then
					Farm_Mode = CFrame.new(0,28,0) * CFrame.Angles(math.rad(-90),0,0)
				elseif _G.Method == "X-Y-Z" then
					Farm_Mode = CFrame.new(getgenv().X ,getgenv().Y,getgenv().Z)
				end
			end)
		end
	end)
	
		WeaponList = {
			"Melee",
			"Sword",
			"Gun",
			"Fruit"
		}
		
			local SelectWeapona = Main:Dropdown("Select Weapon",WeaponList,function(value)
				_G.SelectWeapon = value
			end)
		
		spawn(function()
			while wait(.1) do
				pcall(function()
					if _G.SelectWeapon == "Melee" then
						for i ,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
							if v.ToolTip == "Melee" then
								if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
									_G.SelectWeapon = v.Name
								end
							end
						end
					elseif _G.SelectWeapon == "Sword" then
						for i ,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
							if v.ToolTip == "Sword" then
								if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
									_G.SelectWeapon = v.Name
								end
							end
						end
					elseif _G.SelectWeapon == "Gun" then
						for i ,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
							if v.ToolTip == "Gun" then
								if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
									_G.SelectWeapon = v.Name
								end
							end
						end
					elseif _G.SelectWeapon == "Fruit" then
						for i ,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
							if v.ToolTip == "Blox Fruit" then
								if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
									_G.SelectWeapon = v.Name
								end
							end
						end				
					end
				end)
			end
		end)
		
		spawn(function()
			while wait() do
				if _G.Auto_Farm_Level then
					if _G.Select_Mode_Farm == "Normal Mode" then
						pcall(function()
							if not string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
								StartMagnet = false
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
							end
							if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
								StartMagnet = false
								CheckLevel()
								repeat wait() TP(CFrameQuest) until (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.Auto_Farm_Level
								if (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 then
									wait(1)
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest",NameQuest,LevelQuest)
								end
							elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
								CheckLevel()
								if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
											if v.Name == Ms then
												repeat wait()
													if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
														EquipWeapon(_G.SelectWeapon)
														AutoHaki()
														PosMon = v.HumanoidRootPart.CFrame
														v.HumanoidRootPart.CanCollide = false
														v.Humanoid.WalkSpeed = 0
														v.Humanoid.JumpPower = 0
														v.Head.CanCollide = false
														v.Humanoid:ChangeState(16)
														v.HumanoidRootPart.Size = Vector3.new(50,50,50)
														StartMagnet = true
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														game:GetService'VirtualUser':CaptureController()
														game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
													else
														StartMagnet = false
														game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
													end
												until not _G.Auto_Farm_Level or v.Humanoid.Health <= 0 or not v.Parent or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
											end
										end
									end
								else
									StartMagnet = false
									if game:GetService("ReplicatedStorage"):FindFirstChild(Ms) then
										TP(game:GetService("ReplicatedStorage"):FindFirstChild(Ms).HumanoidRootPart.CFrame * CFrame.new(0,20,0))
									else
										TP(CFrameMon)
									end
								end
							end
						end)
					elseif _G.Select_Mode_Farm == "Fast Mode" then
						pcall(function()
							if game:GetService("Players").LocalPlayer.Data.SpawnPoint.Value == SPAWNPOINT then
								if not string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
									StartMagnet = false
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
								end
								if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
									CheckLevel()
									wait(1)
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest",NameQuest,LevelQuest)
								elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
									CheckLevel()
									if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
										for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
											if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
												if v.Name == Ms then
													repeat wait()
														if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
															EquipWeapon(_G.SelectWeapon)
															AutoHaki()
															PosMon = v.HumanoidRootPart.CFrame
															v.HumanoidRootPart.CanCollide = false
															v.Head.CanCollide = false
															v.HumanoidRootPart.Size = Vector3.new(50,50,50)
															StartMagnet = true
															TP(v.HumanoidRootPart.CFrame * Farm_Mode)
															v.Humanoid:ChangeState(16)
															game:GetService'VirtualUser':CaptureController()
															game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
														else
															StartMagnet = false
															game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
														end
													until not _G.Auto_Farm_Level or v.Humanoid.Health <= 0 or not v.Parent or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
												end
											end
										end
									else
										StartMagnet = false
										if game:GetService("ReplicatedStorage"):FindFirstChild(Ms) then
											TP(game:GetService("ReplicatedStorage"):FindFirstChild(Ms).HumanoidRootPart.CFrame * CFrame.new(0,20,0))
										else
											TP(CFrameMon)
										end
									end
								end
							else
								repeat task.wait()
									game.Players.LocalPlayer.Character.Head:Destroy()
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameQuest
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
								until game:GetService("Players").LocalPlayer.Data.SpawnPoint.Value == SPAWNPOINT
							end
						end)
					elseif _G.Select_Mode_Farm == "No Quest" then
						pcall(function()
							CheckLevel()
							if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
								for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
									if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
										if v.Name == Ms then
											if v.Humanoid.Health > 0 then
												repeat wait()
													EquipWeapon(_G.SelectWeapon)
													AutoHaki()
													PosMon = v.HumanoidRootPart.CFrame
													v.HumanoidRootPart.CanCollide = false
													v.Head.CanCollide = false
													v.Humanoid:ChangeState(16)
													v.HumanoidRootPart.Size = Vector3.new(50,50,50)
													game:GetService'VirtualUser':CaptureController()
													game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
													StartMagnet = true
													TP(v.HumanoidRootPart.CFrame * Farm_Mode)
												until not _G.Auto_Farm_Level or v.Humanoid.Health <= 0 or not v.Parent
											end
										end
									end
								end
							else
								StartMagnet = false
								if game:GetService("ReplicatedStorage"):FindFirstChild(Ms) then
									TP(game:GetService("ReplicatedStorage"):FindFirstChild(Ms).HumanoidRootPart.CFrame * CFrame.new(0,20,0))
								else
									TP(CFrameMon)
								end
							end
						end)
					elseif _G.Select_Mode_Farm == "Easy Mode" then
						pcall(function()
							local QuestTitle = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
							if not string.find(QuestTitle, NameMon) then
								StartMagnet = false
								wait(1)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
							end
							if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
								CheckLevel()
								repeat wait() TP(CFrameQuest) until (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.Auto_Farm_Level
								if (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 then
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest",NameQuest,LevelQuest)
								end
							elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
								CheckLevel()
								if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
											if v.Name == Ms then
												if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
													repeat wait()
														EquipWeapon(_G.SelectWeapon)
														AutoHaki()
														PosMon = v.HumanoidRootPart.CFrame
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														v.HumanoidRootPart.CanCollide = false
														v.Head.CanCollide = false
														v.HumanoidRootPart.Size = Vector3.new(50,50,50)
														v.Humanoid:ChangeState(16)
														StartMagnet = true
														game:GetService'VirtualUser':CaptureController()
														game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
													until not _G.Auto_Farm_Level or v.Humanoid.Health <= 0 or not v.Parent or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
												else
													StartMagnet = false
													wait(1)
													game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
												end
											end
										end
									end
								else
									StartMagnet = false
									TP(CFrameMon)
									if game:GetService("ReplicatedStorage"):FindFirstChild(Ms) then
										TP(game:GetService("ReplicatedStorage"):FindFirstChild(Ms).HumanoidRootPart.CFrame * CFrame.new(15,10,2))
									else
										if (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1 then
											if PosMon ~= nil then
												TP(PosMon * CFrame.new(15,10,2))
											else
												if OldPos ~= nil then
													TP(OldPos.Position)
												end
											end
										end
									end
								end
							end
						end)
					elseif _G.Select_Mode_Farm == "Mob Aura" then
						do
							task = task or getrenv().task;
							fastSpawn,fastWait,delay = task.spawn,task.wait,task.delay
						end
						pcall(function()
							for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
								if _G.Auto_Farm_Level and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= _G.DistanceMobAura then
									repeat wait()
										EquipWeapon(_G.SelectWeapon)
										PosMonAura = v.HumanoidRootPart.CFrame
										v.Humanoid:ChangeState(16)
										TP(v.HumanoidRootPart.CFrame * Farm_Mode)
										game:GetService("VirtualUser"):CaptureController()
										game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670),workspace.CurrentCamera.CFrame)
										StartMagnetKill = true
										_G.AutoMobAura = true
										if delay then
											delay(1,function()
												StartMagnetKill = true
											end)
										end
									until not _G.Auto_Farm_Level or not v.Parent or v.Humanoid.Health <= 0
									_G.AutoMobAura = false
								end
							end
						end)
					elseif _G.Select_Mode_Farm == "Hard Mode" then
						pcall(function()
							CheckLevel()
							magnitude = (workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
							if magnitude < 3000 then
								if not game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
									if _G.Auto_Farm_Level == true then
										if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
											if not game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
												if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
													for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
														if v.Name == Ms then
															monmag = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
															if v.Humanoid.Health > 0 then
																repeat game:GetService("RunService").Heartbeat:wait()
																	EquipWeapon(_G.SelectWeapon)
																	v.Humanoid:ChangeState(16)
																	PosMon = v.HumanoidRootPart.CFrame
																	game:GetService("VirtualUser"):CaptureController()
																	game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 870),workspace.CurrentCamera.CFrame)
																	MinHealth = v.Humanoid.MaxHealth * 90 / 100
																	monmag = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
																	if monmag <= 250 then
																		if v.Humanoid.Health > MinHealth then
																			PosMon = v.HumanoidRootPart.CFrame
																			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,29)
																			StartMagnet = true
																		else
																			PosMon = v.HumanoidRootPart.CFrame
																			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,30,0)
																			StartMagnet = true
																		end
																	else
																		if v.Humanoid.Health > MinHealth then
																			local Distance = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
																			local Speed = 300 --
																			tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
																			tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,14)})
																			tween:Play()
																		else
																			local Distance = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
																			local Speed = 300 --
																			tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
																			tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)})
																			tween:Play()
																		end
																	end
																	v.HumanoidRootPart.Size = Vector3.new(60,60,60)
																	v.HumanoidRootPart.CanCollide = false
																	game.Players.LocalPlayer.Character.HumanoidRootPart.CanCollide = false
																until v.Humanoid.Health <= 0 or _G.Auto_Farm_Level == false
															elseif v.Humanoid.Health <= 0 then
																CheckLevel()
																zmagnitudX = (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
																if zmagnitudX < 500 then
																	CheckLevel()
																	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
																else
																	local Distance = (game.Workspace[Ms].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
																	local Speed = 300 --
																	tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
																	tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameMon})
																	tween:Play()
																end
															end
														end
													end
												else
													wait(1)
													CheckLevel()
													local args = {
														[1] = "AbandonQuest"
													}
													game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
												end
											end
										else
											CheckLevel()
											zmagnitudXz = (game.Workspace[Ms].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
											if zmagnitudXz < 1000 then
												CheckLevel()
												local Distance = (game.Workspace[Ms].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
												local Speed = 500 --
												tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
												tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameMon})
												tween:Play()
												StartMagnet = false
											else
												local Distance = (game.Workspace[Ms].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
												local Speed = 300 --
												tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
												tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameMon})
												tween:Play()
												StartMagnet = true
												PosMon = v.HumanoidRootPart.CFrame
											end
										end
									end
								else
									CheckLevel()
									armmag = (game.Workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
									if armmag <= 1000 then
										local Distance = (game.Workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
										local Speed = 500 --
										tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
										tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameQuest})
										tween:Play()
									else
										local Distance = (game.Workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
										local Speed = 500 --
										tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
										tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameQuest})
										tween:Play()
									end
									print(magnitude)
									farmmag = (game.Workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
									if farmmag <= 120 then
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace[NameMon].CFrame
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack({[1] = "SetSpawnPoint"}))
										task.wait()
										local args = {
											[1] = "StartQuest",
											[2] = NameQuest,
											[3] = LevelQuest
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
								end
							else
								CheckLevel()
								local Distancex = (game.Workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
								local Speexd = 200 --
								tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
								tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameQuest})
								tweenx:Play()
								print(magnitude)
								_G.NoClip = true
								wait(Distancex/Speexd)
								print(Distancex/Speexd)
								_G.NoClip = false
							end
						end)
					end
				end
			end
		end)		

		Main:Seperator("Main Farm")
		
			Main:Toggle("Auto Farm Level",_G.Auto_Farm_Level,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else				
					_G.Auto_Farm_Level = value  
					_G.AutoBacklegv = value
					StopTween(_G.Auto_Farm_Level)
		    	end
		    end)
	
			if World1 then
			Main:Toggle("Auto Second Sea",_G.AutoWorld2,function(value)
					_G.AutoWorld2 = value
					StopTween(_G.AutoWorld2)
				end)
		
			spawn(function() -- Auto Wolrd2
				while wait() do
					if _G.AutoWorld2 then
						local Level = game.Players.LocalPlayer.Data.Level.Value
						if Level >= 700 and World1 then
						  _G.Auto_Farm_Level = false
							if game.Workspace.Map.Ice.Door.CanCollide == true and game.Workspace.Map.Ice.Door.Transparency == 0 then
								TP(CFrame.new(4851.8720703125, 5.6514348983765, 718.47094726563))
								wait(.5)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("DressrosaQuestProgress","Detective")
								EquipWeapon("Key")
								TP(CFrame.new(1347.7124, 37.3751602, -1325.6488))
								wait(3)
							elseif game.Workspace.Map.Ice.Door.CanCollide == false and game.Workspace.Map.Ice.Door.Transparency == 1 then
								if game:GetService("Workspace").Enemies:FindFirstChild("Ice Admiral [Lv. 700] [Boss]") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v.Name == "Ice Admiral [Lv. 700] [Boss]" and v.Humanoid.Health > 0 then
											repeat game:GetService("RunService").Heartbeat:wait()
												pcall(function()
													EquipWeapon(_G.SelectWeapon)
													TP(v.HumanoidRootPart.CFrame * Farm_Mode)
													v.HumanoidRootPart.CanCollide = false
													v.HumanoidRootPart.Size = Vector3.new(60,60,60)
													game:GetService("VirtualUser"):CaptureController()
													game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
												end)
											until v.Humanoid.Health <= 0 or not v.Parent
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
										end
									end
								else
									TP(CFrame.new(1347.7124, 37.3751602, -1325.6488))
								end
							else
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
							end
						end
					end
				end
			end)
		end
		
			if World2 then
				Main:Toggle("Auto Third Sea",_G.AutoThirdSea,function(value)
					_G.AutoThirdSea = value
					StopTween(_G.AutoThirdSea)
				end)
			
				spawn(function()
					while wait() do
						if _G.AutoThirdSea then
							pcall(function()
								if game:GetService("Players").LocalPlayer.Data.Level.Value >= 1500 and World2 then
									_G.Auto_Farm_Level = false
									if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ZQuestProgress","Check") == 0 then
										TP(CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016))
										if (CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 10 then
											wait(1.5)
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ZQuestProgress","Begin")
										end
										wait(1.8)
										if game:GetService("Workspace").Enemies:FindFirstChild("rip_indra [Lv. 1500] [Boss]") then
											for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
												if v.Name == "rip_indra [Lv. 1500] [Boss]" then
													OldCFrameThird = v.HumanoidRootPart.CFrame
													repeat task.wait()
														AutoHaki()
														EquipWeapon(_G.SelectWeapon)
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														v.HumanoidRootPart.CFrame = OldCFrameThird
														v.HumanoidRootPart.Size = Vector3.new(50,50,50)
														v.HumanoidRootPart.CanCollide = false
														v.Humanoid.WalkSpeed = 0
														game:GetService'VirtualUser':CaptureController()
														game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
														game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
														sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
													until _G.AutoThirdSea == false or v.Humanoid.Health <= 0 or not v.Parent
												end
											end
										elseif not game:GetService("Workspace").Enemies:FindFirstChild("rip_indra [Lv. 1500] [Boss]") and (CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1000 then
											TP(CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016))
										end
									end
								end
							end)
						end
					end
				end)
			end
			
			if World2 then
				Main:Toggle("Auto Farm Factory",_G.AutoFactory,function(value)
					_G.AutoFactory = value
					StopTween(_G.AutoFactory)
				end)
			
				spawn(function()
					while wait() do
						pcall(function()
							if _G.AutoFactory then
								if game:GetService("Workspace").Enemies:FindFirstChild("Core") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v.Name == "Core" and v.Humanoid.Health > 0 then
											repeat task.wait()
												_G.Auto_Farm_Level = false
												AutoHaki()         
												EquipWeapon(_G.SelectWeapon)           
												TP(CFrame.new(448.46756, 199.356781, -441.389252))                                  
												game:GetService("VirtualUser"):CaptureController()
												game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670),workspace.CurrentCamera.CFrame)
											until v.Humanoid.Health <= 0 or _G.AutoFactory == false
										end
									end
								end
							end
						end)
					end
				end)
		    end

			if World3 then
				Main:Toggle("Auto Farm Pirate Raids",_G.AutoPirateRaids,function(value)
					_G.AutoPirateRaids = value
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-5093.14258, 315.68924, -3134.78271, -0.368919224, 0, 0.929461479, 0, 1, 0, -0.929461479, 0, -0.368919224)
					StopTween(_G.AutoPirateRaids)
				end)
			
				spawn(function()
					while wait() do
						pcall(function()
							if _G.AutoPirateRaids then              
								if game:GetService("Workspace").Enemies:GetChildren() then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if _G.AutoPirateRaids and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 1000 then
											repeat wait()
												StartMagnet = true
												EquipWeapon(_G.SelectWeapon)
												PosMon = v.HumanoidRootPart.CFrame
												v.HumanoidRootPart.Size = Vector3.new(60,60,60)
												v.Humanoid.JumpPower = 0
												v.Humanoid.WalkSpeed = 0
												v.HumanoidRootPart.CanCollide = false
												v.Humanoid:ChangeState(11)
												TP(v.HumanoidRootPart.CFrame * CFrame.new(0,20,0))
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
											until v.Humanoid.Health <= 0 or _G.AutoPirateRaids == false
											StartMagnet = false
										end
									end
								end
							end
						end)
					end
				end)
		    end

			 Main:Seperator("Fighting Style")
			
			Main:Toggle("Auto Super Human",Auto_Fully_Superhuman,function(value)
				Auto_Fully_Superhuman = value
				StopTween(Auto_Fully_Superhuman)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySuperhuman")	
			end)
			
			spawn(function()
				while wait() do
					if Auto_Fully_Superhuman and game.Players.LocalPlayer:FindFirstChild("WeaponAssetCache") then 
						pcall(function()
							if game:GetService("Players").LocalPlayer.Data.Beli.Value >= 500000 and (game.Players.LocalPlayer.Character:FindFirstChild("Combat") or game.Players.LocalPlayer.Backpack:FindFirstChild("Combat")) then
								_G.SelectWeapon = "Combat"
								local args = {
									[1] = "BuyElectro"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end   
							if game.Players.LocalPlayer.Character:FindFirstChild("Superhuman") or game.Players.LocalPlayer.Backpack:FindFirstChild("Superhuman") then
								_G.SelectWeapon = "Superhuman"
							end  
							if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value <= 299 then
								_G.SelectWeapon = "Black Leg"
							end
							if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value <= 299 then
								_G.SelectWeapon = "Electro"
							end
							if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value <= 299 then
								_G.SelectWeapon = "Fishman Karate"
							end
							if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value <= 299 then
								_G.SelectWeapon = "Dragon Claw"
							end
							if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 300 then
								local args = {
									[1] = "BuyFishmanKarate"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
							if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 300 then
								local args = {
									[1] = "BuyFishmanKarate"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
							if game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 300 then
								local args = {
									[1] = "BuyBlackLeg"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
							if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 300 then
								if Auto_Fully_Superhuman and game.Players.LocalPlayer.Data.Fragments.Value < 1500 then
									if game.Players.LocalPlayer.Data.Level.Value > 1100 then
										_G.SelectChip = "Flame"
										_G.AutoBuyChip = true
										_G.Auto_StartRaid = true
										_G.Next_Islands = true
										_G.KillAura = true
									end
								else
									_G.AutoBuyChip = false
									_G.Auto_StartRaid = false
									_G.Next_Islands = false
									_G.KillAura = false
									local args = {
										[1] = "BlackbeardReward",
										[2] = "DragonClaw",
										[3] = "2"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end
							end
							if game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate").Level.Value >= 300 then
								if Auto_Fully_Superhuman and game.Players.LocalPlayer.Data.Fragments.Value < 1500 then
									if game.Players.LocalPlayer.Data.Level.Value > 1100 then
										_G.SelectChip = "Flame"
										_G.AutoBuyChip = true
										_G.Auto_StartRaid = true
										_G.Next_Islands = true
										_G.KillAura = true
									end
								else
									_G.AutoBuyChip = false
									_G.Auto_StartRaid = false
									_G.Next_Islands = false
									_G.KillAura = false
									local args = {
										[1] = "BlackbeardReward",
										[2] = "DragonClaw",
										[3] = "2"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end
							end
							if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value >= 300 then
								local args = {
									[1] = "BuySuperhuman"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							end
						end)
					end
				end
			end)
			
			if World2 then
			Main:Toggle("Auto Death Step",Auto_Fully_Death_Step,function(value)
				Auto_Fully_Death_Step = value
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDeathStep")
				StopTween(Auto_Fully_Death_Step)
			end)
			
			spawn(function()
				while wait() do
					if Auto_Fully_Death_Step then
						pcall(function()
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Library Key") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Library Key") then
								EquipWeapon("Library Key")
								repeat wait() TP(CFrame.new(6371.2001953125, 296.63433837890625, -6841.18115234375)) until (CFrame.new(6371.2001953125, 296.63433837890625, -6841.18115234375).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.Auto_Fully_Death_Step
									if (CFrame.new(6371.2001953125, 296.63433837890625, -6841.18115234375).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 then
										wait(1.2)
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDeathStep",true)
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDeathStep")
										wait(0.5)
									end
								elseif game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 400 or game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 400 then  
									if game:GetService("ReplicatedStorage"):FindFirstChild("Awakened Ice Admiral [Lv. 1400] [Boss]") or game:GetService("Workspace").Enemies:FindFirstChild("Awakened Ice Admiral [Lv. 1400] [Boss]") then
										if game:GetService("Workspace").Enemies:FindFirstChild("Awakened Ice Admiral [Lv. 1400] [Boss]") then 	
											for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
												if v.Name == "Awakened Ice Admiral [Lv. 1400] [Boss]" then    
													repeat wait()
														AutoHaki()
														EquipWeapon(_G.SelectWeapon)
														v.HumanoidRootPart.Size = Vector3.new(50,50,50)
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														game:GetService'VirtualUser':CaptureController()
														game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
														sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
													until not v.Parent or v.Humanoid.Health <= 0 or Auto_Fully_Death_Step == false or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Library Key") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Library Key")
												end
											end
										else
											repeat wait() TP(game:GetService("ReplicatedStorage"):FindFirstChild("Awakened Ice Admiral [Lv. 1400] [Boss]").HumanoidRootPart.CFrame) until game:GetService("Workspace").Enemies:FindFirstChild("Awakened Ice Admiral [Lv. 1400] [Boss]")
										end
									end
								 end
							end)
						end
					 end
				end)
	
				Main:Toggle("Auto Sharkman Karate",Auto_Fully_SharkMan_Karate,function(value)
					Auto_Fully_SharkMan_Karate = value
					StopTween(Auto_Fully_SharkMan_Karate)
				end)
				
			  spawn(function()
					while wait() do
						if Auto_Fully_SharkMan_Karate then
							pcall(function()	
								if string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate"), "keys") then  
									if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Water Key") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Water Key") then
										repeat wait() TP(-2604.6958, 239.432526, -10315.1982, 0.0425701365, 0, -0.999093413, 0, 1, 0, 0.999093413, 0, 0.0425701365) until (CFrame.new(-2604.6958, 239.432526, -10315.1982, 0.0425701365, 0, -0.999093413, 0, 1, 0, 0.999093413, 0, 0.0425701365).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not Auto_Fully_SharkMan_Karate
										if (CFrame.new(-2604.6958, 239.432526, -10315.1982, 0.0425701365, 0, -0.999093413, 0, 1, 0, 0.999093413, 0, 0.0425701365).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 then
									end
									elseif game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 400 or game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 400 then   
										if game:GetService("ReplicatedStorage"):FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") or game:GetService("Workspace").Enemies:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") then
											if game:GetService("Workspace").Enemies:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") then 	
												for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
													if v.Name == "Tide Keeper [Lv. 1475] [Boss]" then    
														repeat wait()
															AutoHaki()
															EquipWeapon(_G.SelectWeapon)
															v.Head.CanCollide = false
															v.Humanoid.WalkSpeed = 0
															v.HumanoidRootPart.CanCollide = false
															v.HumanoidRootPart.Size = Vector3.new(50,50,50)
															TP(v.HumanoidRootPart.CFrame * Farm_Mode)
															game:GetService'VirtualUser':CaptureController()
															game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
															sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
														until not v.Parent or v.Humanoid.Health <= 0 or Auto_Fully_SharkMan_Karate == false or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Water Key") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Water Key")
													end
												end
											else
												game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyFishmanKarate")
												repeat wait() TP(game:GetService("ReplicatedStorage"):FindFirstChild("Tide Keeper [Lv. 1475] [Boss]").HumanoidRootPart.CFrame) until game:GetService("Workspace").Enemies:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]")
											end
										end
									end
								end
							end)
						end
					end
				end)
			end
	
	if World3 then
		Main:Toggle("Auto Electric Claw",_G.AutoElectricClaw, function(value)
				_G.AutoElectricClaw = value
				StopTween(_G.AutoElectricClaw)
			end)
	
			spawn(function()
				pcall(function()
					while wait() do 
						if _G.AutoElectricClaw then
							if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Electro") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Electro") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Electric Claw") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Electric Claw") then
								if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Electro") and game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 400 then
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
									_G.SelectWeapon = "Electric Claw"
								end  
								if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Electro") and game:GetService("Players").LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 400 then
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
									_G.SelectWeapon = "Electric Claw"
								end  
								if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Electro") and game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value <= 399 then
									_G.SelectWeapon = "Electro"
								end 
							else
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro")
							end
						end
						if _G.AutoElectricClaw then
							if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Electro") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Electro") then
								if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Electro") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Electro") and game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 400 or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 400 then
									if _G.Auto_Farm_Level == false then
										repeat task.wait()
											TP(CFrame.new(-10371.4717, 330.764496, -10131.4199))
										until not _G.AutoElectricClaw or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - CFrame.new(-10371.4717, 330.764496, -10131.4199).Position).Magnitude <= 10
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw","Start")
										wait(2)
										repeat task.wait()
											TP(CFrame.new(-12550.532226563, 336.22631835938, -7510.4233398438))
										until not _G.AutoElectricClaw or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - CFrame.new(-12550.532226563, 336.22631835938, -7510.4233398438).Position).Magnitude <= 10
										wait(1)
										repeat task.wait()
											TP(CFrame.new(-10371.4717, 330.764496, -10131.4199))
										until not _G.AutoElectricClaw or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - CFrame.new(-10371.4717, 330.764496, -10131.4199).Position).Magnitude <= 10
										wait(1)
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
									elseif _G.Auto_Farm_Level == true then
										_G.Auto_Farm_Level = false
										wait(1)
										repeat task.wait()
											TP(CFrame.new(-10371.4717, 330.764496, -10131.4199))
										until not _G.AutoElectricClaw or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - CFrame.new(-10371.4717, 330.764496, -10131.4199).Position).Magnitude <= 10
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw","Start")
										wait(2)
										repeat task.wait()
											TP(CFrame.new(-12550.532226563, 336.22631835938, -7510.4233398438))
										until not _G.AutoElectricClaw or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - CFrame.new(-12550.532226563, 336.22631835938, -7510.4233398438).Position).Magnitude <= 10
										wait(1)
										repeat task.wait()
											TP(CFrame.new(-10371.4717, 330.764496, -10131.4199))
										until not _G.AutoElectricClaw or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - CFrame.new(-10371.4717, 330.764496, -10131.4199).Position).Magnitude <= 10
										wait(1)
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
										_G.SelectWeapon = "Electric Claw"
										wait(.1)
										_G.Auto_Farm_Level = true
									end
								end
							end
						end
					end
				end)
			end)
	
			 Main:Toggle("Auto Dragon Talon",AutoDragonTalon,function(value)
				AutoDragonTalon = value
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","2")
				StopTween(AutoDragonTalon)
			end)
			
			spawn(function()
				while wait() do
					if AutoDragonTalon then
						if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Claw") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon Claw") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Talon") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon Talon") then
							if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value >= 400 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon")
								_G.SelectWeapon = "Dragon Talon"
						    elseif game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value <= 399 then
								_G.SelectWeapon = "Dragon Claw"
								_G.Auto_Farm_Level = true
							end
						end
					end
				end
			end)
		end

        local SupComplete = false
		local EClawComplete = false
		local TalComplete = false
		local SharkComplete = false
		local DeathComplete = false
		local GodComplete = false
		
		function GetAllMeleeFarm()
			if SupComplete == false then
				local args = {
					[1] = "BuySuperhuman"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				if CheckMasteryWeapon("Superhuman",400) == "true UpTo" then
					SupComplete = true
				end
			end
			wait(.5)
			if EClawComplete == false then
				local string_1 = "BuyElectricClaw";
				local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
				Target:InvokeServer(string_1);
		
				if CheckMasteryWeapon("Electric Claw",400) == "true UpTo" then
					EClawComplete = true
				end
			end
			wait(.5)
			if TalComplete == false then
				game.ReplicatedStorage.Remotes.CommF_:InvokeServer("BuyDragonTalon")
		
				if CheckMasteryWeapon("Dragon Talon",400) == "true UpTo" then
					TalComplete = true
				end
			end
			wait(.5)
			if SharkComplete == false then
				local args = {
					[1] = "BuySharkmanKarate"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		
				if CheckMasteryWeapon("Sharkman Karate",400) == "true UpTo" then
					SharkComplete = true
				end
			end
			wait(.5)
			if DeathComplete == false then
				local args = {
					[1] = "BuyDeathStep"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		
				if CheckMasteryWeapon("Death Step",400) == "true UpTo" then
					DeathComplete = true
				end
			end
			if GodComplete == false then
				local args = {
					[1] = "BuyGodhuman"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		
				if CheckMasteryWeapon("Godhuman",350) == "true UpTo" then
					GodComplete = true
				end
			end
		end	
	
			Main:Toggle("Auto God Human",_G.AutoFullyGodhuman,function(value)
				_G.AutoFullyGodhuman = value
				StopTween(_G.AutoFullyGodhuman)
			end)
	
			BuyGodhuman = tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyGodhuman",true))
			if BuyGodhuman then
				if BuyGodhuman ~= 1 then
					GetAllMeleeFarm()
				end
			end
	
			spawn(function()
				while wait() do
					pcall(function()
						if _G.AutoFullyGodhuman then
							BuyGodhuman = tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyGodhuman",true))
							if BuyGodhuman then
								if BuyGodhuman == 1 then
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyGodhuman")
									_G.AutoFullyGodhuman = false
								end
							end
							if not HasTalon then
								BuyDragonTalon = tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon",true))
	
								if BuyDragonTalon then
									if BuyDragonTalon == 1 then
										HasTalon = true
									end
								end
							end
							if not HasSuperhuman then
								BuySuperhuman = tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySuperhuman",true))
	
								if BuySuperhuman then
									if BuySuperhuman == 1 then
										HasSuperhuman = true
									end
								end
							end
							if not HasKarate then
								BuySharkmanKarate = tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true))
	
								if BuySharkmanKarate then
									if BuySharkmanKarate == 1 then
										HasKarate = true
									end
								end
							end
							if not HasDeathStep then
								BuyDeathStep = tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer( "BuyDeathStep",true))
	
								if BuyDeathStep then
									if BuyDeathStep == 1 then
										HasDeathStep = true
									end
								end
							end
							if not HasElectricClaw then
								BuyElectricClaw = tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw",true))
								if BuyElectricClaw then
									if BuyElectricClaw == 1 then
										HasElectricClaw = true
									end
								end
							end
	
							if not HasSuperhuman then
								if game.Players.LocalPlayer:FindFirstChild("WeaponAssetCache") then
									if not game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") and not game.Players.LocalPlayer.Character:FindFirstChild("Combat") then
										if not game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and not game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") then
											if not game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and not game.Players.LocalPlayer.Character:FindFirstChild("Electro") then
												if not game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and not game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") then
													if not game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and not game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") then
														if not game.Players.LocalPlayer.Backpack:FindFirstChild("Superhuman") and not game.Players.LocalPlayer.Character:FindFirstChild("Superhuman") then
															local args = {
																[1] = "BuyElectro"
															}
															game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
														end
													end
												end
											end
										end
									end
									_G.SelectWeapon = GetFightingStyle("Melee")
	
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game.Players.LocalPlayer.Character:FindFirstChild("Combat") then
										local args = {
											[1] = "BuyElectro"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 300 then
										local args = {
											[1] = "BuyBlackLeg"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									if game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 300 then
										local args = {
											[1] = "BuyBlackLeg"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 300 then
										local args = {
											[1] = "BuyFishmanKarate"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 300 then
										local args = {
											[1] = "BuyFishmanKarate"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 300  then
										local args = {
											[1] = "BlackbeardReward",
											[2] = "DragonClaw",
											[3] = "2"
										}
										HaveDragonClaw = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
										if _G.AutoFullyGodhuman and game.Players.LocalPlayer.Data.Fragments.Value <= 1500 and HaveDragonClaw == 0 then
											if game.Players.LocalPlayer.Data.Level.Value > 1100 then
												if _G.Auto_Farm_Level == false then
												end
											end
										else
											if _G.Auto_Farm_Level == true then
										end
											local args = {
												[1] = "BlackbeardReward",
												[2] = "DragonClaw",
												[3] = "2"
											}
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
										end
									end
									if game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate").Level.Value >= 300  then
										local args = {
											[1] = "BlackbeardReward",
											[2] = "DragonClaw",
											[3] = "2"
										}
										HaveDragonClaw = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
										if _G.AutoFullyGodhuman and game.Players.LocalPlayer.Data.Fragments.Value <= 1500 and HaveDragonClaw == 0 then
											if game.Players.LocalPlayer.Data.Level.Value > 1100 then
												if _G.Auto_Farm_Level == false then
												end
											end
										else
											if _G.Auto_Farm_Level == true then 
										end
											local args = {
												[1] = "BlackbeardReward",
												[2] = "DragonClaw",
												[3] = "2"
											}
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
											if _G.Auto_Farm_Level == true then
										end
									end
								end
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value >= 300 then
										if _G.Auto_Farm_Level == true then
									end
										local args = {
											[1] = "BuySuperhuman"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end
									if game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw").Level.Value >= 300 then
										if _G.Auto_Farm_Level == true then
									end
										local args = {
											[1] = "BuySuperhuman"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									end 
								end
							elseif not HasKarate then
								if game.Players.LocalPlayer:FindFirstChild("WeaponAssetCache") then
									if not game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and not game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") then
										if not game.Players.LocalPlayer.Backpack:FindFirstChild("Sharkman Karate") and not game.Players.LocalPlayer.Character:FindFirstChild("Sharkman Karate") then
											local args = {
												[1] = "BuyFishmanKarate"
											}
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
										end
									end
	
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 400 then
										if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true) == "I lost my house keys, could you help me find them? Thanks." and not game.Players.LocalPlayer.Character:FindFirstChild("Water Key") and not game.Players.LocalPlayer.Backpack:FindFirstChild("Water Key") then
											if World2 then
												KillSharkMan = true
												if _G.Auto_Farm_Level == false then
											end
											else
												KillSharkMan = false
												if _G.Auto_Farm_Level == true then
											 end
											end
										elseif tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true)) == 1 then
											KillSharkMan = false
											if _G.Auto_Farm_Level == true then
										 end
											local args = {
												[1] = "BuySharkmanKarate"
											}
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
										elseif game.Players.LocalPlayer.Character:FindFirstChild("Water Key") or game.Players.LocalPlayer.Backpack:FindFirstChild("Water Key") then
											KillSharkMan = false
											if _G.Auto_Farm_Level == true then
										 end
											local args = {
												[1] = "BuySharkmanKarate"
											}
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
										end
									end
	
									if game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate").Level.Value >= 400 then
										if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true) == "I lost my house keys, could you help me find them? Thanks." and not game.Players.LocalPlayer.Character:FindFirstChild("Water Key") and not game.Players.LocalPlayer.Backpack:FindFirstChild("Water Key") then
											if World2 then
												KillSharkMan = true
												if _G.Auto_Farm_Level == false then
											end
											else
												if _G.Auto_Farm_Level == true then
											 end
												KillSharkMan = false
											end
										elseif tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true)) == 1 then
											KillSharkMan = false
											if _G.Auto_Farm_Level == true then
										end
											local args = {
												[1] = "BuySharkmanKarate"
											}
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
										elseif game.Players.LocalPlayer.Character:FindFirstChild("Water Key") or game.Players.LocalPlayer.Backpack:FindFirstChild("Water Key") then
											KillSharkMan = false
											if _G.Auto_Farm_Level == true then
										end
											local args = {
												[1] = "BuySharkmanKarate"
											}
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
										end
									end
									_G.SelectWeapon = GetFightingStyle("Melee")
								end
							elseif not HasDeathStep then
								if game.Players.LocalPlayer:FindFirstChild("WeaponAssetCache") then
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 400 then
										local args = {
											[1] = "BuyDeathStep"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	
									end  
									if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 400 then
										local args = {
											[1] = "BuyDeathStep"
										}
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	
									end  
									_G.SelectWeapon = GetFightingStyle("Melee")
								end
							elseif not HasTalon then
								if game.Players.LocalPlayer:FindFirstChild("WeaponAssetCache") then
									_G.SelectWeapon = GetFightingStyle("Melee")
	
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value >= 400 and game.Players.LocalPlayer.Character:WaitForChild("Humanoid").Health > 0 then
										if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon", true) == 3 then
											local string_1 = "Bones";
											local string_2 = "Buy";
											local number_1 = 1;
											local number_2 = 1;
											local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
											Target:InvokeServer(string_1, string_2, number_1, number_2);
	
											local string_1 = "BuyDragonTalon";
											local bool_1 = true;
											local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
											Target:InvokeServer(string_1, bool_1);
										elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon", true) == 1 then
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon")
										else
											local string_1 = "Bones";
											local string_2 = "Buy";
											local number_1 = 1;
											local number_2 = 1;
											local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
											Target:InvokeServer(string_1, string_2, number_1, number_2);
										end 
									end
	
									if game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw").Level.Value >= 400 and game.Players.LocalPlayer.Character:WaitForChild("Humanoid").Health > 0 then
										if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon", true) == 3 then
											local string_1 = "Bones";
											local string_2 = "Buy";
											local number_1 = 1;
											local number_2 = 1;
											local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
											Target:InvokeServer(string_1, string_2, number_1, number_2);
	
											local string_1 = "BuyDragonTalon";
											local bool_1 = true;
											local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
											Target:InvokeServer(string_1, bool_1);
										elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon", true) == 1 then
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon")
										else
											local string_1 = "Bones";
											local string_2 = "Buy";
											local number_1 = 1;
											local number_2 = 1;
											local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
											Target:InvokeServer(string_1, string_2, number_1, number_2);
										end 
									end
								end
							elseif not HasElectricClaw then
								if game.Players.LocalPlayer:FindFirstChild("WeaponAssetCache") then
									_G.SelectWeapon = GetFightingStyle("Melee")
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 400 then
										local v175 = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw", true);
										if v175 == 4 then
											local v176 = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw", "Start");
											if v176 == nil then
												game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12548, 337, -7481)
											end
										else
											local string_1 = "BuyElectricClaw";
											local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
											Target:InvokeServer(string_1);
										end
									end
	
									if game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 400 then
										local v175 = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw", true);
										if v175 == 4 then
											local v176 = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw", "Start");
											if v176 == nil then
												game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12548, 337, -7481)
											end
										else
											local string_1 = "BuyElectricClaw";
											local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
											Target:InvokeServer(string_1);
										end
									end
								end
							end
							if BuyGodhuman ~= 1 and HasSuperhuman and HasTalon and HasKarate and HasDeathStep and HasElectricClaw then
								if HasSuperhuman and not SupComplete then
									local args = {
										[1] = "BuySuperhuman"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									wait(0.2)
									if CheckMasteryWeapon("Superhuman",400) == "true UpTo" or CheckMasteryWeapon("Superhuman",400) == "true" and SupComplete == false then
										SupComplete = true
									end
								elseif HasTalon and not TalComplete then
									local args = {
										[1] = "BuyDragonTalon"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									wait(0.2)
									if CheckMasteryWeapon("Dragon Talon",400) == "true UpTo" or CheckMasteryWeapon("Superhuman",400) == "true" and TalComplete == false then
										TalComplete = true
									end
								elseif HasKarate and not SharkComplete then
									local args = {
										[1] = "BuySharkmanKarate"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									wait(0.2)
									if CheckMasteryWeapon("Sharkman Karate",400) == "true UpTo" or CheckMasteryWeapon("Superhuman",400) == "true" and SharkComplete == false then
										SharkComplete = true
									end
								elseif HasDeathStep and not DeathComplete then
									local args = {
										[1] = "BuyDeathStep"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									wait(0.2)
									if CheckMasteryWeapon("Death Step",400) == "true UpTo" or CheckMasteryWeapon("Superhuman",400) == "true" and DeathComplete == false then
										DeathComplete = true
									end
								elseif HasElectricClaw and not EClawComplete then
									local args = {
										[1] = "BuyElectricClaw"
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
									wait(0.2)
									if CheckMasteryWeapon("Electric Claw",400) == "true UpTo" or CheckMasteryWeapon("Superhuman",400) == "true" and EClawComplete == false then
										EClawComplete = true
									end
								end
							end
	
							if BuyGodhuman ~= 1 and SupComplete and EClawComplete and TalComplete and SharkComplete and DeathComplete and (not game.Players.LocalPlayer.Character:FindFirstChild("Godhuman") or not game.Players.LocalPlayer.Backpack:FindFirstChild("Godhuman")) then
								if GetMaterial("Fish Tail") >= 20 then
									if GetMaterial("Magma Ore") >= 20 then
										if GetMaterial("Dragon Scale") >= 10 then
											if GetMaterial("Mystic Droplet") >= 10 then
												Com("F_","BuyGodhuman")
												BuyGodhuman = tonumber(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyGodhuman",true))
	
												if BuyGodhuman then
													if BuyGodhuman == 1 then
														_G.AutoFullyGodhuman = false
													end
												end
												if _G.AutoFullyGodhuman == true then
											end
											elseif not World2 then
												Com("F_","TravelDressrosa")
											elseif World2 then
												if _G.Auto_Farm_Level == false then
											end
												CheckMaterial("Mystic Droplet")
												if CustomFindFirstChild(MaterialMob) then
													for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
														if _G.AutoFullyGodhuman and table.find(MaterialMob,v.Name) and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
															repeat wait()
																FarmtoTarget = TP2(v.HumanoidRootPart.CFrame * CFrame.new(0,30,1))
																if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 150 then
																	if FarmtoTarget then 
																		FarmtoTarget:Stop()
																	end
																	EquipWeapon(_G.SelectWeapon)
																	spawn(function()
																		for i,v2 in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
																			if v2.Name == v.Name then
																				spawn(function()
																					if InMyNetWork(v2.HumanoidRootPart) then
																						v2.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
																						v2.Humanoid.JumpPower = 0
																						v2.Humanoid.WalkSpeed = 0
																						v2.HumanoidRootPart.CanCollide = false
																						v2.Humanoid:ChangeState(11)
																						v2.HumanoidRootPart.Size = Vector3.new(80,80,80)
																					end
																				end)
																			end
																		end
																	end)
																	TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
																end
															until not CustomFindFirstChild(MaterialMob) or not _G.AutoFullyGodhuman or v.Humanoid.Health <= 0 or not v.Parent
														end
													end
												else
													Modstween = TP2(CFrameMon.Position,CFrameMon)
													if World1 and (table.find(MaterialMob,"Fishman Commando [Lv. 400]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
														if Modstween then Modstween:Stop() end wait(.5)
														game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
													elseif World1 and not (table.find(MaterialMob,"Fishman Commando [Lv. 400]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
														if Modstween then Modstween:Stop() end wait(.5)
														game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(3864.8515625, 6.6796875, -1926.7841796875))
													elseif World1 and (table.find(MaterialMob,"God's Guard [Lv. 450]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 3000 then
														if Modstween then Modstween:Stop() end wait(.5)
														game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-4607.8227539063, 872.54248046875, -1667.5568847656))
													elseif (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 150 then
														if Modstween then Modstween:Stop() end
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
													end 
												end
											end
										elseif not World3 then
											Com("F_","TravelZou")
										elseif World3 then
											if _G.Auto_Farm_Level == false then
										end
											CheckMaterial("Dragon Scale")
											if CustomFindFirstChild(MaterialMob) then
												for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
													if _G.AutoFullyGodhuman and table.find(MaterialMob,v.Name) and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
														repeat wait()
															FarmtoTarget = TP2(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
															if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 150 then
																if FarmtoTarget then FarmtoTarget:Stop() end
																EquipWeapon(_G.SelectWeapon)
																spawn(function()
																	for i,v2 in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
																		if v2.Name == v.Name then
																			spawn(function()
																				if InMyNetWork(v2.HumanoidRootPart) then
																					v2.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
																					v2.Humanoid.JumpPower = 0
																					v2.Humanoid.WalkSpeed = 0
																					v2.HumanoidRootPart.CanCollide = false
																					v2.Humanoid:ChangeState(11)
																					v2.HumanoidRootPart.Size = Vector3.new(80,80,80)
																				end
																			end)
																		end
																	end
																end)
																TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
															end
														until not CustomFindFirstChild(MaterialMob) or not _G.AutoFullyGodhuman or v.Humanoid.Health <= 0 or not v.Parent
													end
												end
											else
												Modstween = TP2(CFrameMon.Position,CFrameMon)
												if World1 and (table.find(MaterialMob,"Fishman Commando [Lv. 400]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
													if Modstween then Modstween:Stop() end wait(.5)
													game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
												elseif World1 and not (table.find(MaterialMob,"Fishman Commando [Lv. 400]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
													if Modstween then Modstween:Stop() end wait(.5)
													game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(3864.8515625, 6.6796875, -1926.7841796875))
												elseif World1 and (table.find(MaterialMob,"God's Guard [Lv. 450]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 3000 then
													if Modstween then Modstween:Stop() end wait(.5)
													game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-4607.8227539063, 872.54248046875, -1667.5568847656))
												elseif (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 150 then
													if Modstween then Modstween:Stop() end
													game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
												end 
											end
										end
									elseif not World1 then
										Com("F_","TravelMain")
									elseif World1 then
										if _G.Auto_Farm_Level == false then
									end
										CheckMaterial("Magma Ore")
										if CustomFindFirstChild(MaterialMob) then
											for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
												if _G.AutoFullyGodhuman and table.find(MaterialMob,v.Name) and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
													repeat wait()
														FarmtoTarget = TP2(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
														if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 150 then
															if FarmtoTarget then FarmtoTarget:Stop() end
															EquipWeapon(_G.SelectWeapon)
															spawn(function()
																for i,v2 in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
																	if v2.Name == v.Name then
																		spawn(function()
																			if InMyNetWork(v2.HumanoidRootPart) then
																				v2.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
																				v2.Humanoid.JumpPower = 0
																				v2.Humanoid.WalkSpeed = 0
																				v2.HumanoidRootPart.CanCollide = false
																				v2.Humanoid:ChangeState(11)
																				v2.HumanoidRootPart.Size = Vector3.new(80,80,80)
																			end
																		end)
																	end
																end
															end)
															TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
														end
													until not CustomFindFirstChild(MaterialMob) or not _G.AutoFullyGodhuman or v.Humanoid.Health <= 0 or not v.Parent
												end
											end
										else
											Modstween = TP2(CFrameMon.Position,CFrameMon)
											if World1 and (table.find(MaterialMob,"Fishman Commando [Lv. 400]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
												if Modstween then Modstween:Stop() end wait(.5)
												game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
											elseif World1 and not (table.find(MaterialMob,"Fishman Commando [Lv. 400]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
												if Modstween then Modstween:Stop() end wait(.5)
												game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(3864.8515625, 6.6796875, -1926.7841796875))
											elseif World1 and (table.find(MaterialMob,"God's Guard [Lv. 450]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 3000 then
												if Modstween then Modstween:Stop() end wait(.5)
												game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-4607.8227539063, 872.54248046875, -1667.5568847656))
											elseif (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 150 then
												if Modstween then Modstween:Stop() end
												game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
											end 
										end
									end
								elseif not World1 then
									Com("F_","TravelMain")
								elseif World1 then
									if _G.Auto_Farm_Level == false then
								end
									CheckMaterial("Fish Tail")
									if CustomFindFirstChild(MaterialMob) then
										for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
											if _G.AutoFullyGodhuman and table.find(MaterialMob,v.Name) and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
												repeat wait()
													FarmtoTarget = TP2(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
													if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 150 then
														if FarmtoTarget then FarmtoTarget:Stop() end
														EquipWeapon(_G.SelectWeapon)
														spawn(function()
															for i,v2 in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
																if v2.Name == v.Name then
																	spawn(function()
																		if InMyNetWork(v2.HumanoidRootPart) then
																			v2.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
																			v2.Humanoid.JumpPower = 0
																			v2.Humanoid.WalkSpeed = 0
																			v2.HumanoidRootPart.CanCollide = false
																			v2.Humanoid:ChangeState(11)
																			v2.HumanoidRootPart.Size = Vector3.new(80,80,80)
																		end
																	end)
																end
															end
														end)
														TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
													end
												until not CustomFindFirstChild(MaterialMob) or not _G.AutoFullyGodhuman or v.Humanoid.Health <= 0 or not v.Parent
											end
										end
									else
										FastAttack = false
										Modstween = TP2(CFrameMon.Position,CFrameMon)
										if World1 and (table.find(MaterialMob,"Fishman Commando [Lv. 400]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
											if Modstween then Modstween:Stop() end wait(.5)
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
										elseif World1 and not (table.find(MaterialMob,"Fishman Commando [Lv. 400]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 50000 then
											if Modstween then Modstween:Stop() end wait(.5)
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(3864.8515625, 6.6796875, -1926.7841796875))
										elseif World1 and (table.find(MaterialMob,"God's Guard [Lv. 450]")) and (CFrameMon.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 3000 then
											if Modstween then Modstween:Stop() end wait(.5)
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-4607.8227539063, 872.54248046875, -1667.5568847656))
										elseif (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 150 then
											if Modstween then Modstween:Stop() end
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
										end 
									end
								end
							end
						end
					end)
				end
			end)
	
	spawn(function()
		while wait() do
			pcall(function()
				if _G.AutoFullyGodhuman and World2 then
					if game.Workspace.Enemies:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") or game.ReplicatedStorage:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") then
						if (KillSharkMan == true and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true) == "I lost my house keys, could you help me find them? Thanks.") then
							if KillFish then KillFish:Stop() end
							Com("F_","SetSpawnPoint")
							for i,v in pairs(game.Workspace.Enemies:GetChildren()) do 
								if v.Name == "Tide Keeper [Lv. 1475] [Boss]" then
									repeat wait()
										if game.Workspace.Enemies:FindFirstChild(v.Name) then
											if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 200 then
												Farmtween = TP2(v.HumanoidRootPart.CFrame)
											elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 200 then
												if Farmtween then Farmtween:Stop() end
												EquipWeapon(_G.SelectWeapon)
												v.Humanoid.JumpPower = 0
												v.Humanoid.WalkSpeed = 0
												v.HumanoidRootPart.CanCollide = false
												v.Humanoid:ChangeState(11)
												TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
											end
										end
									until not v.Parent or not _G.AutoFullyGodhuman or KillSharkMan == false or v.Humanoid.Health == 0 or game.Players.LocalPlayer.Character:FindFirstChild("Water Key") or game.Players.LocalPlayer.Backpack:FindFirstChild("Water Key")
								end
							end
						end
					else
						if game:GetService("ReplicatedStorage"):FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") then
							KillFish = TP2(game:GetService("ReplicatedStorage"):FindFirstChild("Tide Keeper [Lv. 1475] [Boss]").HumanoidRootPart.CFrame)
						else
							if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true) == "I lost my house keys, could you help me find them? Thanks." then
								Hop()
							end
						end
					end
				end
			end)
		end
	end)
	
		Main:Seperator("Mastery")
			
		Main:Toggle("Auto Farm BF Mastery",_G.AutoFarmFruitMastery,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)			
			else
			_G.AutoFarmFruitMastery = value
			StopTween(_G.AutoFarmFruitMastery)
			end
		end)
		
		spawn(function()
			while wait() do
				if _G.AutoFarmFruitMastery then
					pcall(function()
						local QuestTitle = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
						if not string.find(QuestTitle, NameMon) then
							UseSkill = false
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
						end
						if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
							UseSkill = false
							StartMasteryFruitMagnet = false
							CheckLevel()
							repeat wait()
								TP(CFrameQuest)
							until (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.AutoFarmFruitMastery
							if (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest",NameQuest,LevelQuest)
							end
						elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
							CheckLevel()
							if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
								for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
									if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
										if v.Name == Ms then
											if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
												HealthMs = v.Humanoid.MaxHealth * _G.Kill_At/100
												repeat task.wait()
													if v.Humanoid.Health <= HealthMs then
														AutoHaki()
														EquipWeapon(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value)
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														v.HumanoidRootPart.CanCollide = false
											            v.Humanoid:ChangeState(11)
														v.Humanoid.JumpPower = 0
														v.Humanoid.WalkSpeed = 0
														PosMonMasteryFruit = v.HumanoidRootPart.CFrame														
														UseSkill = true
													else           
														UseSkill = false
														EquipWeapon(_G.SelectWeapon)
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														v.HumanoidRootPart.CanCollide = false
										            	v.Humanoid:ChangeState(11)
														v.Humanoid.JumpPower = 0
														v.Humanoid.WalkSpeed = 0
														v.HumanoidRootPart.Size = Vector3.new(60,60,60)
														wait(0.2)
														PosMonMasteryFruit = v.HumanoidRootPart.CFrame
													end
													StartMasteryFruitMagnet = true
													game:GetService("VirtualUser"):CaptureController()
													game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670),workspace.CurrentCamera.CFrame)
												until not _G.AutoFarmFruitMastery or v.Humanoid.Health <= 0 or not v.Parent or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
											else
												UseSkill = false
												StartMasteryFruitMagnet = false
												TP(CFrameMon)
												game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
											end
										end
									end
								end
							else
								StartMasteryFruitMagnet = false   
								UseSkill = false 
								TP(CFrameMon)
							end
						end
					end)
				end
			end
		end)
		
		spawn(function()
			while wait() do
				if UseSkill then
					pcall(function()
						CheckLevel()
						for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value) then
								MasBF = game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Data.DevilFruit.Value].Level.Value
							elseif game:GetService("Players").LocalPlayer.Backpack:FindFirstChild(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value) then
								MasBF = game:GetService("Players").LocalPlayer.Backpack[game:GetService("Players").LocalPlayer.Data.DevilFruit.Value].Level.Value
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon-Dragon") then                      
								if _G.SkillZ then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                        
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
								end
								if _G.SkillC then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                          
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"C",false,game)
									wait(4)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"C",false,game)
								end
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Venom-Venom") then   
								if _G.SkillZ then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                        
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
									wait(2)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
								end
								if _G.SkillX then        
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))               
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
								end
								if _G.SkillC then 
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                          
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"C",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"C",false,game)
								end
									if _G.SkillF then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"F",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"F",false,game)
								end
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Human-Human: Buddha") then
								if _G.SkillZ and game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Size == Vector3.new(2, 2.0199999809265, 1) then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                         
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
								end
								if _G.SkillX then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
								end
								if _G.SkillC then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"C",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"C",false,game)
								end
								if _G.SkillV then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"V",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"V",false,game)
								end
								if _G.SkillF then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"F",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"F",false,game)
								end
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Portal-Portal") then
								if _G.SkillZ and game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Size == Vector3.new(2, 2.0199999809265, 1) then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                         
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
								end
								if _G.SkillX then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
								end
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dark-Dark") then
								if _G.SkillZ and game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Size == Vector3.new(2, 2.0199999809265, 1) then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                         
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
								end
								if _G.SkillX then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
									wait(2.5)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
								end
								if _G.SkillV then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"V",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"V",false,game)
								end
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value) then
								if _G.SkillZ then 
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                         
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
								end
								if _G.SkillX then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
								end
								if _G.SkillC then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"C",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"C",false,game)
								end
								if _G.SkillV then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"V",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"V",false,game)
								end
								if _G.SkillF then
									local args = {
										[1] = PosMonMasteryFruit.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"F",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"F",false,game)
								end
							end
						end
					end)
				end
			end
		end)
		
		spawn(function()
			game:GetService("RunService").RenderStepped:Connect(function()
				pcall(function()
					if UseSkill then
						for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Notifications:GetChildren()) do
							if v.Name == "NotificationTemplate" then
								if string.find(v.Text,"Skill locked!") then
									v:Destroy()
								end
							end
						end
					end
				end)
			end)
		end)
		
		spawn(function()
			pcall(function()
				game:GetService("RunService").RenderStepped:Connect(function()
					if UseSkill then
						local args = {
							[1] = PosMonMasteryFruit.Position
						}
						game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Data.DevilFruit.Value].RemoteEvent:FireServer(unpack(args))
					end
				end)
			end)
		end)
		
		Main:Toggle("Auto Farm Gun Mastery",_G.AutoFarmGunMastery,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoFarmGunMastery = value
			StopTween(_G.AutoFarmGunMastery)
			end
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if _G.AutoFarmGunMastery then
						local QuestTitle = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
						if not string.find(QuestTitle, NameMon) then
							UseSkillGun = false 
							StartMasteryGunMagnet = false
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
						end
						if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
							UseSkillGun = false 
							StartMasteryGunMagnet = false
							CheckLevel()
							TP(CFrameQuest)
							if (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 10 then
								task.wait()
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NameQuest, LevelQuest)
							end
						elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
							CheckLevel()
							if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
								pcall(function()
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v.Name == Ms then
											repeat task.wait()
												if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
													HealthMin = v.Humanoid.MaxHealth * _G.Kill_At/100
													if v.Humanoid.Health <= HealthMin then         
														EquipWeapon(SelectToolWeaponGun)
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														v.Humanoid.JumpPower = 0
														v.Humanoid.WalkSpeed = 0                                                    
														v.HumanoidRootPart.CanCollide = false
														v.HumanoidRootPart.Size = Vector3.new(120,120,120)
														v.Head.CanCollide = false                                                
														local args = {
															[1] = v.HumanoidRootPart.Position,
															[2] = v.HumanoidRootPart
														}
														game:GetService("Players").LocalPlayer.Character[SelectToolWeaponGun].RemoteFunctionShoot:InvokeServer(unpack(args))
														UseSkillGun = true 
													else
														UseSkillGun = false 
														AutoHaki()
														EquipWeapon(_G.SelectWeapon)
														v.Humanoid.JumpPower = 0
														v.Humanoid.WalkSpeed = 0         
														v.HumanoidRootPart.CanCollide = false
														v.Head.CanCollide = false               
														v.HumanoidRootPart.Size = Vector3.new(120,120,120)
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
													end
													StartMasteryGunMagnet = true
													wait(0.2)
													PosMonMasteryGun = v.HumanoidRootPart.CFrame
													game:GetService'VirtualUser':CaptureController()
													game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
												else
													UseSkillGun = false 
													StartMasteryGunMagnet = false
													TP(CFrameMon)
													game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
												end
											until v.Humanoid.Health <= 0 or _G.AutoFarmGunMastery == false or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
											StartMasteryGunMagnet = false
											UseSkillGun = false 
										end
									end
								end)
							else
								StartMasteryGunMagnet = false
								UseSkillGun = false 
								TP(CFrameMon)
								local Mob = game:GetService("ReplicatedStorage"):FindFirstChild(Ms) 
								if Mob then
									TP(Mob.HumanoidRootPart.CFrame * CFrame.new(5,35,5))
								end
							end 
						end
					end
				end
			end)
		end)
		
		spawn(function()
			while wait() do
				if UseSkillGun then
					pcall(function()
						CheckLevel()
						for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do                                                 
								if _G.SkillGunZ then
									local args = {
										[1] = PosMonMasteryGun.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                        
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
								end
								if _G.SkillGunX then          
									local args = {
										[1] = PosMonMasteryGun.Position
									}
									game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))               
									game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
									game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
							end
						end
					end)
				end
			end
		end)
		
		spawn(function()
			game:GetService("RunService").RenderStepped:Connect(function()
				pcall(function()
					if UseSkillGun then
						for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Notifications:GetChildren()) do
							if v.Name == "NotificationTemplate" then
								if string.find(v.Text,"Skill locked!") then
									v:Destroy()
								end
							end
						end
					end
				end)
			end)
		end)
		
		spawn(function()
			pcall(function()
				game:GetService("RunService").RenderStepped:Connect(function()
					if UseSkillGun then
						local args = {
							[1] = PosMonMasteryGun.Position
						}
						game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Data.Gun.Value].RemoteEvent:FireServer(unpack(args))
					end
				end)
			end)
		end)
	
		function MaterialMon()
			if _G.SelectMaterial == "Radioactive Material" then
				MMon = "Factory Staff [Lv. 800]"
				MPos = CFrame.new(-507.7895202636719, 72.99479675292969, -126.45632934570312)
				SP = "Bar"
			elseif _G.SelectMaterial == "Mystic Droplet" then
				MMon = "Water Fighter [Lv. 1450]"
				MPos = CFrame.new(-3214.218017578125, 298.69952392578125, -10543.685546875)
				SP = "ForgottenIsland"
			elseif _G.SelectMaterial == "Magma Ore" then
				if game.PlaceId == 2753915549 then
					MMon = "Military Spy [Lv. 325]"
					MPos = CFrame.new(-5850.2802734375, 77.28675079345703, 8848.6748046875)
					SP = "Magma"
				elseif game.PlaceId == 4442272183 then
					MMon = "Lava Pirate [Lv. 1200]"
					MPos = CFrame.new(-5234.60595703125, 51.953372955322266, -4732.27880859375)
					SP = "CircleIslandFire"
				end
			elseif _G.SelectMaterial == "Angel Wings" then
				MMon = "Royal Soldier [Lv. 550]"
				MPos = CFrame.new(-7827.15625, 5606.912109375, -1705.5833740234375)
				SP = "Sky2"
			elseif _G.SelectMaterial == "Leather" then
				if game.PlaceId == 2753915549 then
					MMon = "Pirate [Lv. 36]"
					MPos = CFrame.new(-1211.8792724609375, 4.787090301513672, 3916.83056640625)
					SP = "Pirate"
				elseif game.PlaceId == 4442272183 then
					MMon = "Marine Captain [Lv. 900]"
					MPos = CFrame.new(-2010.5059814453125, 73.00115966796875, -3326.620849609375)
					SP = "Greenb"
				elseif game.PlaceId == 7449423635 then
					MMon = "Jungle Pirate [Lv. 1900]"
					MPos = CFrame.new(-11975.78515625, 331.7734069824219, -10620.0302734375)
					SP = "PineappleTown"
				end
			elseif _G.SelectMaterial == "Scrap Metal" then
				if game.PlaceId == 2753915549 then
					MMon = "Brute [Lv. 45]"
					MPos = CFrame.new(-1132.4202880859375, 14.844913482666016, 4293.30517578125)
					SP = "Pirate"
				elseif game.PlaceId == 4442272183 then
					MMon = "Mercenary [Lv. 725]"
					MPos = CFrame.new(-972.307373046875, 73.04473876953125, 1419.2901611328125)
					SP = "DressTown"
				elseif game.PlaceId == 7449423635 then
					MMon = "Pirate Millionaire [Lv. 1500]"
					MPos = CFrame.new(-289.6311950683594, 43.8282470703125, 5583.66357421875)
					SP = "Default"
				end
			elseif _G.SelectMaterial == "Demonic Wisp" then
				MMon = "Demonic Soul [Lv. 2025]"
				MPos = CFrame.new(-9503.388671875, 172.139892578125, 6143.0634765625)
				SP = "HauntedCastle"
			elseif _G.SelectMaterial == "Vampire Fang" then
				MMon = "Vampire [Lv. 975]"
				MPos = CFrame.new(-5999.20458984375, 6.437741279602051, -1290.059326171875)
				SP = "Graveyard"
			elseif _G.SelectMaterial == "Conjured Cocoa" then
				MMon = "Chocolate Bar Battler [Lv. 2325]"
				MPos = CFrame.new(744.7930908203125, 24.76934242248535, -12637.7255859375)
				SP = "Chocolate"
			elseif _G.SelectMaterial == "Dragon Scale" then
				MMon = "Dragon Crew Warrior [Lv. 1575]"
				MPos = CFrame.new(5824.06982421875, 51.38640213012695, -1106.694580078125)
				SP = "Hydra1"
			elseif _G.SelectMaterial == "Gunpowder" then
				MMon = "Pistol Billionaire [Lv. 1525]"
				MPos = CFrame.new(-379.6134338378906, 73.84449768066406, 5928.5263671875)
				SP = "Default"
			elseif _G.SelectMaterial == "Fish Tail" then
				MMon = "Fishman Captain [Lv. 1800]"
				MPos = CFrame.new(-10961.0126953125, 331.7977600097656, -8914.29296875)
				SP = "PineappleTown"
			elseif _G.SelectMaterial == "Mini Tusk" then
				MMon = "Mythological Pirate [Lv. 1850]"
				MPos = CFrame.new(-13516.0458984375, 469.8182373046875, -6899.16064453125)
				SP = "BigMansion"
			end
		end
	
	local MaterialMethod
	if World1 then
	MaterialMethod = {
	"Magma Ore",
	"Angel Wings",
	"Leather",
	"Scrap Metal",
	"Radioactive Material",
	}
	elseif World2 then
	MaterialMethod = {
	"Mystic Droplet",
	"Magma Ore",
	"Leather",
	"Scrap Metal",
	"Demonic Wisp",
	"Vampire Fang",
	"Radioactive Material",
	}
	elseif World3 then
	MaterialMethod = {
	"Leather",
	"Scrap Metal",
	"Vampire Fang",
	"Conjured Cocoa",
	"Dragon Scale",
	"Gunpowder",
	"Fish Tail",
	"Mini Tusk",
	"Radioactive Material",
	}
	end
	
	Main:Seperator("Materials")
	
	local SelectMaterial = Main:Dropdown("Select Material",MaterialMethod,function(value)
	_G.SelectMaterial = value
	end)
	
	Main:Toggle("Auto Farm Material",_G.AutoFarmMaterial,function(t)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
		_G.AutoFarmMaterial = t
		StopTween(_G.AutoFarmMaterial)
		end
	end)
		
	spawn(function()
			while wait() do
				pcall(function()
					if _G.AutoFarmMaterial and _G.SelectMaterial then
						MaterialMon()
						if game.Workspace.Enemies:FindFirstChild(MMon) then
							for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
								if v.Name == MMon then
									if v:FindFirstChild("HumanoidRootPart") then
										repeat task.wait()
											AutoHaki()
											EquipWeapon(_G.SelectWeapon)
												PosMon = v.HumanoidRootPart.CFrame
												v.HumanoidRootPart.CanCollide = false
												v.Humanoid.WalkSpeed = 0
												v.Head.CanCollide = false
												v.HumanoidRootPart.Size = Vector3.new(50,50,50)
												StartMagnetMaterial = true
												TP(v.HumanoidRootPart.CFrame * Farm_Mode)
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
											MatMon = v.Name
											MatPos = v.HumanoidRootPart.CFrame
										until not _G.AutoFarmMaterial or not v.Parent or v.Humanoid.Health <= 0
									end
								end
							end
						else
							TP(MPos)
						end
					end
				end)
			end
		end)
	
		Main:Seperator("Bosses")
		
		local Boss = {}
		
		for i, v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
			if string.find(v.Name, "Boss") then
				if v.Name == "Ice Admiral [Lv. 700] [Boss]" then
					else
					table.insert(Boss, v.Name)
				end
			end
		end
		
		local BossName = Main:Dropdown("Select Boss",Boss,function(value)
			_G.Select_Boss = value
		end)
		
		Main:Button("Refresh Boss",function()
			BossName:Clear()
				for i, v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
				if string.find(v.Name, "Boss") then
					BossName:Add(v.Name) 
				end
			end
		end)
		
		Main:Toggle("Auto Farm Boss",_G.AutoFarmBoss,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoFarmBoss = value
			StopTween(_G.AutoFarmBoss)
			end
		end)
		
		Main:Toggle("Auto Quest Boss",true,function(value)
			_G.AutoQuestBoss = value
		end)
		   
		   spawn(function()
			   while wait(.1) do
				   if _G.AutoFarmBoss then
					   pcall(function()
						CheckBossQuest()
						   if MsBoss == "Soul Reaper [Lv. 2100] [Raid Boss]" or MsBoss == "Longma [Lv. 2000] [Boss]" or MsBoss == "Don Swan [Lv. 1000] [Boss]" or MsBoss == "Cursed Captain [Lv. 1325] [Raid Boss]" or MsBoss == "Order [Lv. 1250] [Raid Boss]" or MsBoss == "rip_indra True Form [Lv. 5000] [Raid Boss]" then
							   if game:GetService("Workspace").Enemies:FindFirstChild(MsBoss) then
								   for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
									   if v.Name == MsBoss then
										   repeat task.wait()
											   EquipWeapon(_G.SelectWeapon)
											   AutoHaki()
											   TP(v.HumanoidRootPart.CFrame * Farm_Mode)
											   v.HumanoidRootPart.CanCollide = false
											   v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
											   game:GetService'VirtualUser':CaptureController()
											   game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										   until _G.AutoFarmBoss == false or not v.Parent or v.Humanoid.Health <= 0
									   end
								   end
							   else
								   TP(CFrameBoss)
							   end
						   else
							   if _G.AutoQuestBoss then
								CheckBossQuest()
								   if not string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameBoss) then
									game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer("AbandonQuest")
								end
								   if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
									   repeat task.wait() TP(CFrameQuestBoss) until (CFrameQuestBoss.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.Auto_Farm_Boss
									   if (CFrameQuestBoss.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 then
										   wait(1.1)
										   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NameQuestBoss, LevelQuestBoss)
									   end
								   elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
									   if game:GetService("Workspace").Enemies:FindFirstChild(MsBoss) then
										   for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
											   if v.Name == MsBoss then
												   repeat task.wait()
													   if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameBoss) then
														   EquipWeapon(_G.SelectWeapon)
														   AutoHaki()
														   TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														   v.HumanoidRootPart.CanCollide = false
														   v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
														   game:GetService'VirtualUser':CaptureController()
														   game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))									
													   else
														game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer("AbandonQuest")
													end
												   until _G.AutoFarmBoss == false or not v.Parent or v.Humanoid.Health <= 0
											   end
										   end
									   else
										   TP(CFrameBoss)
									   end
								   end
							   else
								   if game:GetService("Workspace").Enemies:FindFirstChild(MsBoss) then
									   for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										   if v.Name == MsBoss then
											   repeat task.wait()
												   EquipWeapon(_G.SelectWeapon)
												   AutoHaki()
												   TP(v.HumanoidRootPart.CFrame * Farm_Mode)
												   v.HumanoidRootPart.CanCollide = false
												   v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
												   game:GetService'VirtualUser':CaptureController()
												   game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))										
											   until _G.AutoFarmBoss == false or not v.Parent or v.Humanoid.Health <= 0
										   end
									   end
								   else
									   TP(CFrameBoss)
								   end
							   end
						   end
					   end)
				   end
			   end
		   end)
	
		Main:Toggle("Auto Farm All Boss",_G.AutoAllBoss,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoAllBoss = value
			StopTween(_G.AutoAllBoss)
			end
		end)
		
		Main:Toggle("Auto Farm All Boss Hop",_G.AutoAllBossHop,function(value)
			_G.AutoAllBossHop = value
		end)
		
		spawn(function()
			while wait(.1) do
				if _G.AutoAllBoss then
					pcall(function()
						for i,v in pairs(game.ReplicatedStorage:GetChildren()) do
							if string.find(v.Name,"Boss") then
								if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude < 17000 then
									repeat task.wait()
										AutoHaki()
										EquipWeapon(_G.SelectWeapon)
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										v.HumanoidRootPart.Size = Vector3.new(80,80,80)
										TP(v.HumanoidRootPart.CFrame * Farm_Mode)
										game:GetService'VirtualUser':CaptureController()
										game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
									until v.Humanoid.Health <= 0 or _G.AutoAllBoss == false or not v.Parent
								end
							else
								if _G.AutoAllBossHop then
									Hop()
								end
							end
						end
					end)
				end
			end
		end)
	
		if World2 or World3 then
		Main:Seperator("Sea Beasts")
		
		local Sea = Main:Label("Sea Beast : 0")
		
		spawn(function()
			while wait(.1) do
				local countS = 0
				for i,v in pairs(game:GetService("Workspace").SeaBeasts:GetChildren()) do
					countS = countS + 1
				end
				Sea:Set("Sea Beast : "..countS)
			end
		end)
	
		Main:Toggle("Auto Sea Beast",_G.AutoSeaBest,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
		_G.AutoSeaBest = value
		StopTween(_G.AutoSeaBest)
			end
		end)
		
		Main:Toggle("Auto Sea Beast Hop",_G.AutoSeaBestHop,function(value)
		_G.AutoSeaBestHop = value
		end)
	
		spawn(function()
			pcall(function()
				while wait(.1) do
					if (_G.AutoSeaBestHop) and World2 and Wolrd3 and not game:GetService("ReplicatedStorage"):FindFirstChild("SeaBeasts") and not game:GetService("Workspace").SeaBeasts:FindFirstChild("SeaBeasts") then
						Hop()
					end
				end
			end)
		end)
		
				spawn(function()
					while wait() do
						if _G.AutoSeaBest then
							pcall(function()
								for i,v in pairs(game:GetService("Workspace").SeaBeasts:GetChildren()) do
									if v:FindFirstChild("HumanoidRootPart") then 
										AutoHaki()
										EquipWeapon(_G.SelectWeapon)
										TP(v.HumanoidRootPart.CFrame * CFrame.new(5,500,7))
										if _G.AutoSeaBest and (game:GetService("Workspace").SeaBeasts.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 60 then
										   game:service('VirtualInputManager'):SendKeyEvent(true, "Z", false, game)
										   game:service('VirtualInputManager'):SendKeyEvent(false, "Z", false, game)
										if _G.AutoSeaBest and (game:GetService("Workspace").SeaBeasts.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 60 then
										   game:service('VirtualInputManager'):SendKeyEvent(true, "X", false, game)
										   game:service('VirtualInputManager'):SendKeyEvent(false, "X", false, game)
										if _G.AutoSeaBest and (game:GetService("Workspace").SeaBeasts.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 60 then
										   game:service('VirtualInputManager'):SendKeyEvent(true, "C", false, game)
										   game:service('VirtualInputManager'):SendKeyEvent(false, "C", false, game)
										end
									end
								end
							end
						end
					end)
				end
			end
		end)
	end
	
		Main:Seperator("Auto Farm Chest")
	
		Main:Toggle("Auto Chest Bypass",false,function(vu)
		_G.ChestBypass = vu
		end)
		
spawn(function()
	while wait() do
		if _G.ChestBypass then
			pcall(function()
				for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
					if string.find(v.Name, "Chest") then
					   game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
					end
			    end
	     	end)
	    end
	end
end)
		
		Main:Toggle("Auto Chest Tween",_G.Grab_Chest,function(value)
		Grab_Chest = value
		StopTween(Grab_Chest)
		end)
		
		Main:Toggle("Auto Chest Stop Torch",_G.STP,function(value)
		Grab_Chest = value
		_G.STP = value
		T_P_H = value
		StopTween(Grab_Chest)
		end)
		
		spawn(function()
			while wait() do
				pcall(function()
					if Grab_Chest then
						if T_P_H then
							if game.Players.LocalPlayer.Backpack:FindFirstChild("Fist of Darkness") or game.Players.LocalPlayer.Character:FindFirstChild("Fist of Darkness") then
								TP(CFrame.new(-379.70889282227, 73.0458984375, 304.84692382813))
								H_F = true
								game:GetService'VirtualUser':Button1Down(Vector2.new(1280,600))
								wait()
							else
								StopTween(Grab_Chest)
								_G.Chest_100 = nil
								_G.Chest_500 = nil
								_G.Chest_1000 = nil
								_G.Chest_1500 = nil
								_G.Chest_2000 = nil
								_G.Chest_2500 = nil
								_G.Chest_3500 = nil
								_G.Chest_4500 = nil
								_G.Chest_5500 = nil
								_G.Chest_6500 = nil
								_G.Chest_7500 = nil
								_G.Chest_9500 = nil
								_G.Chest_10500 = nil
								_G.Chest_12500 = nil
								_G.Chest_15500 = nil
								_G.Chest_17500 = nil
								Chest_100()
								Chest_500()
								Chest_1000()
								Chest_1500()
								Chest_2000()
								Chest_2500()
								Chest_3500()
								Chest_4500()
								Chest_5500()
								Chest_6500()
								Chest_7500()
								Chest_9500()
								Chest_10500()
								Chest_12500()
								Chest_15500()
								Chest_17500()
								if _G.Chest_100 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_100.CFrame)
									until not _G.Chest_100.Parent or not Grab_Chest
								elseif _G.Chest_500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_500.CFrame)
									until not _G.Chest_500.Parent or not Grab_Chest
								elseif _G.Chest_1000 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_1000.CFrame)
									until not _G.Chest_1000.Parent or not Grab_Chest
								elseif _G.Chest_1500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_1500.CFrame)
									until not _G.Chest_1500.Parent or not Grab_Chest
								elseif _G.Chest_2000 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_2000.CFrame)
									until not _G.Chest_2000.Parent or not Grab_Chest
								elseif _G.Chest_2500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_2500.CFrame)
									until not _G.Chest_2500.Parent or not Grab_Chest
								elseif _G.Chest_3500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_3500.CFrame)
									until not _G.Chest_3500.Parent or not Grab_Chest
								elseif _G.Chest_4500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_4500.CFrame)
									until not _G.Chest_4500.Parent or not Grab_Chest
								elseif _G.Chest_5500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_5500.CFrame)
									until not _G.Chest_5500.Parent or not Grab_Chest
								elseif _G.Chest_6500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_6500.CFrame)
									until not _G.Chest_6500.Parent or not Grab_Chest
								elseif _G.Chest_7500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_7500.CFrame)
									until not _G.Chest_7500.Parent or not Grab_Chest
								elseif _G.Chest_9500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_9500.CFrame)
									until not _G.Chest_9500.Parent or not Grab_Chest
								elseif _G.Chest_10500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_10500.CFrame)
									until not _G.Chest_10500.Parent or not Grab_Chest
								elseif _G.Chest_12500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_12500.CFrame)
									until not _G.Chest_12500.Parent or not Grab_Chest
								elseif _G.Chest_15500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_15500.CFrame)
									until not _G.Chest_15500.Parent or not Grab_Chest
								elseif _G.Chest_17500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_17500.CFrame)
									until not _G.Chest_17500.Parent or not Grab_Chest
								end
							end
						else
							StopTween(Grab_Chest)
								_G.Chest_100 = nil
								_G.Chest_500 = nil
								_G.Chest_1000 = nil
								_G.Chest_1500 = nil
								_G.Chest_2000 = nil
								_G.Chest_2500 = nil
								_G.Chest_3500 = nil
								_G.Chest_4500 = nil
								_G.Chest_5500 = nil
								_G.Chest_6500 = nil
								_G.Chest_7500 = nil
								_G.Chest_9500 = nil
								_G.Chest_10500 = nil
								_G.Chest_12500 = nil
								_G.Chest_15500 = nil
								_G.Chest_17500 = nil
								Chest_100()
								Chest_500()
								Chest_1000()
								Chest_1500()
								Chest_2000()
								Chest_2500()
								Chest_3500()
								Chest_4500()
								Chest_5500()
								Chest_6500()
								Chest_7500()
								Chest_9500()
								Chest_10500()
								Chest_12500()
								Chest_15500()
								Chest_17500()
								if _G.Chest_100 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_100.CFrame)
									until not _G.Chest_100.Parent or not Grab_Chest
								elseif _G.Chest_500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_500.CFrame)
									until not _G.Chest_500.Parent or not Grab_Chest
								elseif _G.Chest_1000 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_1000.CFrame)
									until not _G.Chest_1000.Parent or not Grab_Chest
								elseif _G.Chest_1500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_1500.CFrame)
									until not _G.Chest_1500.Parent or not Grab_Chest
								elseif _G.Chest_2000 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_2000.CFrame)
									until not _G.Chest_2000.Parent or not Grab_Chest
								elseif _G.Chest_2500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_2500.CFrame)
									until not _G.Chest_2500.Parent or not Grab_Chest
								elseif _G.Chest_3500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_3500.CFrame)
									until not _G.Chest_3500.Parent or not Grab_Chest
								elseif _G.Chest_4500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_4500.CFrame)
									until not _G.Chest_4500.Parent or not Grab_Chest
								elseif _G.Chest_5500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_5500.CFrame)
									until not _G.Chest_5500.Parent or not Grab_Chest
								elseif _G.Chest_6500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_6500.CFrame)
									until not _G.Chest_6500.Parent or not Grab_Chest
								elseif _G.Chest_7500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_7500.CFrame)
									until not _G.Chest_7500.Parent or not Grab_Chest
								elseif _G.Chest_9500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_9500.CFrame)
									until not _G.Chest_9500.Parent or not Grab_Chest
								elseif _G.Chest_10500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_10500.CFrame)
									until not _G.Chest_10500.Parent or not Grab_Chest
								elseif _G.Chest_12500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_12500.CFrame)
									until not _G.Chest_12500.Parent or not Grab_Chest
								elseif _G.Chest_15500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_15500.CFrame)
									until not _G.Chest_15500.Parent or not Grab_Chest
								elseif _G.Chest_17500 ~= nil then
									repeat wait(.3)
										TP(_G.Chest_17500.CFrame)
									until not _G.Chest_17500.Parent or not Grab_Chest
							end
						end
					end
				end)
			end
			end)
			
			function Chest_100()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 100 then
					_G.Chest_100 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 100 then
					_G.Chest_100 = v
					return
				end
			end
			end
			function Chest_500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 500 then
					_G.Chest_500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 500 then
					_G.Chest_500 = v
					return
				end
			end
			end
			function Chest_1000()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1000 then
					_G.Chest_1000 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1000 then
					_G.Chest_1000 = v
					return
				end
			end
			end
			function Chest_1500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1500 then
					_G.Chest_1500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1500 then
					_G.Chest_1500 = v
					return
				end
			end
			end
			function Chest_2000()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 2000 then
					_G.Chest_2000 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 2000 then
					_G.Chest_2000 = v
					return
				end
			end
			end
			function Chest_2500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 2500 then
					_G.Chest_2500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 2500 then
					_G.Chest_2500 = v
					return
				end
			end
			end
			function Chest_3500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3500 then
					_G.Chest_3500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3500 then
					_G.Chest_3500 = v
					return
				end
			end
			end
			function Chest_4500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4500 then
					_G.Chest_4500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4500 then
					_G.Chest_4500 = v
					return
				end
			end
			end
			function Chest_5500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 5500 then
					_G.Chest_5500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 5500 then
					_G.Chest_5500 = v
					return
				end
			end
			end
			function Chest_6500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 6500 then
					_G.Chest_6500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 6500 then
					_G.Chest_6500 = v
					return
				end
			end
			end
			function Chest_7500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 7500 then
					_G.Chest_7500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 7500 then
					_G.Chest_7500 = v
					return
				end
			end
			end
			function Chest_9500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 9500 then
					_G.Chest_9500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 9500 then
					_G.Chest_9500 = v
					return
				end
			end
			end
			function Chest_10500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 10500 then
					_G.Chest_10500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 10500 then
					_G.Chest_10500 = v
					return
				end
			end
			end
			function Chest_12500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 12500 then
					_G.Chest_12500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 12500 then
					_G.Chest_12500 = v
					return
				end
			end
			end
			function Chest_15500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 15500 then
					_G.Chest_15500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 15500 then
					_G.Chest_15500 = v
					return
				end
			end
			end
			function Chest_17500()
			for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
				if v.Name == "Chest1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 17500 then
					_G.Chest_17500 = v
					return
				elseif v.Name == "Chest2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 17500 then
					_G.Chest_17500 = v
					return
				end
			end
			end
			
		if World3 then
			Main:Seperator("[ EVENT ]")
	
			Main:Toggle("Auto Hearts", false, function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoHearts = value
			StopTween(_G.AutoHearts)
			end
			end)
			
			spawn(function()
				while wait() do 
					if _G.AutoHearts then
						pcall(function()
							if game:GetService("Workspace").Enemies:FindFirstChild("Sweet Thief [Lv. 2350]") or game:GetService("Workspace").Enemies:FindFirstChild("Candy Rebel [Lv. 2375]") or game:GetService("Workspace").Enemies:FindFirstChild("Candy Pirate [Lv. 2400]") or game:GetService("Workspace").Enemies:FindFirstChild("Snow Demon [Lv. 2425]") then
								for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
									if v.Name == "Sweet Thief [Lv. 2350]" or v.Name == "Candy Rebel [Lv. 2375]" or v.Name == "Candy Pirate [Lv. 2400]" or v.Name == "Snow Demon [Lv. 2425]" then
										if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											repeat task.wait()
												AutoHaki()
												EquipWeapon(_G.SelectWeapon)
												v.HumanoidRootPart.CanCollide = false
												v.Head.CanCollide = false 
												v.Humanoid:ChangeState(11)
												HeartsMon = v.HumanoidRootPart.CFrame
												StartHeartsMagnet = true
												TP(v.HumanoidRootPart.CFrame * Farm_Mode)
												game:GetService("VirtualUser"):CaptureController()
												game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
											until not _G.AutoHearts or not v.Parent or v.Humanoid.Health <= 0
										end
									end
								end
							else
								StartHeartsMagnet = false
								for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do 
									if v.Name == "Snow Demon [Lv. 2425]" then
									TP(v.HumanoidRootPart.CFrame * Farm_Mode)  
								elseif v.Name == "Candy Pirate [Lv. 2400]" then
									TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
								elseif v.Name == "Candy Rebel [Lv. 2375]" then
									TP(v.HumanoidRootPart.CFrame * Farm_Mode)  
								elseif v.Name == "Sweet Thief [Lv. 2350]" then
									TP(v.HumanoidRootPart.CFrame * Farm_Mode) 
								else
									if not game:GetService("Workspace").Enemies:FindFirstChild("Sweet Thief [Lv. 2350]") then
										TP(CFrame.new(38.4782219, 97.788147, -12932.6465, 0.930317581, 4.81577223e-09, -0.366755038, -2.24385133e-08, 1, -4.37871854e-08, 0.366755038, 4.89654255e-08, 0.930317581))
									elseif game:GetService("Workspace").Enemies:FindFirstChild("Snow Demon [Lv. 2425]") then
										TP(CFrame.new(-924.273499, 100.931976, -14331.5439, -0.0911905766, -1.29348299e-09, -0.995833457, -1.56020423e-08, 1, 1.29817226e-10, 0.995833457, 1.55488742e-08, -0.0911905766))
									end
								end
							end
						end
					end)
				end
			end
		end)
	end
	
	if World3 then
	Main:Toggle("Auto Farm Candy", false, function(value)
		if _G.SelectWeapon == nil then
			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
			wait(1)
			Notification:Notify(
				{Title = "Pado Hub", Description = "Select Weapon"},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
			)
		else
		_G.AutoFarmCandy = value
		StopTween(_G.AutoFarmCandy)
		end
	end)
	
	spawn(function()
		while wait() do
			pcall(function()
				if _G.AutoFarmCandy then
						 if game:GetService("Workspace").Enemies:FindFirstChild("Candy Pirate [Lv. 2400]") or game:GetService("Workspace").Enemies:FindFirstChild("Snow Demon [Lv. 2425]") then
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								 if v.Name == "Candy Pirate [Lv. 2400]" or v.Name == "Snow Demon [Lv. 2425]" then
									 if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
									  repeat task.wait()
										AutoHaki()
										EquipWeapon(_G.SelectWeapon)
										CandyMon = v.HumanoidRootPart.CFrame
										StartCandyMagnet = true
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.CanCollide = false
										v.Humanoid:ChangeState(11)
										TP(v.HumanoidRootPart.CFrame * Farm_Mode) 
										game:GetService("VirtualUser"):CaptureController()
										game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
									until not _G.AutoFarmCandy or v.Humanoid.Health <= 0 or not v.Parent or v.Humanoid.Health <= 0
								end
							end
						end
					else
						StartCandyMagnet = false
						TP(CFrame.new(-1408.46521, 16.1423531, -14552.2041, 0.90175873, -8.17216943e-08, -0.432239741, 7.81264475e-08, 1, -2.60746162e-08, 0.432239741, -1.02563433e-08, 0.90175873))
						 end
					end
				end)
			 end
		end)
	end
	
		if World2 then
		Main:Seperator("Ectoplasm")
	
		Main:Toggle("Auto Ectoplasm", false, function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
		_G.AutoEctoplasm = value
		StopTween(_G.AutoEctoplasm)
		end
		end)
		
	    spawn(function()
		    while wait() do 
			    if _G.AutoEctoplasm then
				    pcall(function()
						if game:GetService("Workspace").Enemies:FindFirstChild("Ship Deckhand [Lv. 1250]") or game:GetService("Workspace").Enemies:FindFirstChild("Ship Engineer [Lv. 1275]") or game:GetService("Workspace").Enemies:FindFirstChild("Ship Steward [Lv. 1300]") or game:GetService("Workspace").Enemies:FindFirstChild("Ship Officer [Lv. 1325]") then
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v.Name == "Ship Deckhand [Lv. 1250]" or v.Name == "Ship Engineer [Lv. 1275]" or v.Name == "Ship Steward [Lv. 1300]" or v.Name == "Ship Officer [Lv. 1325]" then
									if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										repeat wait()
											AutoHaki()
											EquipWeapon(_G.SelectWeapon)
											v.HumanoidRootPart.CanCollide = false
											v.Head.CanCollide = false 
                                            v.Humanoid:ChangeState(11)
											EctoplasmMon = v.HumanoidRootPart.CFrame
											StartEctoplasmMagnet = true
											TP(v.HumanoidRootPart.CFrame * Farm_Mode)
											game:GetService("VirtualUser"):CaptureController()
											game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
										until not _G.AutoEctoplasm or not v.Parent or v.Humanoid.Health <= 0
									end
								end
							end
						else
							StartEctoplasmMagnet = false
							local Distance = (Vector3.new(920.3770751953125, 125.08328247070312, 32845.15625) - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
						if Distance > 10000 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
						end
							for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do 
								if v.Name == "Ship Deckhand [Lv. 1250]" then
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
							elseif v.Name == "Ship Engineer [Lv. 1275]" then
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
							elseif v.Name == "Ship Steward [Lv. 1300]" then
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
							elseif v.Name == "Ship Officer [Lv. 1325]" then
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
							end
						end
					end
				end)
			end
		end
		end)
		
		Main:Toggle("Auto Buy Item Ectoplasm All",_G.AutoBuyBizarreRifle,function(A)
			AutoBuyBizarreRifle = A
		end)
	
		spawn(function()
			while wait() do
				if AutoBuyBizarreRifle then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Ectoplasm","Buy",1)
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Ectoplasm","Buy",2)
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Ectoplasm","Buy",3)
				end
			end
		end)
	end

		if World3 then
		Main:Seperator("Dought")
		
		local MobKilled = Main:Label("Killed")
		
		spawn(function()
			while wait(.1) do
				pcall(function()
					if string.len(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")) == 88 then
						MobKilled:Set("Need Kill Mods : "..string.sub(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"),39,41))
					elseif string.len(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")) == 87 then
						MobKilled:Set("Need Kill Mods : "..string.sub(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"),39,40))
					elseif string.len(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")) == 86 then
						MobKilled:Set("Need Kill Mods : "..string.sub(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"),39,39))
					else
						MobKilled:Set("Boss Is Spawning")
					end
				end)
			end
		end)
		
		Main:Toggle("Auto Farm Cake Prince",_G.AutoDoughtBoss,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoDoughtBoss = value
			StopTween(_G.AutoDoughtBoss)
		end
		end)
		
			spawn(function()
				while wait() do
					if _G.AutoDoughtBoss then
						pcall(function()
							if game.ReplicatedStorage:FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") or game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") then   
								if game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do 
										if v.Name == "Cake Prince [Lv. 2300] [Raid Boss]" then
											repeat task.wait()
												AutoHaki()
												EquipWeapon(_G.SelectWeapon)
												v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                                                v.Humanoid:ChangeState(11)
												v.HumanoidRootPart.CanCollide = false
												TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
											until _G.AutoDoughtBoss == false or not v.Parent or v.Humanoid.Health <= 0
										end    
									end    
								else
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2187.23218, 70.0092163, -12395.624, 0.096041739, 1.03172715e-08, -0.995377302, -7.85410847e-09, 1, 9.60736113e-09, 0.995377302, 6.89509339e-09, 0.096041739)
								end
							else
								if game.Workspace.Enemies:FindFirstChild("Baking Staff [Lv. 2250]") or game.Workspace.Enemies:FindFirstChild("Head Baker [Lv. 2275]") or game.Workspace.Enemies:FindFirstChild("Cake Guard [Lv. 2225]") or game.Workspace.Enemies:FindFirstChild("Cookie Crafter [Lv. 2200]") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do  
										if (v.Name == "Baking Staff [Lv. 2250]" or v.Name == "Head Baker [Lv. 2275]" or v.Name == "Cake Guard [Lv. 2225]" or v.Name == "Cookie Crafter [Lv. 2200]") and v.Humanoid.Health > 0 then
											repeat task.wait()
												AutoHaki()
												EquipWeapon(_G.SelectWeapon)
												StartCakeMagnet = true
												v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)  
                                                v.Humanoid:ChangeState(11)
												POSCAKE = v.HumanoidRootPart.CFrame
												TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
											until _G.AutoDoughtBoss == false or game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") or not v.Parent or v.Humanoid.Health <= 0
										end
									end
								else
									StartCakeMagnet = false
									TP(CFrame.new(-1820.0634765625, 210.74781799316406, -12297.49609375))
								end
							end
						end)
					end
				end
			end)
		
		Main:Toggle("Auto Spawn Cake Prince",false,function(value)
			Auto_Spawn_Cake_Prince = value
		end)
		
			spawn(function()
				while wait() do
					if Auto_Spawn_Cake_Prince then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner",true)                    
					end
				end
			end)
		end
	
		if World3 then
		Main:Seperator("Elite")
		
		local EliteProgress = Main:Label("")
		
		spawn(function()
			pcall(function()
				while wait() do
					EliteProgress:Set("Elite Progress : "..game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter","Progress"))
				end
			end)
		end)
	
		Main:Toggle("Auto Elite Hunter",_G.AutoEliteHunter,function(a)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoEliteHunter = a
			StopTween(_G.AutoEliteHunter)
		end
		end)
		
		Main:Toggle("Auto Elite Hunter Hop",_G.AutoEliteHunterHOP,function(a)
			_G.AutoEliteHunterHOP = a
		end)
		
		spawn(function()
			while wait() do
				if _G.AutoEliteHunter then
					if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then
						if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Diablo") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Urban") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Deandre") then
							for i,v in pairs(game.ReplicatedStorage:GetChildren()) do
								if string.find(v.Name,"Diablo") then
									EliteHunter = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
									if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
										if EliteHunter then
											EliteHunter:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
									end
								end
								if string.find(v.Name,"Urban") then
									EliteHunter = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
									if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
										if EliteHunter then
											EliteHunter:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
									end
								end	
								if string.find(v.Name,"Deandre") then
									EliteHunter = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
									if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
										if EliteHunter then
											EliteHunter:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
									end
								end	
							end
							for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
								if _G.AutoEliteHunter and string.find(v.Name,"Diablo") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
									repeat wait()
										if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
											Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
										elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
											if Farmtween then
												Farmtween:Stop()
											end
											EquipWeapon(_G.SelectWeapon)
                                            v.Humanoid:ChangeState(11)
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,30,0)
											game:GetService'VirtualUser':CaptureController()
											game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										end
									until not _G.AutoEliteHunter or not v.Parent or v.Humanoid.Health <= 0
								end
								if _G.AutoEliteHunter and string.find(v.Name,"Urban") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
									repeat wait()
										if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
											Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
										elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
											if Farmtween then
												Farmtween:Stop()
											end
											EquipWeapon(_G.SelectWeapon)
                                            v.Humanoid:ChangeState(11)
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,30,0)
											game:GetService'VirtualUser':CaptureController()
											game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										end 
									until not _G.AutoEliteHunter or not v.Parent or v.Humanoid.Health <= 0
								end
								if _G.AutoEliteHunter and string.find(v.Name,"Deandre") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
									repeat wait()
										if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
											Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
										elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
											if Farmtween then
												Farmtween:Stop()
											end
											EquipWeapon(_G.SelectWeapon)
                                            v.Humanoid:ChangeState(11)
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,30,0)
											game:GetService'VirtualUser':CaptureController()
											game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										end 
									until not _G.AutoEliteHunter or not v.Parent or v.Humanoid.Health <= 0
								end
							end
						else
							if _G.AutoEliteHunterHOP and game:GetService("ReplicatedStorage").Remotes["CommF_"]:InvokeServer("EliteHunter") == "I don't have anything for you right now. Come back later." then
								Hop()
							else
								local string_1 = "EliteHunter";
								local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
								Target:InvokeServer(string_1);
							end
						end
					else
						if _G.AutoEliteHunterHOP and game:GetService("ReplicatedStorage").Remotes["CommF_"]:InvokeServer("EliteHunter") == "I don't have anything for you right now. Come back later." then
							Hop()
						else
							local string_1 = "EliteHunter";
							local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
							Target:InvokeServer(string_1);
						end
					end
				end
			end	
		end)
		end
		
		if World2 then
			Main:Seperator("Acidum Rifle")
	
			Main:Toggle("Auto Acidum Rifle",_G.Auto_Acidum_Rifle,function(vu)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
				_G.Auto_Acidum_Rifle = vu
			end
			end)
			
			spawn(function()
				while wait() do
					pcall(function()
						if _G.Auto_Acidum_Rifle then
								if game.Workspace.Enemies:FindFirstChild("Core") or game.ReplicatedStorage:FindFirstChild("Core") then
									if game.Workspace.Enemies:FindFirstChild("Core") then
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
										for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
											if v.Name == "Core" then
												repeat task.wait()
													EquipWeapon(_G.SelectWeapon)
													TP(CFrame.new(402.404296875, 182.53373718262, -414.73394775391))
												until not game.Workspace.Enemies:FindFirstChild("Core") or not _G.Auto_Acidum_Rifle
											end
										end
									end
								end
							end
						end)
					end
				end)
	
			Main:Toggle("Auto Acidum Rifle Hop",_G.Auto_Acidum_Rifle_Hop,function(value)
				_G.Auto_Acidum_Rifle_Hop = value
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if (_G.Auto_Acidum_Rifle_Hop) and World2 and not game:GetService("ReplicatedStorage"):FindFirstChild("Core") and not game:GetService("Workspace").Enemies:FindFirstChild("Core") then
							Hop()
						end
					end
				end)
			end)
		end
	
			if World2 then
				Main:Seperator("Black Spikey Coat")
		
					Main:Toggle("Auto Black Spikey Coat",_G.BlackSpikeyCoat,function(value)
						if _G.SelectWeapon == nil then
							local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
							local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
							wait(1)
							Notification:Notify(
								{Title = "Pado Hub", Description = "Select Weapon"},
								{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
							)
						else
					_G.BlackSpikeyCoat = value
					StopTween(_G.BlackSpikeyCoat)
					end
				end)					
				
				spawn(function()
					while wait() do
						if _G.BlackSpikeyCoat then
							pcall(function()
								if game:GetService("Workspace").Enemies:FindFirstChild("Jeremy [Lv. 850] [Boss]") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v.Name == "Jeremy [Lv. 850] [Boss]" then
											if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
												repeat task.wait()
													AutoHaki()
													EquipWeapon(_G.SelectWeapon)
													v.HumanoidRootPart.CanCollide = false
													v.Humanoid.JumpPower = 0
													v.Humanoid.WalkSpeed = 0
													v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                                    v.Humanoid:ChangeState(11)
													TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
													game:GetService("VirtualUser"):CaptureController()
													game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
													sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
												until not _G.BlackSpikeyCoat or not v.Parent or v.Humanoid.Health <= 0
											end
										end
									end
								else
									if game:GetService("ReplicatedStorage"):FindFirstChild("Jeremy [Lv. 850] [Boss]") then
										TP(game:GetService("ReplicatedStorage"):FindFirstChild("Jeremy [Lv. 850] [Boss]").HumanoidRootPart.CFrame * CFrame.new(5,10,7))
									end
								end
							end)
						end
					end
				end)
				
				Main:Toggle("Auto Black Spikey Coat Hop",_G.AutoBlackSpikeyCoat_Hop,function(value)
					_G.AutoBlackSpikeyCoat_Hop = value
				end)
				
				spawn(function()
					pcall(function()
						while wait() do
							if (_G.AutoBlackSpikeyCoat_Hop) and World2 and not game:GetService("ReplicatedStorage"):FindFirstChild("Jeremy [Lv. 850] [Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Jeremy [Lv. 850] [Boss]") then
								Hop()
							end
						end
					end)
				end)
				end
		
		if World2 then
		Main:Seperator("Dark Coat")	
		
		Main:Toggle("Auto Dark Coat",_G.BlackBeard,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.BlackBeard = value
			StopTween(_G.BlackBeard)
		end
		end)
		
		Main:Toggle("Auto Dark Coat Hop",_G.BlackBeardHop,function(value)
			_G.BlackBeardHop = value
		end)
		
		spawn(function()
			while wait() do
				if _G.BlackBeard then
					pcall(function()
						if game:GetService("Workspace").Enemies:FindFirstChild("Darkbeard [Lv. 1000] [Raid Boss]") then
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if string.find(v.Name , "Fist of Darkness") then
									repeat task.wait()
										EquipWeapon(_G.SelectWeapon)
										AutoHaki()
										v.HumanoidRootPart.CanCollide = false
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                        v.Humanoid:ChangeState(11)
										TP(v.HumanoidRootPart.CFrame * Farm_Mode)
										game:GetService("VirtualUser"):CaptureController()
										game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670))
										sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
									until v.Humanoid.Health <= 0 or _G.BlackBeard == false
								end
							end
						elseif game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Fist of Darkness") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Fist of Darkness") then
							repeat TP(CFrame.new(3777.564697265625, 14.876824378967285, -3499.460205078125)) wait() until (CFrame.new(3777.564697265625, 14.876824378967285, -3499.460205078125).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 8                        
						end
					end)
				end
			end
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if (_G.BlackBeardHop) and World2 and not game:GetService("ReplicatedStorage"):FindFirstChild("Darkbeard [Lv. 1000] [Raid Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Darkbeard [Lv. 1000] [Raid Boss]") then
						Hop()
					end
				end
			end)
		end)
		end
	
		if World2 then
		Main:Seperator("Swan Glasses")
		
		Main:Toggle("Auto Swan Glasses",_G.AutoFarmSwanGlasses,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoFarmSwanGlasses = value
			StopTween(_G.AutoFarmSwanGlasses)
		end
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if _G.AutoFarmSwanGlasses then
						if game:GetService("Workspace").Enemies:FindFirstChild("Don Swan [Lv. 1000] [Boss]") then
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v.Name == "Don Swan [Lv. 1000] [Boss]" and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
									repeat task.wait()
										pcall(function()
											AutoHaki()
											EquipWeapon(_G.SelectWeapon)
											v.HumanoidRootPart.CanCollide = false
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                            v.Humanoid:ChangeState(11)
											TP(v.HumanoidRootPart.CFrame * Farm_Mode)
											game:GetService("VirtualUser"):CaptureController()
											game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670))
											sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
										end)
									until _G.AutoFarmSwanGlasses == false or v.Humanoid.Health <= 0
								end
							end
							  else 
								repeat task.wait()
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(2284.912109375, 15.537666320801, 905.48291015625)) 
							until (CFrame.new(2284.912109375, 15.537666320801, 905.48291015625).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 or _G.AutoFarmSwanGlasses == false
						end
					end
				end
			end)
		end)
		
		Main:Toggle("Auto Swan Glasses Hop",_G.AutoFarmSwanGlasses_Hop,function(value)
			_G.AutoFarmSwanGlasses_Hop = value
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if (_G.AutoFarmSwanGlasses_Hop) and World2 and not game:GetService("ReplicatedStorage"):FindFirstChild("Don Swan [Lv. 1000] [Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Don Swan [Lv. 1000] [Boss]") then
						Hop()
					end
				end
			end)
		end)
		end
		
		if World3 then
		Main:Seperator("Cursed Dual Katana")
			
		 Main:Button("Tushita Quest : 1",function()
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("LoadItem","Tushita")
			wait(1)
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CDKQuest","StartTrial","Good")
			Tushita_Quest1 = true
			TP(CFrame.new(-6127.5712890625, 16.446542739868164, -2247.595703125))
			wait(60)
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CDKQuest","BoatQuest", workspace.NPCs:FindFirstChild("Luxury Boat Dealer"))
			wait(1)
			TP(CFrame.new(-127.23313903808594, 6.755744934082031, 5259.51025390625))    
		   wait(60)
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CDKQuest","BoatQuest", workspace.NPCs:FindFirstChild("Luxury Boat Dealer"))
		   wait(1)
		   TP(CFrame.new(-2067.349365234375, 4.701088905334473, -9890.4501953125))
			wait(60)
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CDKQuest","BoatQuest", workspace.NPCs:FindFirstChild("Luxury Boat Dealer"))
			Tushita_Quest1 = false
		 end)
	
		   Main:Toggle("Tushita Quest : 2", Tushita_Quest2, function(value)
				Tushita_Quest2 = value
				StopTween(Tushita_Quest2)
			end)
	
				spawn(function()
					while wait() do
						pcall(function()
							if Tushita_Quest2 then
								TP(CFrame.new(-5473.24072, 369.774017, -2790.04517, 0.93348068, 2.05335038e-08, 0.358627766, -5.78810706e-08, 1, 9.3404239e-08, -0.358627766, -1.07948807e-07, 0.93348068))
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("LoadItem","Tushita")
								wait(1)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CDKQuest","StartTrial","Good")
								wait(.5)
								if game:GetService("Workspace").Enemies:GetChildren() then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if Tushita_Quest2 and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 1000 then
											repeat wait()
												StartMagnet = true
												EquipWeapon(_G.SelectWeapon)
												PosMon = v.HumanoidRootPart.CFrame
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
												v.HumanoidRootPart.Size = Vector3.new(60,60,60)
												v.Humanoid.JumpPower = 0
												v.Humanoid.WalkSpeed = 0
												v.HumanoidRootPart.CanCollide = false
												v.Humanoid:ChangeState(11)
												TP(v.HumanoidRootPart.CFrame * CFrame.new(0,20,0))
											until v.Humanoid.Health <= 0 or not Tushita_Quest2
											StartMagnet = false
										end
									end
								end
							end
						end)
					end
				end)
	
			Main:Toggle("Tushita Quest : 3", Tushita_Quest3, function(value)
				Tushita_Quest3 = value
				StopTween(Tushita_Quest3)
			end)
	
			spawn(function()
				while wait() do
					if Tushita_Quest3 then
						pcall(function()
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CDKQuest","Progress","Good")
							 if game:GetService("Workspace").Enemies:FindFirstChild("Cake Queen [Lv. 2175] [Boss]") then
								for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
									if v.Name == "Cake Queen [Lv. 2175] [Boss]" then
										if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											repeat task.wait()
												AutoHaki()
												EquipWeapon(_G.SelectWeapon)
												v.HumanoidRootPart.CanCollide = false
												v.Humanoid.JumpPower = 0
												v.Humanoid.WalkSpeed = 0
												v.HumanoidRootPart.Size = Vector3.new(55,55,55)
												TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
												game:GetService("VirtualUser"):CaptureController()
												game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
												sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
											until not Tushita_Quest3 or not v.Parent or v.Humanoid.Health <= 0
										end
									end
								end
							else
								if game:GetService("ReplicatedStorage"):FindFirstChild("Cake Queen [Lv. 2175] [Boss]") then
									TP(game:GetService("ReplicatedStorage"):FindFirstChild("Cake Queen [Lv. 2175] [Boss]").HumanoidRootPart.CFrame * Farm_Mode)
								end
							end
						end)
					end
				end
			end)
	
			Main:Toggle("Yama Quest : 2", Auto_Quest_Yama_2, function(value)
				Auto_Quest_Yama_2 = value
				StopTween(Auto_Quest_Yama_2)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CDKQuest","StartTrial","Evil")
			end)
	
			spawn(function()
				while wait() do
					pcall(function()
						if Auto_Quest_Yama_2 then
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v:FindFirstChild("HazeESP") then
									v.HazeESP.Size = UDim2.new(50,50,50,50)
									v.HazeESP.MaxDistance = "inf"
								end
							end
							for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
								if v:FindFirstChild("HazeESP") then
									v.HazeESP.Size = UDim2.new(50,50,50,50)
									v.HazeESP.MaxDistance = "inf"
								end
							end
						end
					end)
				end
			end)
		
			spawn(function()
				while wait() do
					pcall(function()
						for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if Auto_Quest_Yama_2 and v:FindFirstChild("HazeESP") and (v.HumanoidRootPart.Position - PosMonsEsp.Position).magnitude <= 300 then
								v.HumanoidRootPart.CFrame = PosMonsEsp
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(50,50,50)
								if not v.HumanoidRootPart:FindFirstChild("BodyVelocity") then
									local vc = Instance.new("BodyVelocity", v.HumanoidRootPart)
									vc.MaxForce = Vector3.new(1, 1, 1) * math.huge
									vc.Velocity = Vector3.new(0, 0, 0)
								end
							end
						end
					end)
				end
			end)
		
			spawn(function()
				while wait() do
					if Auto_Quest_Yama_2 then 
						pcall(function() 
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v:FindFirstChild("HazeESP") then
									repeat wait()
										if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 2000 then
											TP(y.HumanoidRootPart.CFrameMon * CFrame.new(0,20,0))
										else
											StartMagnet = true
											EquipWeapon(_G.SelectWeapon)
											PosMonsEsp = v.HumanoidRootPart.CFrame
											v.HumanoidRootPart.Size = Vector3.new(60,60,60)
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.CanCollide = false
											v.Humanoid:ChangeState(11)
											TP(v.HumanoidRootPart.CFrame * CFrame.new(0,20,0))		
											game:GetService("VirtualUser"):CaptureController()
											game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
										end      
									until Auto_Quest_Yama_2 == false or not v.Parent or v.Humanoid.Health <= 0 or not v:FindFirstChild("HazeESP")
								else
									for x,y in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
										if y:FindFirstChild("HazeESP") then
											if (y.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 2000 then
												TP(y.HumanoidRootPart.CFrameMon * CFrame.new(0,20,0))
											else
												TP(y.HumanoidRootPart.CFrame * CFrame.new(0,20,0))
											end
										end
									end
								end
							end
						end)
					end
				end
			end)
	
			Main:Toggle("Yama Quest : 3", Auto_Quest_Yama_3, function(value)
				Auto_Quest_Yama_3 = value
				StopTween(Auto_Quest_Yama_3)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CDKQuest","Progress","Evil")
			end)
	
			spawn(function()
				while wait() do
					if Auto_Quest_Yama_3 then
						pcall(function()
							if game.Players.LocalPlayer.Backpack:FindFirstChild("Hallow Essence") then         
								_G.Auto_Bone = false           
								TP(game:GetService("Workspace").Map["Haunted Castle"].Summoner.Detection.CFrame)
							elseif game:GetService("Workspace").Map:FindFirstChild("HellDimension") then
								repeat wait()
									if game:GetService("Workspace").Enemies:FindFirstChild("Cursed Skeleton [Lv. 2200]") or game:GetService("Workspace").Enemies:FindFirstChild("Cursed Skeleton [Lv. 2200] [Boss]") or game:GetService("Workspace").Enemies:FindFirstChild("Hell's Messenger [Lv. 2200] [Boss]") then
										for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
											if v.Name == "Cursed Skeleton [Lv. 2200]" or v.Name == "Cursed Skeleton [Lv. 2200] [Boss]" or v.Name == "Hell's Messenger [Lv. 2200] [Boss]" then
												if v.Humanoid.Health > 0 then
													repeat wait()
														StartMagnet = true
														EquipWeapon(_G.SelectWeapon)
														PosMonsEsp = v.HumanoidRootPart.CFrame
														game:GetService'VirtualUser':CaptureController()
														game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
														v.HumanoidRootPart.Size = Vector3.new(60,60,60)
														v.Humanoid.JumpPower = 0
														v.Humanoid.WalkSpeed = 0
														v.HumanoidRootPart.CanCollide = false
														v.Humanoid:ChangeState(11)
														TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
													until v.Humanoid.Health <= 0 or not v.Parent or Auto_Quest_Yama_3 == false
												end
											end
										end
									else
										wait(5)
										TP(game:GetService("Workspace").Map.HellDimension.Torch1.CFrame)
										wait(1.5)
										game:GetService("VirtualInputManager"):SendKeyEvent(true, "E", false, game)
										wait(1.5)        
										TP(game:GetService("Workspace").Map.HellDimension.Torch2.CFrame)
										wait(1.5)
										game:GetService("VirtualInputManager"):SendKeyEvent(true, "E", false, game)
										wait(1.5)     
										TP(game:GetService("Workspace").Map.HellDimension.Torch3.CFrame)
										wait(1.5)
										game:GetService("VirtualInputManager"):SendKeyEvent(true, "E", false, game)
										wait(1.5)     
										TP(game:GetService("Workspace").Map.HellDimension.Exit.CFrame)
									end
								until Auto_Quest_Yama_3 == false or GetMaterial("Alucard Fragment") == 3
							else
								if game:GetService("Workspace").Enemies:FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]") or game.ReplicatedStorage:FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]") then
									if game:GetService("Workspace").Enemies:FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]") then
										for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
											if v.Name == "Soul Reaper [Lv. 2100] [Raid Boss]" then
												if v.Humanoid.Health > 0 then
													repeat wait()
														TP(v.HumanoidRootPart.CFrame * CFrame.new(0,0,-2))
													until Auto_Quest_Yama_3 == false or game:GetService("Workspace").Map:FindFirstChild("HellDimension")
												end
											end
										end
									else
										TP(CFrame.new(-9570.033203125, 315.9346923828125, 6726.89306640625))
									end
								else
									_G.Auto_Bone = true
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Bones","Buy",1,1)
								end
							end		
						end)
					end
				end
			end)
		end
	
		if World3 then
		Main:Seperator("Bone")
	
		local Bone = Main:Label("")
		
		spawn(function()
			pcall(function()
				while wait() do
					Bone:Set("Your Bone : "..(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Bones","Check")))
				end
			end)
		end)
	
		Main:Toggle("Auto Farm Bone",_G.Auto_Bone,function(value)
			_G.Auto_Bone = value
			StopTween(_G.Auto_Bone)
		end)
		
		spawn(function()
			while wait() do 
				if _G.Auto_Bone then
					pcall(function()
						if game:GetService("Workspace").Enemies:FindFirstChild("Reborn Skeleton [Lv. 1975]") or game:GetService("Workspace").Enemies:FindFirstChild("Living Zombie [Lv. 2000]") or game:GetService("Workspace").Enemies:FindFirstChild("Demonic Soul [Lv. 2025]") or game:GetService("Workspace").Enemies:FindFirstChild("Posessed Mummy [Lv. 2050]") then
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v.Name == "Reborn Skeleton [Lv. 1975]" or v.Name == "Living Zombie [Lv. 2000]" or v.Name == "Demonic Soul [Lv. 2025]" or v.Name == "Posessed Mummy [Lv. 2050]" then
									if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										repeat task.wait()
											AutoHaki()
											EquipWeapon(_G.SelectWeapon)
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
                                            v.Humanoid:ChangeState(11)
											v.Head.CanCollide = false 
											StartMagnetBoneMon = true
											PosMonBone = v.HumanoidRootPart.CFrame
											TP(v.HumanoidRootPart.CFrame * Farm_Mode)
										until not _G.Auto_Bone or not v.Parent or v.Humanoid.Health <= 0
									end
								end
							end
						else
							StartMagnetBoneMon = false
							TP(CFrame.new(-9515.751953125, 144.33457946777344, 5787.08935546875))
							for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do 
								if v.Name == "Reborn Skeleton [Lv. 1975]" then
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)                
							elseif v.Name == "Living Zombie [Lv. 2000]" then
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)
							elseif v.Name == "Demonic Soul [Lv. 2025]" then
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)
							elseif v.Name == "Posessed Mummy [Lv. 2050]" then
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)
							end
						end
					end
				end)
			end
		end
	end)
		
		Main:Toggle("Auto Random Surprise",_G.Auto_Random_Bone,function(value)
			_G.Auto_Random_Bone = value
		end)
		
		spawn(function()
			pcall(function()
				while wait(.1) do
					if _G.Auto_Random_Bone then    
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Bones","Buy",1,1)
					end
				end
			end)
		end)
	end
		
		Main:Seperator("Observation")
	
		local ObservationVirtualUser = game:GetService('VirtualUser')
		Main:Toggle("Auto Farm Observation",false ,function(a)
			Observation = a
			StopTween(Observation)
			if Observation and not game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
				ObservationVirtualUser:CaptureController()
				ObservationVirtualUser:SetKeyDown('0x65')
				wait(2)
				ObservationVirtualUser:SetKeyUp('0x65')
			end
		end)
	
		spawn(function()
			while wait() do
				if Observation then
					if game:GetService("Players").LocalPlayer.VisionRadius.Value >= 3000 then
						local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
						local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
						wait(1)
						Notification:Notify(
							{Title = "Pado Hub", Description = ("You Have Max Observation")},
							{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
						)
				else
					if World3 then
						if game.Workspace.Enemies:FindFirstChild("Dragon Crew Warrior [Lv. 1575]") then
							if game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
								repeat wait()
									if (game.Workspace.Enemies:FindFirstChild("Dragon Crew Warrior [Lv. 1575]").HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
										Farmtween = TP2(game.Workspace.Enemies:FindFirstChild("Dragon Crew Warrior [Lv. 1575]").HumanoidRootPart.Position,game.Workspace.Enemies:FindFirstChild("Dragon Crew Warrior [Lv. 1575]").HumanoidRootPart.CFrame)
									elseif (game.Workspace.Enemies:FindFirstChild("Dragon Crew Warrior [Lv. 1575]").HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
										if Farmtween then
											Farmtween:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Dragon Crew Warrior [Lv. 1575]").HumanoidRootPart.CFrame * CFrame.new(3,0,0)
									end
								until Observation == false or not game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
							else
								repeat wait()
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Dragon Crew Warrior [Lv. 1575]").HumanoidRootPart.CFrame * CFrame.new(10,15,0)
									if not game:GetService("Players").LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") and _G.AutoObservation_Hop == true then
										game:GetService("TeleportService"):Teleport(game.PlaceId,game:GetService("Players").LocalPlayer)
									end
								until Observation == false or game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
							end
						else
							Modstween = TP2(CFrame.new(4530.3540039063, 656.75695800781, -131.60952758789).Position, CFrame.new(4530.3540039063, 656.75695800781, -131.60952758789))
							if game.Workspace.Enemies:FindFirstChild("Water Fighter [Lv. 1450]") and (CFrame.new(4530.3540039063, 656.75695800781, -131.60952758789).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
								if Modstween then
									Modstween:Stop()
								end
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(4530.3540039063, 656.75695800781, -131.60952758789)
							end 
						end
					elseif World2 then
						if game.Workspace.Enemies:FindFirstChild("Water Fighter [Lv. 1450]") then
							if game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
								repeat wait()
									if (game.Workspace.Enemies:FindFirstChild("Water Fighter [Lv. 1450]").HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
										Farmtween = TP2(game.Workspace.Enemies:FindFirstChild("Water Fighter [Lv. 1450]").HumanoidRootPart.Position,game.Workspace.Enemies:FindFirstChild("Water Fighter [Lv. 1450]").HumanoidRootPart.CFrame)
									elseif (game.Workspace.Enemies:FindFirstChild("Water Fighter [Lv. 1450]").HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
										if Farmtween then
											Farmtween:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Water Fighter [Lv. 1450]").HumanoidRootPart.CFrame * CFrame.new(3,0,0)
									end
								until Observation == false or not game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
							else
								repeat wait()
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Water Fighter [Lv. 1450]").HumanoidRootPart.CFrame * CFrame.new(10,15,0)
									if not game:GetService("Players").LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") and _G.AutoObservation_Hop == true then
										game:GetService("TeleportService"):Teleport(game.PlaceId,game:GetService("Players").LocalPlayer)
									end
								until Observation == false or game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
							end
						else
							Modstween = TP2(CFrame.new(-3305.61279, 252.562607, -10497.5693, -0.694175005, -2.20830731e-08, 0.719806314, -2.05950599e-08, 1, 1.08174909e-08, -0.719806314, -7.31522265e-09, -0.694175005).Position, CFrame.new(-3305.61279, 252.562607, -10497.5693, -0.694175005, -2.20830731e-08, 0.719806314, -2.05950599e-08, 1, 1.08174909e-08, -0.719806314, -7.31522265e-09, -0.694175005))
							if game.Workspace.Enemies:FindFirstChild("Water Fighter [Lv. 1450]") and (CFrame.new(-3305.61279, 252.562607, -10497.5693, -0.694175005, -2.20830731e-08, 0.719806314, -2.05950599e-08, 1, 1.08174909e-08, -0.719806314, -7.31522265e-09, -0.694175005).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
								if Modstween then
									Modstween:Stop()
								end
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-3305.61279, 252.562607, -10497.5693, -0.694175005, -2.20830731e-08, 0.719806314, -2.05950599e-08, 1, 1.08174909e-08, -0.719806314, -7.31522265e-09, -0.694175005)
							end 
						end
					elseif World1 then
						if game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]") then
							if game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
								repeat wait()
									if (game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]").HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
										Farmtween = TP2(game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]").HumanoidRootPart.Position,game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]").HumanoidRootPart.CFrame)
									elseif (game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]").HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
										if Farmtween then
											Farmtween:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]").HumanoidRootPart.CFrame * CFrame.new(3,0,0)
									end
								until Observation == false or not game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
							else
								repeat wait()
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Enemies:FindFirstChild("Galley Captain [Lv. 650]").HumanoidRootPart.CFrame * CFrame.new(10,15,0)
									if not game:GetService("Players").LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") and _G.AutoObservation_Hop == true then
										game:GetService("TeleportService"):Teleport(game.PlaceId,game:GetService("Players").LocalPlayer)
									end
								until Observation == false or game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel")
							end
						else
							Modstween = TP2(CFrame.new(5533.29785, 88.1079102, 4852.3916).Position, CFrame.new(5533.29785, 88.1079102, 4852.3916))
							if game.Workspace.Enemies:FindFirstChild("Ship Engineer [Lv. 1275]") and (CFrame.new(5533.29785, 88.1079102, 4852.3916).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
								if Modstween then
									Modstween:Stop()
								end
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5533.29785, 88.1079102, 4852.3916)
							end
							end 
						end
					end
				end
			end
		end)
	
		spawn(function()
			while wait() do
				pcall(function()
					if Observation and not game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
						ObservationVirtualUser:CaptureController()
						ObservationVirtualUser:SetKeyDown('0x65')
						wait(2)
						ObservationVirtualUser:SetKeyUp('0x65')
					end
				end)
			end
		end)	
		
		Main:Toggle("Auto Farm Observation Hop",_G.AutoObservation_Hop,function(value)
			_G.AutoObservation_Hop = value
		end)
		
		if World2 then
		Main:Seperator("Legendary Sword")
	
		Main:Toggle("Auto Legendary Sword Buy",_G.AutoBuyLegendarySword,function(value)
			_G.AutoBuyLegendarySword = value
		end)
		
		spawn(function()
			while wait() do
				if _G.AutoBuyLegendarySword then
					pcall(function()
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("LegendarySwordDealer","1")
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("LegendarySwordDealer","2")
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("LegendarySwordDealer","3")
						if _G.AutoBuyLegendarySword_Hop and _G.AutoBuyLegendarySword and World2 then
							wait(10)
							Hop()
						end
					end)
				end 
			end
		end)
		
		Main:Toggle("Auto Legendary Sword Hop",_G.AutoBuyLegendarySword_Hop,function(value)
			_G.AutoBuyLegendarySword_Hop = value
		end)
		end
		
		if World2 or World3 then
		Main:Seperator("Enchancement Colour")
	
		Main:Toggle("Auto Enchancement Colour Buy",_G.AutoBuyEnchancementColour,function(value)
			_G.AutoBuyEnchancementColour = value
		end)
		
		Main:Toggle("Auto Enchancement Hop",_G.AutoBuyEnchancementColour_Hop,function(value)
			_G.AutoBuyEnchancementColour_Hop = value
		end)
		
		spawn(function()
			while wait() do
				if _G.AutoBuyEnchancementColour then
					local args = {
						[1] = "ColorsDealer",
						[2] = "2"
					}
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
					if _G.AutoBuyEnchancementColour_Hop and _G.AutoBuyEnchancementColour and not World1 then
						wait(10)
						Hop()
					end
				end 
			end
		end)
	end
		
	if World3 then
		Main:Seperator("Spikey Trident")
		
		Main:Toggle("Auto Spikey Trident",_G.Auto_Spikey_Trident,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.Auto_Spikey_Trident = value
			StopTween(_G.Auto_Spikey_Trident)
		end
	end)
		
	Main:Toggle("Auto Spikey Trident Hop",_G.Auto_Spikey_Trident_Hop,function(value)
					_G.Auto_Spikey_Trident_Hop = value
					StopTween(_G.Auto_Spikey_Trident_Hop)
				end)

			spawn(function()
				while wait(.1) do
					if _G.Auto_Spikey_Trident then
						pcall(function()
							if game.ReplicatedStorage:FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") or game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") then   
								if game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do 
										if v.Name == "Cake Prince [Lv. 2300] [Raid Boss]" then
											repeat task.wait()
												AutoHaki()
												EquipWeapon(_G.SelectWeapon)
												v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                                                v.Humanoid:ChangeState(11)
												v.HumanoidRootPart.CanCollide = false
												TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
											until _G.Auto_Spikey_Trident == false or not v.Parent or v.Humanoid.Health <= 0
										end    
									end    
								else
									game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2187.23218, 70.0092163, -12395.624, 0.096041739, 1.03172715e-08, -0.995377302, -7.85410847e-09, 1, 9.60736113e-09, 0.995377302, 6.89509339e-09, 0.096041739)
								end
							else
								if game.Workspace.Enemies:FindFirstChild("Baking Staff [Lv. 2250]") or game.Workspace.Enemies:FindFirstChild("Head Baker [Lv. 2275]") or game.Workspace.Enemies:FindFirstChild("Cake Guard [Lv. 2225]") or game.Workspace.Enemies:FindFirstChild("Cookie Crafter [Lv. 2200]") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do  
										if (v.Name == "Baking Staff [Lv. 2250]" or v.Name == "Head Baker [Lv. 2275]" or v.Name == "Cake Guard [Lv. 2225]" or v.Name == "Cookie Crafter [Lv. 2200]") and v.Humanoid.Health > 0 then
											repeat task.wait()
												AutoHaki()
												EquipWeapon(_G.SelectWeapon)
												StartCakeMagnet = true
												v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)  
                                                v.Humanoid:ChangeState(11)
												POSCAKE = v.HumanoidRootPart.CFrame
												TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
											until _G.Auto_Spikey_Trident == false or game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") or not v.Parent or v.Humanoid.Health <= 0
										end
									end
								else
									StartCakeMagnet = false
									TP(CFrame.new(-1820.0634765625, 210.74781799316406, -12297.49609375))
								end
							end
						end)
					end
				end
			end)

		spawn(function()
			pcall(function()
				while wait() do
					if (_G.Auto_Spikey_Trident_Hop) and World3 and not game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") then
						Hop()
					end
				end
			end)
		end)
		end

	if World3 then
		Main:Seperator("Twin Hook")
	
		Main:Toggle("Auto Twin Hook",_G.Auto_Twin_Hook,function(value)
		if _G.SelectWeapon == nil then
			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
			wait(1)
			Notification:Notify(
				{Title = "Pado Hub", Description = "Select Weapon"},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
			)
		else
				_G.Auto_Twin_Hook = value
				StopTween(_G.Auto_Twin_Hook)
	end
	end)
	
	Main:Toggle("Auto Twin Hook Hop",_G.AutoTwinHook_Hop,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
				_G.AutoTwinHook_Hop = value
				StopTween(_G.AutoTwinHook_Hop)
			end
			end)
	
		spawn(function()
			while wait() do
				if _G.Auto_Twin_Hook then
					pcall(function()
						if _G.Auto_Twin_Hook and game.ReplicatedStorage:FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") or game.Workspace.Enemies:FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") then
							if game.Workspace.Enemies:FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") then
								for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
									if v.Name == "Captain Elephant [Lv. 1875] [Boss]" and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
										repeat task.wait()
											AutoHaki()
											EquipWeapon(_G.SelectWeapon)
											v.HumanoidRootPart.CanCollide = false
											v.HumanoidRootPart.Size = Vector3.new(50,50,50)
											TP(v.HumanoidRootPart.CFrame * Farm_Mode)
											game:GetService'VirtualUser':CaptureController()
											game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										until _G.Auto_Twin_Hook or v.Humanoid.Health <= 0 or not v.Parent
									end
								end
							else
								TP(CFrame.new(-13348.0654296875, 405.8904113769531, -8570.62890625))
							end
						end
					end)
				end
			end
		end)
	
	spawn(function()
		pcall(function()
			while wait() do
				if (_G.AutoTwinHook_Hop) and World3 and not game:GetService("ReplicatedStorage"):FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") then
					Hop()
				end
			end
		end)
	end)
	end

	if World3 then
		Main:Seperator("Hallow Scythe")
	
		Main:Toggle("Auto Soul Reaper",_G.AutoFarmBossHallow,function(value)
		if _G.SelectWeapon == nil then
			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
			wait(1)
			Notification:Notify(
				{Title = "Pado Hub", Description = "Select Weapon"},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
			)
		else
		_G.AutoFarmBossHallow = value
		StopTween(_G.AutoFarmBossHallow)
	end
	end)
	
	Main:Toggle("Auto Soul Reaper Hop",_G.AutoFarmBossHallowHop,function(value)
		_G.AutoFarmBossHallowHop = value
	end)
	
	spawn(function()
		while wait() do
			if _G.AutoFarmBossHallow then
				pcall(function()
					if game:GetService("Workspace").Enemies:FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]") then
						for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if string.find(v.Name , "Soul Reaper") then
								repeat task.wait()
									EquipWeapon(_G.SelectWeapon)
									AutoHaki()
									v.HumanoidRootPart.CanCollide = false
									v.HumanoidRootPart.Size = Vector3.new(50,50,50)
									TP(v.HumanoidRootPart.CFrame * Farm_Mode)
									game:GetService("VirtualUser"):CaptureController()
									game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670))
									sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
								until v.Humanoid.Health <= 0 or _G.AutoFarmBossHallow == false
							end
						end
					elseif game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Hallow Essence") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Hallow Essence") then
						repeat TP(CFrame.new(-8932.322265625, 146.83154296875, 6062.55078125)) wait() until (CFrame.new(-8932.322265625, 146.83154296875, 6062.55078125).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 8                        
					else
						if game:GetService("ReplicatedStorage"):FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]") then
							TP(game:GetService("ReplicatedStorage"):FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]").HumanoidRootPart.CFrame * CFrame.new(5,10,7))
						end
					end
				end)
			end
		end
	end)
	
	spawn(function()
		pcall(function()
			while wait() do
				if (_G.AutoFarmBossHallowHop) and World3 and not game:GetService("ReplicatedStorage"):FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]") then
					Hop()
				end
			end
		end)
	end)
	end
	
	if World3 then
		Main:Seperator("Dark Dagger")
	
		Main:Toggle("Auto Dark Dagger",_G.AutoDarkDagger,function(value)
		if _G.SelectWeapon == nil then
			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
			wait(1)
			Notification:Notify(
				{Title = "Pado Hub", Description = "Select Weapon"},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
			)
		else
		_G.AutoDarkDagger = value
		StopTween(_G.AutoDarkDagger)
	end
	end)

	spawn(function()
		while wait() do
			if _G.AutoDarkDagger then
				pcall(function()
					if game:GetService("Workspace").Enemies:FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") then
						for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if v.Name == "rip_indra True Form [Lv. 5000] [Raid Boss]" then
								if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
									repeat task.wait()
										AutoHaki()
										EquipWeapon(_G.SelectWeapon)
										v.HumanoidRootPart.CanCollide = false
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(50,50,50)
										TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
										game:GetService("VirtualUser"):CaptureController()
										game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
										sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
									until not _G.AutoDarkDagger or not v.Parent or v.Humanoid.Health <= 0
								end
							end
						end
					else
						if game:GetService("ReplicatedStorage"):FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") then
							TP(game:GetService("ReplicatedStorage"):FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]").HumanoidRootPart.CFrame * CFrame.new(5,10,7))
						end
					end
				end)
			end
		end
	end)
	
	Main:Toggle("Auto Dark Dagger Hop",_G.AutoDarkDagger_Hop,function(value)
		_G.AutoDarkDagger_Hop = value
	end)
	
	spawn(function()
		pcall(function()
			while wait() do
				if (_G.AutoDarkDagger_Hop) and World3 and not game:GetService("ReplicatedStorage"):FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") then
					Hop()
				end
			end
		end)
	end)
	end	

	if World3 then
		Main:Seperator("Serpent Bow")
		
		Main:Toggle("Auto Serpent Bow",false,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoSerpentBow = value
			StopTween(_G.AutoSerpentBow)
		end
		end)
	
		spawn(function()
			while wait() do
				if _G.AutoSerpentBow then
					pcall(function()
						if game:GetService("Workspace").Enemies:FindFirstChild("Island Empress [Lv. 1675] [Boss]") then
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v.Name == "Island Empress [Lv. 1675] [Boss]" then
									if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										repeat task.wait()
											AutoHaki()
											EquipWeapon(_G.SelectWeapon)
											v.HumanoidRootPart.CanCollide = false
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(60,60,60)
											TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
											game:GetService("VirtualUser"):CaptureController()
											game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
											sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
										until not _G.AutoSerpentBow or not v.Parent or v.Humanoid.Health <= 0
									end
								end
							end
						else
							if game:GetService("ReplicatedStorage"):FindFirstChild("Island Empress [Lv. 1675] [Boss]") then
								TP(game:GetService("ReplicatedStorage"):FindFirstChild("Island Empress [Lv. 1675] [Boss]").HumanoidRootPart.CFrame * Farm_Mode)
							end
						end
					end)
				end
			end
		end)
	
		Main:Toggle("Auto Serpent Bow Hop",_G.AutoSerpentBow_Hop,function(value)
			_G.AutoSerpentBow_Hop = value
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if (_G.AutoSerpentBow_Hop) and World3 and not game:GetService("ReplicatedStorage"):FindFirstChild("Island Empress [Lv. 1675] [Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Island Empress [Lv. 1675] [Boss]") then
						Hop()
					end
				end
			end)
		end)
	end
		
		if World3 then
			Main:Seperator("Buddy Sword")
		
			Main:Toggle("Auto Buddy Sword",_G.AutoBudySword,function(value)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoBudySword = value
			StopTween(_G.AutoBudySword)
		end
		end)
		
		Main:Toggle("Auto Buddy Sword Hop",_G.AutoBudySword_Hop,function(value)
			_G.AutoBudySword_Hop = value
		end)
		
		spawn(function()
			while wait() do
				if _G.AutoBudySword then
					pcall(function()
						if game:GetService("Workspace").Enemies:FindFirstChild("Cake Queen [Lv. 2175] [Boss]") then
							for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v.Name == "Cake Queen [Lv. 2175] [Boss]" then
									if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										repeat task.wait()
											AutoHaki()
											EquipWeapon(_G.SelectWeapon)
											v.HumanoidRootPart.CanCollide = false
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(55,55,55)
											TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
											game:GetService("VirtualUser"):CaptureController()
											game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
											sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
										until not _G.AutoBudySword or not v.Parent or v.Humanoid.Health <= 0
									end
								end
							end
						else
							if game:GetService("ReplicatedStorage"):FindFirstChild("Cake Queen [Lv. 2175] [Boss]") then
								TP(game:GetService("ReplicatedStorage"):FindFirstChild("Cake Queen [Lv. 2175] [Boss]").HumanoidRootPart.CFrame * Farm_Mode)
							end
						end
					end)
				end
			end
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if (_G.AutoBudySword_Hop) and World3 and not game:GetService("ReplicatedStorage"):FindFirstChild("Cake Queen [Lv. 2175] [Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Cake Queen [Lv. 2175] [Boss]") then
						Hop()
					end
				end
			end)
		end)
		end
		
		if World3 then
			Main:Seperator("Cavander")
			
			Main:Toggle("Auto Cavander",_G.AutoFarmCavander,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
				_G.AutoFarmCavander = value
				StopTween(_G.AutoFarmCavander)
			end
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.AutoFarmCavander then
							if game:GetService("Workspace").Enemies:FindFirstChild("Beautiful Pirate [Lv. 1950] [Boss]") then
								for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
									if v.Name == "Beautiful Pirate [Lv. 1950] [Boss]" and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
										repeat task.wait()
											pcall(function()
												AutoHaki()
												EquipWeapon(_G.SelectWeapon)
												v.HumanoidRootPart.CanCollide = false
												v.Humanoid.JumpPower = 0
												v.Humanoid.WalkSpeed = 0
												v.HumanoidRootPart.Size = Vector3.new(50,50,50)
												TP(v.HumanoidRootPart.CFrame * Farm_Mode)
												game:GetService("VirtualUser"):CaptureController()
												game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670))
												sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
											end)
										until _G.AutoFarmCavander == false or v.Humanoid.Health <= 0
									end
								end
								  else 
								repeat task.wait()
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(5315.6318359375, 22.562606811523438, -131.0099334716797)) 
								until (CFrame.new(5315.6318359375, 22.562606811523438, -131.0099334716797).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 or _G.AutoFarmCavander == false
							end
						end
					end
				end)
			end)
			
			Main:Toggle("Auto Cavander Hop",_G.AutoFarmCavander_Hop,function(value)
				_G.AutoFarmCavander_Hop = value
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if (_G.AutoFarmCavander_Hop) and World3 and not game:GetService("ReplicatedStorage"):FindFirstChild("Beautiful Pirate [Lv. 1950] [Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Beautiful Pirate [Lv. 1950] [Boss]") then
							Hop()
						end
					end
				end)
			end)
			end			

			if World3 then
				Main:Seperator("Tushita")
				
				Main:Toggle("Auto Tushita",_G.AutoEnmaSword,function(v)
					if _G.SelectWeapon == nil then
						local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
						local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
						wait(1)
						Notification:Notify(
							{Title = "Pado Hub", Description = "Select Weapon"},
							{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
						)
					else
					_G.AutoTushitaSword = v
					StopTween(_G.AutoTushitaSword)
				end
				end)
				
				Main:Toggle("Auto Tushita Hop",_G.AutoEnmaHop,function(v)
					HopFunction = v
				end)
				
				spawn(function()
					while wait() do
						if _G.AutoTushitaSword then
							autoTushita()
						end
					end
				end)
				
				function enemyrip()
					repeat 
						TP(CFrame.new(-5332.30371, 423.985413, -2673.48218)) 
						wait() 
					until _G.StopTween == true or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-5332.30371, 423.985413, -2673.48218)).Magnitude <= 10
					wait()
					if game.Workspace.Enemies:FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") then
						local mobs = game.Workspace.Enemies:GetChildren()
						for i,v in pairs(mobs) do
							if v.Name == "rip_indra True Form [Lv. 5000] [Raid Boss]" and v:IsA("Model") and v:FindFirstChild("Humanoid") and
								v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
								return v
							end
						end
					end
					return game.ReplicatedStorage:FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]")
				end
				function enemyEliteBoss()
					if game.Workspace.Enemies:FindFirstChild("Deandre [Lv. 1750]") or game.Workspace.Enemies:FindFirstChild("Urban [Lv. 1750]") or game.Workspace.Enemies:FindFirstChild("Diablo [Lv. 1750]") then
						local mobs = game.Workspace.Enemies:GetChildren()
						for i,v in pairs(mobs) do
							if v.Name == "Deandre [Lv. 1750]" or v.Name == "Diablo [Lv. 1750]" or v.Name == "Urban [Lv. 1750]"  and v:IsA("Model") and v:FindFirstChild("Humanoid") and
								v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
								return v
							end
						end
					end
					return game.ReplicatedStorage:FindFirstChild("Deandre [Lv. 1750]") or game.ReplicatedStorage:FindFirstChild("Urban [Lv. 1750]") or game.ReplicatedStorage:FindFirstChild("Diablo [Lv. 1750]")
				end
				function enemylongma()
					repeat 
						TP(CFrame.new(-10171.7051, 406.981995, -9552.31738)) 
						wait() 
					until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-10171.7051, 406.981995, -9552.31738)).Magnitude <= 10
					if game.Workspace.Enemies:FindFirstChild("Longma [Lv. 2000] [Boss]") then
						local mobs = game.Workspace.Enemies:GetChildren()
						for i,v in pairs(mobs) do
							if v.Name == "Longma [Lv. 2000] [Boss]" and v:IsA("Model") and v:FindFirstChild("Humanoid") and
								v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
								return v
							end
						end
					end
					return game.ReplicatedStorage:FindFirstChild("Longma [Lv. 2000] [Boss]")
				end
				
				_G.checkup = true
				function autoTushita()
					if _G.checkup and not game.Players.LocalPlayer.Backpack:FindFirstChild("God's Chalice") and not game.Players.LocalPlayer.Character:FindFirstChild("God's Chalice") then
						if game.Workspace.Enemies:FindFirstChild("Deandre [Lv. 1750]") or game.Workspace.Enemies:FindFirstChild("Urban [Lv. 1750]") or game.Workspace.Enemies:FindFirstChild("Diablo [Lv. 1750]") or game.ReplicatedStorage:FindFirstChild("Deandre [Lv. 1750]") or game.ReplicatedStorage:FindFirstChild("Urban [Lv. 1750]") or game.ReplicatedStorage:FindFirstChild("Diablo [Lv. 1750]") then
							if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
								repeat 
									TP(CFrame.new(-5420.49219, 314.446045, -2823.07373)) 
									wait() 
								until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-5420.49219, 314.446045, -2823.07373)).Magnitude <= 10
								wait(1.1)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter")
								wait(1)
							elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
								CheckLevel()
								pcall(function()
									EquipWeapon(_G.SelectWeapon)
									pcall(function()
										local v = enemyEliteBoss()
										v.HumanoidRootPart.CanCollide = false
										v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
										TP(v.HumanoidRootPart.CFrame * Farm_Mode) 
										game:GetService("VirtualUser"):CaptureController()
										game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
									end)										
								end)
							end
						elseif HopFunction then
							TP(CFrame.new(-12554.9443, 337.194092, -7501.44727, 0.906377554, 4.23948272e-08, -0.422468632, -1.89128269e-08, 1, 5.97740595e-08, 0.422468632, -4.61877896e-08, 0.906377554))				
							wait(1)
							HopServer()
						end
					elseif game.Players.LocalPlayer.Backpack:FindFirstChild("God's Chalice") or game.Players.LocalPlayer.Character:FindFirstChild("God's Chalice") then
						_G.checkup = false
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("activateColor","Winter Sky")
						wait(0.5)
						repeat 
							TP(CFrame.new(-5420.16602, 1084.9657, -2666.8208)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-5420.16602, 1084.9657, -2666.8208)).Magnitude <= 10
						wait(0.5)
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("activateColor","Pure Red")
						wait(0.5)
						repeat 
							TP(CFrame.new(-5414.41357, 309.865753, -2212.45776)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-5414.41357, 309.865753, -2212.45776)).Magnitude <= 10
						wait(0.5)
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("activateColor","Snow White")
						wait(0.5)
						repeat 
							TP(CFrame.new(-4971.47559, 331.565765, -3720.02954)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-4971.47559, 331.565765, -3720.02954)).Magnitude <= 10
						wait(0.5)
						EquipWeapon("God's Chalice")
						wait(0.5)
						repeat 
							TP(CFrame.new(-5560.27295, 313.915466, -2663.89795)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-5560.27295, 313.915466, -2663.89795)).Magnitude <= 10
						wait(0.5)
						repeat 
							TP(CFrame.new(-5561.37451, 313.342529, -2663.49487)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-5561.37451, 313.342529, -2663.49487)).Magnitude <= 10
						wait(1)
						repeat 
							TP(CFrame.new(5154.17676, 141.786423, 911.046326)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(5154.17676, 141.786423, 911.046326)).Magnitude <= 10
						wait(0.2)
						repeat 
							TP(CFrame.new(5148.03613, 162.352493, 910.548218)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(5148.03613, 162.352493, 910.548218)).Magnitude <= 10
						wait(1)
						EquipWeapon("Holy Torch")
						wait(1)
						wait(0.4)
						repeat 
							TP(CFrame.new(-10752.7695, 412.229523, -9366.36328)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-10752.7695, 412.229523, -9366.36328)).Magnitude <= 10
						wait(0.4)
						repeat 
							TP(CFrame.new(-11673.4111, 331.749023, -9474.34668)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-11673.4111, 331.749023, -9474.34668)).Magnitude <= 10
						wait(0.4)
						repeat 
							TP(CFrame.new(-12133.3389, 519.47522, -10653.1904)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-12133.3389, 519.47522, -10653.1904)).Magnitude <= 10
						wait(0.4)
						repeat 
							TP(CFrame.new(-13336.5, 485.280396, -6983.35254, 0.912677109)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-13336.5, 485.280396, -6983.35254, 0.912677109)).Magnitude <= 10
						wait(0.4)
						repeat 
							TP(CFrame.new(-13487.4131, 334.84845, -7926.34863)) 
							wait() 
						until _G.StopTween == true or not _G.AutoTushitaSword or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-13487.4131, 334.84845, -7926.34863)).Magnitude <= 10
						wait(1)
					elseif game.Workspace.Enemies:FindFirstChild("Longma [Lv. 2000] [Boss]") or game.ReplicatedStorage:FindFirstChild("Longma [Lv. 2000] [Boss]") then
						pcall(function()
							EquipWeapon(_G.SelectWeapon)
							pcall(function()
								local v = enemylongma()
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)
								game:GetService("VirtualUser"):CaptureController()
								game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
							end)
						end)
					elseif game.Workspace.Enemies:FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") or game.ReplicatedStorage:FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") then
						pcall(function()
							EquipWeapon(_G.SelectWeapon)
							pcall(function()
								local v = enemyrip()
								v.HumanoidRootPart.CanCollide = false
								v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
								TP(v.HumanoidRootPart.CFrame * Farm_Mode)
								game:GetService("VirtualUser"):CaptureController()
								game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
							end)
						end)
					elseif HopFunction then
						TP(CFrame.new(-12554.9443, 337.194092, -7501.44727, 0.906377554, 4.23948272e-08, -0.422468632, -1.89128269e-08, 1, 5.97740595e-08, 0.422468632, -4.61877896e-08, 0.906377554))
						wait(1)
						HopServer()
					end
				end
				end
				
				if World3 then
					Main:Seperator("Enma & Yama")
				
					Main:Toggle("Auto Enma & Yama",_G.AutoYama,function(v)
					if _G.SelectWeapon == nil then
						local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
						local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
						wait(1)
						Notification:Notify(
							{Title = "Pado Hub", Description = "Select Weapon"},
							{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
						)
					else
					_G.AutoYama = v
					StopTween(_G.AutoYama)
				end
				end)
				
				Main:Toggle("Auto Enma & Yama Hop",_G.AutoYamaHOP,function(v)
					_G.AutoYamaHOP = v
				end)
				
				spawn(function()
					while wait() do
						if _G.AutoYama then
							if game:GetService("ReplicatedStorage").Remotes["CommF_"]:InvokeServer("EliteHunter", "Progress") < 30 then
								if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then
									if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Diablo") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Urban") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Deandre") then
										for i,v in pairs(game.ReplicatedStorage:GetChildren()) do
											if string.find(v.Name,"Diablo") then
												YemaTween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
												if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
													if YemaTween then
														YemaTween:Stop()
													end
													game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
												end
											end	
											if string.find(v.Name,"Urban") then
												YemaTween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
												if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
													if YemaTween then
														YemaTween:Stop()
													end
													game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
												end
											end	
											if string.find(v.Name,"Deandre") then
												YemaTween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
												if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
													if YemaTween then
														YemaTween:Stop()
													end
													game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
												end
											end	
										end
										for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
											if _G.AutoYama and string.find(v.Name,"Diablo") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
												repeat wait()
													if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
														Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
													elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
														if Farmtween then
															Farmtween:Stop()
														end
														EquipWeapon(_G.SelectWeapon)
														v.Humanoid:ChangeState(11)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,30,0)
													end 
												until not _G.AutoYama or not v.Parent or v.Humanoid.Health <= 0
											end
											if _G.AutoYama and string.find(v.Name,"Urban") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
												repeat wait()
													if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
														Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
													elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
														if Farmtween then
															Farmtween:Stop()
														end
														EquipWeapon(_G.SelectWeapon)
														v.Humanoid:ChangeState(11)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,30,0)
													end 
												until not _G.AutoYama or not v.Parent or v.Humanoid.Health <= 0
											end
											if _G.AutoYama and string.find(v.Name,"Deandre") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
												repeat wait()
													if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
														Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
													elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
														if Farmtween then
															Farmtween:Stop()
														end
														EquipWeapon(_G.SelectWeapon)
														v.Humanoid:ChangeState(11)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,30,0)
													end 
												until not _G.AutoYama or not v.Parent or v.Humanoid.Health <= 0
											end
										end
									else
										local string_1 = "EliteHunter";
										local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
										Target:InvokeServer(string_1);
									end
								else
									if _G.AutoYamaHOP and game:GetService("ReplicatedStorage").Remotes["CommF_"]:InvokeServer("EliteHunter") == "I don't have anything for you right now. Come back later." then
										local PlaceID = game.PlaceId
										local AllIDs = {}
										local foundAnything = ""
										local actualHour = os.date("!*t").hour
										local Deleted = false
										function TPReturner()
											local Site;
											if foundAnything == "" then
												Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
											else
												Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
											end
											local ID = ""
											if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
												foundAnything = Site.nextPageCursor
											end
											local num = 0;
											for i,v in pairs(Site.data) do
												local Possible = true
												ID = tostring(v.id)
												if tonumber(v.maxPlayers) > tonumber(v.playing) then
													for _,Existing in pairs(AllIDs) do
														if num ~= 0 then
															if ID == tostring(Existing) then
																Possible = false
															end
														else
															if tonumber(actualHour) ~= tonumber(Existing) then
																local delFile = pcall(function()
																	-- delfile("NotSameServers.json")
																	AllIDs = {}
																	table.insert(AllIDs, actualHour)
																end)
															end
														end
														num = num + 1
													end
													if Possible == true then
														table.insert(AllIDs, ID)
														wait()
														pcall(function()
															-- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
															wait()
															game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
														end)
														wait(1)
													end
												end
											end
										end
										function Teleport() 
											while wait() do
												pcall(function()
													TPReturner()
													if foundAnything ~= "" then
														TPReturner()
													end
												end)
											end
										end
										Teleport()
									else
										local string_1 = "EliteHunter";
										local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
										Target:InvokeServer(string_1);
									end
								end
							else
								TweenYema = TP2(game.Workspace.Map.Waterfall.SealedKatana.Handle.Position,game.Workspace.Map.Waterfall.SealedKatana.Handle.CFrame)
								if (game.Workspace.Map.Waterfall.SealedKatana.Handle.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
									if TweenYema then
										TweenYema:Stop()
									end
									if game.Workspace.Enemies:FindFirstChild("Ghost [Lv. 1500]") then
										for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
											if _G.AutoYama and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == "Ghost [Lv. 1500]" then
												repeat wait()
													if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
														Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
													elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
														if Farmtween then
															Farmtween:Stop()
														end
														EquipWeapon(_G.SelectWeapon)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 30, 0)
													end 
												until not _G.AutoYama or not v.Parent or v.Humanoid.Health <= 0
											end
										end
									else
										if TweenYema then
											TweenYema:Stop()
										end
										fireclickdetector(game.Workspace.Map.Waterfall.SealedKatana.Handle.ClickDetector)
									end
								end
							end
						end
					end
				end)
				end				

				if World1 then
					Main:Seperator("Pole V.1")
					
					Main:Toggle("Auto Pole V.1",_G.AutoPole,function(value)
						if _G.SelectWeapon == nil then
							local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
							local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
							wait(1)
							Notification:Notify(
								{Title = "Pado Hub", Description = "Select Weapon"},
								{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
							)
						else
						_G.AutoPole = value
						StopTween(_G.AutoPole)
					end
					end)
					
					Main:Toggle("Auto Pole V.1 Hop",_G.AutoPole_Hop,function(value)
						_G.AutoPole_Hop = value
					end)
					
					spawn(function()
						while wait() do
							if _G.AutoPole then
								pcall(function()
									if game:GetService("Workspace").Enemies:FindFirstChild("Thunder God [Lv. 575] [Boss]") then
										for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
											if v.Name == "Thunder God [Lv. 575] [Boss]" then
												if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
													repeat task.wait()
														AutoHaki()
														EquipWeapon(_G.SelectWeapon)
														v.Humanoid:ChangeState(11)
														v.HumanoidRootPart.Size = Vector3.new(50,50,50)
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
														game:GetService("VirtualUser"):CaptureController()
														game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
														sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
													until not _G.AutoPole or not v.Parent or v.Humanoid.Health <= 0
												end
											end
										end
									else
										if game:GetService("ReplicatedStorage"):FindFirstChild("Thunder God [Lv. 575] [Boss]") then
											TP(game:GetService("ReplicatedStorage"):FindFirstChild("Thunder God [Lv. 575] [Boss]").HumanoidRootPart.CFrame * CFrame.new(5,10,7))
										end
									end
								end)
							end
						end
					end)
					
					spawn(function()
						pcall(function()
							while wait() do
								if (_G.AutoPole_Hop) and World1 and not game:GetService("ReplicatedStorage"):FindFirstChild("Thunder God [Lv. 575] [Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Thunder God [Lv. 575] [Boss]") then
									Hop()
								end
							end
						end)
					end)
					end
				
					if World1 then
						Main:Seperator("Trident")
				
						Main:Toggle("Auto Shark Trident",_G.AutoFarmFishmanIsland,function(value)
							if _G.SelectWeapon == nil then
								local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
								local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
								wait(1)
								Notification:Notify(
									{Title = "Pado Hub", Description = "Select Weapon"},
									{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
								)
							else
							_G.AutoFarmFishmanIsland = value
							StopTween(_G.AutoFarmFishmanIsland)
						end
						end)					
						
						spawn(function()
							while wait() do
								if _G.AutoFarmFishmanIsland then
									pcall(function()
										if game:GetService("Workspace").Enemies:FindFirstChild("Fishman Lord [Lv. 425] [Boss]") then
											for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
												if v.Name == "Fishman Lord [Lv. 425] [Boss]" then
													if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
														repeat task.wait()
															AutoHaki()
															EquipWeapon(_G.SelectWeapon)
															v.Humanoid:ChangeState(11)
															v.HumanoidRootPart.Size = Vector3.new(50,50,50)
															TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
															game:GetService("VirtualUser"):CaptureController()
															game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
															sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
														until not _G.AutoFarmFishmanIsland or not v.Parent or v.Humanoid.Health <= 0 
													end
												end
											end
										else
											repeat task.wait()
												game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875)) 
											until (CFrame.new(61163.8515625, 11.6796875, 1819.7841796875).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1 or _G.AutoFarmFishmanIsland == false
										end
									end)
								end
							end
						end)
						
						Main:Toggle("Auto Shark Trident Hop",_G.AutoFarmFishmanIsland_Hop,function(value)
							_G.AutoFarmFishmanIsland_Hop = value
						end)
						
						spawn(function()
							pcall(function()
								while wait() do
									if (_G.AutoFarmFishmanIsland_Hop) and World1 and not game:GetService("ReplicatedStorage"):FindFirstChild("Fishman Lord [Lv. 425] [Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Fishman Lord [Lv. 425] [Boss]") then
										Hop()
									end
								end
							end)
						end)
					end

						if World2 then
							Main:Seperator("Trident")
						
							Main:Toggle("Auto Dragon Trident",_G.Auto_Dragon_Trident,function(value)
								if _G.SelectWeapon == nil then
									local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
									local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
									wait(1)
									Notification:Notify(
										{Title = "Pado Hub", Description = "Select Weapon"},
										{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
									)
								else
						 _G.Auto_Dragon_Trident = value
						StopTween(_G.Auto_Dragon_Trident)
							end
						end)
							
						Main:Toggle("Auto Dragon Trident Hop",_G.Auto_Dragon_Trident_Hop,function(value)
						_G.Auto_Dragon_Trident_Hop = value
						end)
						
							spawn(function()
								while wait() do
									if _G.Auto_Dragon_Trident then
										pcall(function()
											if _G.Auto_Dragon_Trident and game.ReplicatedStorage:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") or game.Workspace.Enemies:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") then
												if game.Workspace.Enemies:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") then
													for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
														if v.Name == "Tide Keeper [Lv. 1475] [Boss]" and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
															repeat wait()
																EquipWeapon(_G.SelectWeapon)
																AutoHaki()
																v.Humanoid:ChangeState(11)
																v.HumanoidRootPart.Size = Vector3.new(50,50,50)
																TP(v.HumanoidRootPart.CFrame * Farm_Mode)    																	
																game:GetService'VirtualUser':CaptureController()
																game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
															until _G.Auto_Dragon_Trident or v.Humanoid.Health <= 0 or not v.Parent
														end
													end
												else
													TP(CFrame.new(-3914.830322265625, 123.29389190673828, -11516.8642578125))
												end
											else
												if not game.ReplicatedStorage:FindFirstChild("Tide Keeper [Lv. 1475] [Boss]") and _G.Auto_Dragon_Trident_Hop then
													hop()
												end
											end
										end)
									end
								end
							end)
						end				

						if World2 then
							Main:Seperator("Long sword")
					
							Main:Toggle("Auto Long sword",_G.AutoLongsword,function(value)
								if _G.SelectWeapon == nil then
									local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
									local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
									wait(1)
									Notification:Notify(
										{Title = "Pado Hub", Description = "Select Weapon"},
										{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
									)
								else
								_G.AutoLongsword = value
								StopTween(_G.AutoLongsword)
							end
							end)					
							
							spawn(function()
								while wait() do
									if _G.AutoLongsword then
										pcall(function()
											if game:GetService("Workspace").Enemies:FindFirstChild("Diamond [Lv. 750] [Boss]") then
												for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
													if v.Name == "Diamond [Lv. 750] [Boss]" then
														if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
															repeat task.wait()
																AutoHaki()
																EquipWeapon(_G.SelectWeapon)
																v.Humanoid:ChangeState(11)
																v.HumanoidRootPart.Size = Vector3.new(50,50,50)
																TP(v.HumanoidRootPart.CFrame * Farm_Mode)                         
																game:GetService("VirtualUser"):CaptureController()
																game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
																sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
															until not _G.AutoLongsword or not v.Parent or v.Humanoid.Health <= 0
														end
													end
												end
											else
												if game:GetService("ReplicatedStorage"):FindFirstChild("Diamond [Lv. 750] [Boss]") then
													TP(game:GetService("ReplicatedStorage"):FindFirstChild("Diamond [Lv. 750] [Boss]").HumanoidRootPart.CFrame * CFrame.new(5,10,7))
												end
											end
										end)
									end
								end
							end)
							
							Main:Toggle("Auto Long sword Hop",_G.AutoLongsword_Hop,function(value)
								_G.AutoLongsword_Hop = value
							end)
							
							spawn(function()
								pcall(function()
									while wait() do
										if (_G.AutoLongsword_Hop) and World2 and not game:GetService("ReplicatedStorage"):FindFirstChild("Diamond [Lv. 750] [Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("Diamond [Lv. 750] [Boss]") then
											Hop()
										end
									end
								end)
							end)
							end

							if World2 then
								Main:Seperator("Oder Sword")
							  
								Main:Toggle("Auto Oder Sword",_G.AutoOderSword,function(value)
									if _G.SelectWeapon == nil then
										local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
										local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
										wait(1)
										Notification:Notify(
											{Title = "Pado Hub", Description = "Select Weapon"},
											{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
										)
									else
								   _G.AutoOderSword = value
								  StopTween(_G.AutoOderSword)
								end
							  end)
							  
							  spawn(function()
								  while wait() do
									  if _G.AutoOderSword then
										  pcall(function()
											  if game:GetService("Workspace").Enemies:FindFirstChild("Order [Lv. 1250] [Raid Boss]") then
												  for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
													  if v.Name == "Order [Lv. 1250] [Raid Boss]" then
														  if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
															  repeat task.wait()
																  AutoHaki()
																  EquipWeapon(_G.SelectWeapon)
																  v.Humanoid:ChangeState(11)
																  v.HumanoidRootPart.Size = Vector3.new(60,60,60)
																  TP(v.HumanoidRootPart.CFrame * Farm_Mode)
																  game:GetService("VirtualUser"):CaptureController()
																  game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
																  sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
															  until not _G.AutoOderSword or not v.Parent or v.Humanoid.Health <= 0
														  end
													  end
												  end
											  else
												  if game:GetService("ReplicatedStorage"):FindFirstChild("Order [Lv. 1250] [Raid Boss]") then
													  TP(game:GetService("ReplicatedStorage"):FindFirstChild("Order [Lv. 1250] [Raid Boss]").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
												  end
											  end
										  end)
									  end
								  end
							  end)
						  
							  Main:Toggle("Auto Buy Microchip Oder",_G.MicrochipOder,function(value)
								  _G.MicrochipOder = value
							  end)
						  
						spawn(function()
							while wait() do
								if _G.MicrochipOder then
									if not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Microchip") and not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Microchip") then											  
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Microchip","2")
									end
								end
							end
						end)
						  
						Main:Toggle("Auto Start Raid Oder",_G.AutoStartRaidOder,function(value)
								  _G.AutoStartRaidOder = value
							  end)
							  
							  spawn(function()
								  while wait() do
									  pcall(function()
										  if _G.AutoStartRaidOder then
											  if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
												  if not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Microchip") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Microchip") then
													  if World2 then
														fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon.Button.Main.ClickDetector)												
													 end
												 end
											  end
										  end
									  end)
								  end
							  end)
						  end						  

						  if World1 then
							Main:Seperator("Saber")
								
								Main:Toggle("Auto Saber",_G.AutoSaber,function(value)
									if _G.SelectWeapon == nil then
										local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
										local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
										wait(1)
										Notification:Notify(
											{Title = "Pado Hub", Description = "Select Weapon"},
											{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
										)
									else
								   _G.AutoSaber = value
								end
							end)
										
										Main:Toggle("Auto Saber Hop",_G.AutoSaberHop,function(value)
											_G.AutoSaberHop = value
										end)
										
									spawn(function()
										while wait() do
											if _G.AutoSaber then
												if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Saber") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Saber") then
													game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("LoadItem","Saber")
														local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
														local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
														wait(1)
														Notification:Notify(
															{Title = "Pado Hub", Description = "You Have Saber"},
															{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
														)
													_G.AutoSaber = false
												end
												if game.Players.localPlayer.Data.Level.Value < 200 then
												else
													if game.Workspace.Map.Jungle.Final.Part.CanCollide == false then
														if _G.AutoSaber and game.ReplicatedStorage:FindFirstChild("Saber Expert [Lv. 200] [Boss]") or game.Workspace.Enemies:FindFirstChild("Saber Expert [Lv. 200] [Boss]") then
															if game.Workspace.Enemies:FindFirstChild("Saber Expert [Lv. 200] [Boss]") then
																for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
																	if v.Name == "Saber Expert [Lv. 200] [Boss]" and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
																		repeat wait()
																			if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
																				Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
																			elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																				if Farmtween then
																					Farmtween:Stop()
																				end
																				AutoHaki()
																				EquipWeapon(_G.SelectWeapon)
																				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 30, 0)
																				game:GetService'VirtualUser':CaptureController()
																				game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
																			end
																		until not _G.AutoSaber or not v.Parent or v.Humanoid.Health <= 0
																	end
																end
															else
																Questtween = TP2(CFrame.new(-1405.41956, 29.8519993, 5.62435055).Position,CFrame.new(-1405.41956, 29.8519993, 5.62435055))
																if (CFrame.new(-1405.41956, 29.8519993, 5.62435055).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																	if Questtween then
																		Questtween:Stop()
																	end
																	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1405.41956, 29.8519993, 5.62435055, 0.885240912, 3.52892613e-08, 0.465132833, -6.60881128e-09, 1, -6.32913171e-08, -0.465132833, 5.29540891e-08, 0.885240912)
																end
															end
														else
															if _G.AutoSaberHop then
																Hop()
															end
														end
													elseif game.Players.LocalPlayer.Backpack:FindFirstChild("Relic") or game.Players.LocalPlayer.Character:FindFirstChild("Relic") and game.Players.localPlayer.Data.Level.Value >= 200 then
														EquipWeapon("Relic")
														wait(0.5)
														Questtween = TP2(CFrame.new(-1405.41956, 29.8519993, 5.62435055).Position,CFrame.new(-1405.41956, 29.8519993, 5.62435055))
														if (CFrame.new(-1405.41956, 29.8519993, 5.62435055).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
															if Questtween then
																Questtween:Stop()
															end
															game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1405.41956, 29.8519993, 5.62435055, 0.885240912, 3.52892613e-08, 0.465132833, -6.60881128e-09, 1, -6.32913171e-08, -0.465132833, 5.29540891e-08, 0.885240912)
														end
													else
														if Workspace.Map.Jungle.QuestPlates.Door.CanCollide == false then
															if game.Workspace.Map.Desert.Burn.Part.CanCollide == false then
																if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","SickMan") == 0 then
																	if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","RichSon") == 0 then
																		if game.Workspace.Enemies:FindFirstChild("Mob Leader [Lv. 120] [Boss]") then
																			for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
																				if _G.AutoSaber and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == "Mob Leader [Lv. 120] [Boss]" then
																					repeat
																						pcall(function() wait() 
																							if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
																								Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
																							elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																								if Farmtween then
																									Farmtween:Stop()
																								end
																								AutoHaki()
																								EquipWeapon(_G.SelectWeapon)
																								if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
																									local args = {
																										[1] = "Buso"
																									}
																									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
																								end
																								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 30, 0)
																								game:GetService'VirtualUser':CaptureController()
																								game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
																							end
																						end)
																					until not _G.AutoSaber or not v.Parent or v.Humanoid.Health <= 0
																				end
																			end
																		else
																			Questtween = TP2(CFrame.new(-2848.59399, 7.4272871, 5342.44043).Position,CFrame.new(-2848.59399, 7.4272871, 5342.44043))
																			if (CFrame.new(-2848.59399, 7.4272871, 5342.44043).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																				if Questtween then
																					Questtween:Stop()
																				end
																				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2848.59399, 7.4272871, 5342.44043, -0.928248107, -8.7248246e-08, 0.371961564, -7.61816636e-08, 1, 4.44474857e-08, -0.371961564, 1.29216433e-08, -0.928248107)
																			end
																		end
																	elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","RichSon") == 1 then
																		if game.Players.LocalPlayer.Backpack:FindFirstChild("Relic") or game.Players.LocalPlayer.Character:FindFirstChild("Relic") then
																			EquipWeapon("Relic")
																			wait(0.5)
																			Questtween = TP2(CFrame.new(-1405.41956, 29.8519993, 5.62435055).Position,CFrame.new(-1405.41956, 29.8519993, 5.62435055))
																			if (CFrame.new(-1405.41956, 29.8519993, 5.62435055).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																				if Questtween then
																					Questtween:Stop()
																				end
																				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1405.41956, 29.8519993, 5.62435055)
																			end
																		else
																			Questtween = TP2(CFrame.new(-910.979736, 13.7520342, 4078.14624).Position,CFrame.new(-910.979736, 13.7520342, 4078.14624))
																			if (CFrame.new(-910.979736, 13.7520342, 4078.14624).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																				if Questtween then
																					Questtween:Stop()
																				end
																				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-910.979736, 13.7520342, 4078.14624, 0.00685182028, -1.53155766e-09, -0.999976516, 9.15205245e-09, 1, -1.46888401e-09, 0.999976516, -9.14177267e-09, 0.00685182028)
																				wait(.5)
																				local args = {
																					[1] = "ProQuestProgress",
																					[2] = "RichSon"
																				}
																				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
																			end
																		end
																	else
																		Questtween = TP2(CFrame.new(-910.979736, 13.7520342, 4078.14624).Position,CFrame.new(-910.979736, 13.7520342, 4078.14624))
																		if (CFrame.new(-910.979736, 13.7520342, 4078.14624).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																			if Questtween then
																				Questtween:Stop()
																			end
																			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-910.979736, 13.7520342, 4078.14624)
																			local args = {
																				[1] = "ProQuestProgress",
																				[2] = "RichSon"
																			}
																			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
																		end
																	end
																else
																	if game.Players.LocalPlayer.Backpack:FindFirstChild("Cup") or game.Players.LocalPlayer.Character:FindFirstChild("Cup") then
																		EquipWeapon("Cup")
																		if game.Players.LocalPlayer.Character.Cup.Handle:FindFirstChild("TouchInterest") then
																			Questtween = TP2(CFrame.new(1397.229, 37.3480148, -1320.85217).Position,CFrame.new(1397.229, 37.3480148, -1320.85217))
																			if (CFrame.new(1397.229, 37.3480148, -1320.85217).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																				if Questtween then
																					Questtween:Stop()
																				end
																				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1397.229, 37.3480148, -1320.85217, -0.11285457, 2.01368788e-08, 0.993611455, 1.91641178e-07, 1, 1.50028845e-09, -0.993611455, 1.90586206e-07, -0.11285457)
																			end
																		else
																			wait(0.5)
																			if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","SickMan") ~= 0 then
																				local args = {
																					[1] = "ProQuestProgress",
																					[2] = "SickMan"
																				}
																				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
																			end
																		end
																	else
																		Questtween = TP2(game.Workspace.Map.Desert.Cup.Position,game.Workspace.Map.Desert.Cup.CFrame)
																		if (game.Workspace.Map.Desert.Cup.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																			if Questtween then
																				Questtween:Stop()
																			end
																			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Map.Desert.Cup.CFrame
																		end
																		firetouchinterest(game.Workspace.Map.Desert.Cup.TouchInterest,game.Players.LocalPlayer.Character.Head, 1)
																	end
																end
															else
																if game.Players.LocalPlayer.Backpack:FindFirstChild("Torch") or game.Players.LocalPlayer.Character:FindFirstChild("Torch") then
																	EquipWeapon("Torch")
																	Questtween = TP2(CFrame.new(1114.87708, 4.9214654, 4349.8501).Position,CFrame.new(1114.87708, 4.9214654, 4349.8501))
																	if (CFrame.new(1114.87708, 4.9214654, 4349.8501).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																		if Questtween then
																			Questtween:Stop()
																		end
																		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1114.87708, 4.9214654, 4349.8501, -0.612586915, -9.68697833e-08, 0.790403247, -1.2634203e-07, 1, 2.4638446e-08, -0.790403247, -8.47679615e-08, -0.612586915)
																	end
																else
																	Questtween = TP2(CFrame.new(-1610.00757, 11.5049858, 164.001587).Position,CFrame.new(-1610.00757, 11.5049858, 164.001587))
																	if (CFrame.new(-1610.00757, 11.5049858, 164.001587).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
																		if Questtween then
																			Questtween:Stop()
																		end
																		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1610.00757, 11.5049858, 164.001587, 0.984807551, -0.167722285, -0.0449818149, 0.17364943, 0.951244235, 0.254912198, 3.42372805e-05, -0.258850515, 0.965917408)
																	end
																end
															end
														else
															for i,v in pairs(Workspace.Map.Jungle.QuestPlates:GetChildren()) do
																if v:IsA("Model") then wait()
																	if v.Button.BrickColor ~= BrickColor.new("Camo") then
																		repeat wait()
																			Questtween = TP2(v.Button.Position,v.Button.CFrame)
																			if (v.Button.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 150 then
																				if Questtween then
																					Questtween:Stop()
																				end
																				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Button.CFrame
																			end
																		until not _G.AutoSaber or v.Button.BrickColor == BrickColor.new("Camo")
																	end
																end
															end    
														end
													end
												end 
											end
										end
									end)
								end				
								
if World2 or World3 then
		Quest:Seperator("Quest")
	end
		
		Quest:Toggle("Auto Player Hunter",_G.AutoPlayerHunter,function(x)
			if _G.SelectWeapon == nil then
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description =  "Select Weapon"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
				)
			else
			_G.AutoPlayerHunter = x
			StopTween(_G.AutoPlayerHunter)
		end
		end)
	
			spawn(function()
				while wait(.1) do
					if _G.AutoPlayerHunter then
						if game:GetService("Players").LocalPlayer.PlayerGui.Main.PvpDisabled.Visible == true then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EnablePvp")
						else
						if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
							wait(.5)
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PlayerHunter")
						else
							for i,v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
								if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text,v.Name) then
									repeat task.wait()
										if game:GetService("Players").LocalPlayer.PlayerGui.Main.SafeZone.Visible == true then
												game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(20, 50, 0)
												game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PlayerHunter")
											end
												EquipWeapon(_G.SelectWeapon)
												TP(v.HumanoidRootPart.CFrame * CFrame.new(1,7,3))								
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
											until _G.AutoPlayerHunter == false or v.Humanoid.Health <= 0
												game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
											end
										end
									end
								end
							end
						end
					end)
	
		if World3 then
			Quest:Toggle("Auto Musketeer Hat",_G.AutoMusketeerHat,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
			_G.AutoMusketeerHat = value
			StopTween(_G.AutoMusketeerHat)
			end
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if _G.AutoMusketeerHat then
						if game:GetService("Players").LocalPlayer.Data.Level.Value >= 1800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress").KilledBandits == false then
							if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Forest Pirate") and string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "50") and game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
								if game:GetService("Workspace").Enemies:FindFirstChild("Forest Pirate [Lv. 1825]") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v.Name == "Forest Pirate [Lv. 1825]" then
											repeat task.wait()
												pcall(function()
													EquipWeapon(_G.SelectWeapon)
													AutoHaki()
													v.HumanoidRootPart.Size = Vector3.new(50,50,50)
													TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
											 		v.HumanoidRootPart.CanCollide = false
                                                    v.Humanoid:ChangeState(11)
													game:GetService'VirtualUser':CaptureController()
													game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
													MusketeerHatMon = v.HumanoidRootPart.CFrame
													StartMagnetMusketeerhat = true
												end)
											until _G.AutoMusketeerHat == false or not v.Parent or v.Humanoid.Health <= 0 or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
											StartMagnetMusketeerhat = false
										end
									end
								else
									StartMagnetMusketeerhat = false
									TP(CFrame.new(-13206.452148438, 425.89199829102, -7964.5537109375))
								end
							else
								TP(CFrame.new(-12443.8671875, 332.40396118164, -7675.4892578125))
								if (Vector3.new(-12443.8671875, 332.40396118164, -7675.4892578125) - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 30 then
									wait(1.5)
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest","CitizenQuest",1)
								end
							end
						elseif game:GetService("Players").LocalPlayer.Data.Level.Value >= 1800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress").KilledBoss == false then
							if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible and string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Captain Elephant") and game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
								if game:GetService("Workspace").Enemies:FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v.Name == "Captain Elephant [Lv. 1875] [Boss]" then
											OldCFrameElephant = v.HumanoidRootPart.CFrame
											repeat task.wait()
												pcall(function()
													EquipWeapon(_G.SelectWeapon)
													AutoHaki()
													v.HumanoidRootPart.CanCollide = false
													v.HumanoidRootPart.Size = Vector3.new(50,50,50)
													TP(v.HumanoidRootPart.CFrame * CFrame.new(5,10,7))
                                                    v.Humanoid:ChangeState(11)
													v.HumanoidRootPart.CFrame = OldCFrameElephant
													game:GetService("VirtualUser"):CaptureController()
													game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 672))
													sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
												end)
											until _G.AutoMusketeerHat == false or v.Humanoid.Health <= 0 or not v.Parent or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
										end
									end
								else
									TP(CFrame.new(-13374.889648438, 421.27752685547, -8225.208984375))
									local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
									local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
									wait(1)
									Notification:Notify(
										{Title = "Pado Hub", Description = "The boss hasn't been born yet."},
										{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
									)
								end
							else
								TP(CFrame.new(-12443.8671875, 332.40396118164, -7675.4892578125))
								if (CFrame.new(-12443.8671875, 332.40396118164, -7675.4892578125).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 then
									wait(1.5)
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen")
								end
							end
						elseif game:GetService("Players").LocalPlayer.Data.Level.Value >= 1800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen") == 2 then
							TP(CFrame.new(-12512.138671875, 340.39279174805, -9872.8203125))
						end
					end
				end
			end)
		end)
		end
		
		if World3 then
			Quest:Toggle("Auto Observation Haki v2",_G.AutoObservationv2,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
			_G.AutoObservationv2 = value
			StopTween(_G.AutoObservationv2)
			end
		end)
		
		spawn(function()
			while wait() do
				pcall(function()
					if _G.AutoObservationv2 then
						if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen") == 3 then
							if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Banana") and  game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Apple") and game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Pineapple") then
								repeat 
									TP(CFrame.new(-12444.78515625, 332.40396118164, -7673.1806640625)) 
									wait() 
								until not _G.AutoObservationv2 or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-12444.78515625, 332.40396118164, -7673.1806640625)).Magnitude <= 10
								wait(.5)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen")
							elseif game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Fruit Bowl") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Fruit Bowl") then
								repeat 
									TP(CFrame.new(-10920.125, 624.20275878906, -10266.995117188)) 
									wait() 
								until not _G.AutoObservationv2 or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-10920.125, 624.20275878906, -10266.995117188)).Magnitude <= 10
								wait(.5)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("KenTalk2","Start")
								wait(1)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("KenTalk2","Buy")
							else
								for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
									if v.Name == "Apple" or v.Name == "Banana" or v.Name == "Pineapple" then
										v.Handle.CFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,1,10)
										wait()
										firetouchinterest(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart,v.Handle,0)    
										wait()
									end
								end   
							end
						end
					end
				end)
			end
		end)
		end
		
		if World3 then
			Quest:Toggle("Auto Haki Rainbow",_G.AutoHakiRainbow,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
			_G.AutoHakiRainbow = value
			StopTween(_G.AutoHakiRainbow)
			end
		end)
		
		spawn(function()
			while wait() do
				if _G.AutoHakiRainbow then
					if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then
						if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Stone") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Island Empress") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Kilo Admiral") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Captain Elephant") or string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Beautiful Pirate") then
							if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Stone") then
								if game.Workspace.Enemies:FindFirstChild("Stone [Lv. 1550] [Boss]") then
									for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
										if _G.AutoHakiRainbow and v.Name == "Stone [Lv. 1550] [Boss]" and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											repeat
												pcall(function() wait() 
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
														Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
													elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
														if Farmtween then
															Farmtween:Stop()
														end
														EquipWeapon(_G.SelectWeapon)
                                                        v.Humanoid:ChangeState(11)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 30, 0)
														game:GetService("VirtualUser"):CaptureController()
														game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 672))
													end 
												end)
											until not _G.AutoHakiRainbow or not v.Parent or v.Humanoid.Health <= 0 or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
										end
									end
								else 
									if (CFrame.new(-1134, 40, 6877).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 250 then
										HakiRainbowTween = TP2(CFrame.new(-1134, 40, 6877).Position,CFrame.new(-1134, 40, 6877))
									elseif (CFrame.new(-1134, 40, 6877).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
										if HakiRainbowTween then
											HakiRainbowTween:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1134, 40, 6877)
									end
								end
							elseif string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Island Empress") then
								if game.Workspace.Enemies:FindFirstChild("Island Empress [Lv. 1675] [Boss]") then
									for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
										if _G.AutoHakiRainbow and v.Name == "Island Empress [Lv. 1675] [Boss]" and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											repeat
												pcall(function() wait() 
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
														Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
													elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
														if Farmtween then
															Farmtween:Stop()
														end
                                                        v.Humanoid:ChangeState(11)
														EquipWeapon(_G.SelectWeapon)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 30, 0)
														game:GetService("VirtualUser"):CaptureController()
														game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 672))
													end 
												end)
											until not _G.AutoHakiRainbow or not v.Parent or v.Humanoid.Health <= 0 or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
										end
									end
								else
									if (CFrame.new(5614, 603, 339).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 250 then
										HakiRainbowTween = TP2(CFrame.new(5614, 603, 339).Position,CFrame.new(5614, 603, 339))
									elseif (CFrame.new(5614, 603, 339).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
										if HakiRainbowTween then
											HakiRainbowTween:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5614, 603, 339)
									end
								end	
							elseif string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Kilo Admiral") then
								if game.Workspace.Enemies:FindFirstChild("Kilo Admiral [Lv. 1750] [Boss]") then
									for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
										if _G.AutoHakiRainbow and v.Name == "Kilo Admiral [Lv. 1750] [Boss]" and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											repeat
												pcall(function() wait() 
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
														Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
													elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
														if Farmtween then
															Farmtween:Stop()
														end
                                                        v.Humanoid:ChangeState(11)
														EquipWeapon(_G.SelectWeapon)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 30, 0)
														game:GetService("VirtualUser"):CaptureController()
														game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 672))
													end 
												end)
											until not _G.AutoHakiRainbow or not v.Parent or v.Humanoid.Health <= 0 or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
										end
									end
								else
									if (CFrame.new(2879, 433, -7090).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 250 then
										HakiRainbowTween = TP2(CFrame.new(2879, 433, -7090).Position,CFrame.new(2879, 433, -7090))
									elseif (CFrame.new(2879, 433, -7090).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
										if HakiRainbowTween then
											HakiRainbowTween:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2879, 433, -7090)
									end
								end	
							elseif string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Captain Elephant") then
								if game.Workspace.Enemies:FindFirstChild("Captain Elephant [Lv. 1875] [Boss]") then
									for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
										if _G.AutoHakiRainbow and v.Name == "Captain Elephant [Lv. 1875] [Boss]" and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											repeat
												pcall(function() wait() 
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
														Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
													elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
														if Farmtween then
															Farmtween:Stop()
														end
                                                        v.Humanoid:ChangeState(11)
														EquipWeapon(_G.SelectWeapon)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 30, 0)
														game:GetService("VirtualUser"):CaptureController()
														game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 672))
													end 
												end)
											until not _G.AutoHakiRainbow or not v.Parent or v.Humanoid.Health <= 0 or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
										end
									end
								else
									if (CFrame.new(-13348, 406, -8574).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 250 then
										HakiRainbowTween = TP2(CFrame.new(-13348, 406, -8574).Position,CFrame.new(-13348, 406, -8574))
									elseif (CFrame.new(-13348, 406, -8574).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
										if HakiRainbowTween then
											HakiRainbowTween:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-13348, 406, -8574)
									end
								end	
							elseif string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Beautiful Pirate") then
								if game.Workspace.Enemies:FindFirstChild("Beautiful Pirate [Lv. 1950] [Boss]") then
									for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
										if _G.AutoHakiRainbow and v.Name == "Beautiful Pirate [Lv. 1950] [Boss]" and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											repeat
												pcall(function() wait() 
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													local string_1 = "HornedMan";
													local string_2 = "Bet";
													local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
													Target:InvokeServer(string_1, string_2);
													if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
														Farmtween = TP2(v.HumanoidRootPart.Position,v.HumanoidRootPart.CFrame)
													elseif (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
														if Farmtween then
															Farmtween:Stop()
														end
														v.Humanoid:ChangeState(11)
														EquipWeapon(_G.SelectWeapon)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 30, 0)
														game:GetService("VirtualUser"):CaptureController()
														game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 672))
													end 
												end)
											until not _G.AutoHakiRainbow or not v.Parent or v.Humanoid.Health <= 0 or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
										end
									end
								else
									if (CFrame.new(5206, 23, -80).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 250 then
										HakiRainbowTween = TP2(CFrame.new(5206, 23, -80).Position,CFrame.new(5206, 23, -80))
									elseif (CFrame.new(5206, 23, -80).Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).magnitude > 20000 then
										if HakiRainbowTween then
											HakiRainbowTween:Stop()
										end
										local TouchInterest = game:GetService("Workspace").Map.Turtle.Entrance.Door.BossDoor.Hitbox
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = TouchInterest.CFrame
									elseif (CFrame.new(5206, 23, -80).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 250 then
										if HakiRainbowTween then
											HakiRainbowTween:Stop()
										end
										game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5206, 23, -80)
									end
								end	
							end
						else
							local string_1 = "HornedMan";
							local string_2 = "Bet";
							local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
							Target:InvokeServer(string_1, string_2);
							local string_1 = "HornedMan";
							local string_2 = "Bet";
							local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
							Target:InvokeServer(string_1, string_2);
						end
					else
						local string_1 = "HornedMan";
						local string_2 = "Bet";
						local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
						Target:InvokeServer(string_1, string_2);
						local string_1 = "HornedMan";
						local string_2 = "Bet";
						local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
						Target:InvokeServer(string_1, string_2);
					end
				end
			end
		end)
	end
		
		if World2 then
			Quest:Toggle("Auto Rengoku",_G.AutoRengoku,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
			_G.AutoRengoku = value
			StopTween(_G.AutoRengoku)
		end
	end)
	
                		spawn(function()
							pcall(function()
								while wait() do
									if _G.AutoRengoku then
										if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rengoku") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rengoku") then
											local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
											local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
											wait(1)
											Notification:Notify(
												{Title = "Pado Hub", Description = "Have Rengoku"},
												{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
											)
										end
										if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Hidden Key") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Hidden Key") then
											EquipWeapon("Hidden Key")
											TP(CFrame.new(6571.1201171875, 299.23028564453, -6967.841796875))
										elseif game:GetService("Workspace").Enemies:FindFirstChild("Snow Lurker [Lv. 1375]") or game:GetService("Workspace").Enemies:FindFirstChild("Arctic Warrior [Lv. 1350]") then
											for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
												if (v.Name == "Snow Lurker [Lv. 1375]" or v.Name == "Arctic Warrior [Lv. 1350]") and v.Humanoid.Health > 0 then
													repeat task.wait()
														EquipWeapon(_G.SelectWeapon)
														AutoHaki()
														v.HumanoidRootPart.CanCollide = false
														v.Humanoid:ChangeState(11)
														v.HumanoidRootPart.Size = Vector3.new(60,60,60)
														RengokuMon = v.HumanoidRootPart.CFrame
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														game:GetService'VirtualUser':CaptureController()
														game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
														StartRengokuMagnet = true
													until game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Hidden Key") or not v.Parent or v.Humanoid.Health <= 0
													StartRengokuMagnet = false
												end
											end
										else
											StartRengokuMagnet = false
											TP(CFrame.new(5439.716796875, 84.420944213867, -6715.1635742188))
										end
									end
								end
							end)
						end)
					end
	
		if World2 then
			Quest:Toggle("Auto Quest Flower",_G.Auto_EvoRace,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
			_G.Auto_EvoRace = value
			StopTween(_G.Auto_EvoRace)
			end
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if _G.Auto_EvoRace then
						if not game:GetService("Players").LocalPlayer.Data.Race:FindFirstChild("Evolved") then
							if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","1") == 0 then
								TP(CFrame.new(-2779.83521, 72.9661407, -3574.02002, -0.730484903, 6.39014104e-08, -0.68292886, 3.59963224e-08, 1, 5.50667032e-08, 0.68292886, 1.56424669e-08, -0.730484903))
								if (Vector3.new(-2779.83521, 72.9661407, -3574.02002) - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 then
									wait(1.3)
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","2")
								end
							elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","1") == 1 then
								pcall(function()
									if not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower 1") and not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flower 1") then
										TP(game:GetService("Workspace").Flower1.CFrame)
									elseif not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower 2") and not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flower 2") then
										TP(game:GetService("Workspace").Flower2.CFrame)
									elseif not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower 3") and not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flower 3") then
										if game:GetService("Workspace").Enemies:FindFirstChild("Zombie [Lv. 950]") then
											for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
												if v.Name == "Zombie [Lv. 950]" then
													repeat task.wait()
														AutoHaki()
														EquipWeapon(_G.SelectWeapon)
														TP(v.HumanoidRootPart.CFrame * Farm_Mode)
														v.HumanoidRootPart.CanCollide = false
														v.Humanoid:ChangeState(11)
														v.HumanoidRootPart.Size = Vector3.new(50,50,50)
														game:GetService("VirtualUser"):CaptureController()
														game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 672))
														PosMonEvo = v.HumanoidRootPart.CFrame
														StartEvoMagnet = true
													until game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower 3") or not v.Parent or v.Humanoid.Health <= 0 or _G.Auto_EvoRace == false
													StartEvoMagnet = false
												end
											end
										else
											StartEvoMagnet = false
											TP(CFrame.new(-5685.9233398438, 48.480125427246, -853.23724365234))
										end
									end
								end)
							elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","1") == 2 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","3")
							end
						end
					end
				end
			end)
		end)
		end
		
		if World2 then
			Quest:Toggle("Auto Bartlio Quest",_G.AutoBartilo,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
			_G.AutoBartilo = value
			StopTween(_G.AutoBartilo)
			end
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if _G.AutoBartilo then
						if game:GetService("Players").LocalPlayer.Data.Level.Value >= 800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress","Bartilo") == 0 then
							if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Swan Pirates") and string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "50") and game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then 
								if game:GetService("Workspace").Enemies:FindFirstChild("Swan Pirate [Lv. 775]") then
									Ms = "Swan Pirate [Lv. 775]"
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
										if v.Name == Ms then
											pcall(function()
												repeat task.wait()
													sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
													EquipWeapon(_G.SelectWeapon)
													AutoHaki()
													v.HumanoidRootPart.Transparency = 1
													v.HumanoidRootPart.CanCollide = false
													v.Humanoid:ChangeState(11)
													v.HumanoidRootPart.Size = Vector3.new(50,50,50)
													TP(v.HumanoidRootPart.CFrame * Farm_Mode)												
													PosMonBarto =  v.HumanoidRootPart.CFrame
													game:GetService'VirtualUser':CaptureController()
													game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
													AutoBartiloBring = true
												until not v.Parent or v.Humanoid.Health <= 0 or _G.AutoBartilo == false or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
												AutoBartiloBring = false
											end)
										end
									end
								else
									repeat TP(CFrame.new(932.624451, 156.106079, 1180.27466, -0.973085582, 4.55137119e-08, -0.230443969, 2.67024713e-08, 1, 8.47491108e-08, 0.230443969, 7.63147128e-08, -0.973085582)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(932.624451, 156.106079, 1180.27466, -0.973085582, 4.55137119e-08, -0.230443969, 2.67024713e-08, 1, 8.47491108e-08, 0.230443969, 7.63147128e-08, -0.973085582)).Magnitude <= 10
								end
							else
								repeat TP(CFrame.new(-456.28952, 73.0200958, 299.895966)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-456.28952, 73.0200958, 299.895966)).Magnitude <= 10
								wait(1.1)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest","BartiloQuest",1)
							end 
						elseif game:GetService("Players").LocalPlayer.Data.Level.Value >= 800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress","Bartilo") == 1 then
							if game:GetService("Workspace").Enemies:FindFirstChild("Jeremy [Lv. 850] [Boss]") then
								for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
									if v.Name == "Jeremy [Lv. 850] [Boss]" then
     									repeat task.wait()
											EquipWeapon(_G.SelectWeapon)
											AutoHaki()
											v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                            v.Humanoid:ChangeState(11)
											TP(v.HumanoidRootPart.CFrame * Farm_Mode)												
											game:GetService'VirtualUser':CaptureController()
											game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										until not v.Parent or v.Humanoid.Health <= 0 or _G.AutoBartilo == false
									end
								end
							elseif game:GetService("ReplicatedStorage"):FindFirstChild("Jeremy [Lv. 850] [Boss]") then
								repeat TP(CFrame.new(-456.28952, 73.0200958, 299.895966)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-456.28952, 73.0200958, 299.895966)).Magnitude <= 10
								wait(1.1)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress","Bartilo")
								wait(1)
								repeat TP(CFrame.new(2099.88159, 448.931, 648.997375)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(2099.88159, 448.931, 648.997375)).Magnitude <= 10
								wait(2)
							else
								repeat TP(CFrame.new(2099.88159, 448.931, 648.997375)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(2099.88159, 448.931, 648.997375)).Magnitude <= 10
							end
						elseif game:GetService("Players").LocalPlayer.Data.Level.Value >= 800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress","Bartilo") == 2 then
							repeat TP(CFrame.new(-1850.49329, 13.1789551, 1750.89685)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-1850.49329, 13.1789551, 1750.89685)).Magnitude <= 10
							wait(1)
							repeat TP(CFrame.new(-1858.87305, 19.3777466, 1712.01807)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-1858.87305, 19.3777466, 1712.01807)).Magnitude <= 10
							wait(1)
							repeat TP(CFrame.new(-1803.94324, 16.5789185, 1750.89685)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-1803.94324, 16.5789185, 1750.89685)).Magnitude <= 10
							wait(1)
							repeat TP(CFrame.new(-1858.55835, 16.8604317, 1724.79541)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-1858.55835, 16.8604317, 1724.79541)).Magnitude <= 10
							wait(1)
							repeat TP(CFrame.new(-1869.54224, 15.987854, 1681.00659)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-1869.54224, 15.987854, 1681.00659)).Magnitude <= 10
							wait(1)
							repeat TP(CFrame.new(-1800.0979, 16.4978027, 1684.52368)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-1800.0979, 16.4978027, 1684.52368)).Magnitude <= 10
							wait(1)
							repeat TP(CFrame.new(-1819.26343, 14.795166, 1717.90625)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-1819.26343, 14.795166, 1717.90625)).Magnitude <= 10
							wait(1)
							repeat TP(CFrame.new(-1813.51843, 14.8604736, 1724.79541)) wait() until not _G.AutoBartilo or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-1813.51843, 14.8604736, 1724.79541)).Magnitude <= 10
						end
					end 
				end
			end)
		end)
	end
		
		if World3 then
		Quest:Toggle("Auto Open Color Haki",_G.Farm_Ob_Color,function(vu)
		_G.Farm_Ob_Color = vu
		StopTween(_G.Farm_Ob_Color)
		end)
		
	spawn(function()
		while wait() do
			pcall(function()
				if _G.Farm_Ob_Color then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("activateColor","Winter Sky")
					wait(0.5)
					repeat TP(CFrame.new(-5420.16602, 1084.9657, -2666.8208)) wait() 
					until _G.StopTween == true or _G.Farm_Ob_Color == false or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-5420.16602, 1084.9657, -2666.8208)).Magnitude <= 10
					wait(0.5)
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("activateColor","Pure Red")
					wait(0.5)
					repeat TP(CFrame.new(-5414.41357, 309.865753, -2212.45776)) wait() 
					until _G.StopTween == true or _G.Farm_Ob_Color == false or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-5414.41357, 309.865753, -2212.45776)).Magnitude <= 10
					wait(0.5)
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("activateColor","Snow White")
					wait(0.5)
					repeat TP(CFrame.new(-4971.47559, 331.565765, -3720.02954)) wait() 
					until _G.StopTween == true or _G.Farm_Ob_Color == false or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-Vector3.new(-4971.47559, 331.565765, -3720.02954)).Magnitude <= 10
					wait(0.5)
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "finish"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				end
			end) 
		end
	end)
	
		if World3 then
			Quest:Toggle("Auto Quest Soul Guitar",_G.AutoQuestSoulGuitar,function(value)
			_G.AutoQuestSoulGuitar = value
		StopTween(_G.AutoQuestSoulGuitar)
		end)
	
	spawn(function()
		while wait() do
			pcall(function()
				if _G.AutoQuestSoulGuitar then
					if GetWeaponInventory("Soul Guitar") == false then
						if (CFrame.new(-9681.458984375, 6.139880657196045, 6341.3720703125).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 5000 then
							if game:GetService("Workspace").NPCs:FindFirstChild("Skeleton Machine") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("soulGuitarBuy",true)
							else
								if game:GetService("Workspace").Map["Haunted Castle"].Candle1.Transparency == 0 then
									if game:GetService("Workspace").Map["Haunted Castle"].Placard1.Left.Part.Transparency == 0 then
										Quest2 = true
										repeat wait() TP(CFrame.new(-8762.69140625, 176.84783935546875, 6171.3076171875)) until (CFrame.new(-8762.69140625, 176.84783935546875, 6171.3076171875).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.Settings.Main["Auto Quest Soul Guitar"]
										wait(1)
										fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard7.Left.ClickDetector)
										wait(1)
										fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard6.Left.ClickDetector)
										wait(1)
										fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard5.Left.ClickDetector)
										wait(1)
										fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard4.Right.ClickDetector)
										wait(1)
										fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard3.Left.ClickDetector)
										wait(1)
										fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard2.Right.ClickDetector)
										wait(1)
										fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard1.Right.ClickDetector)
										wait(1)
									elseif game:GetService("Workspace").Map["Haunted Castle"].Tablet.Segment1:FindFirstChild("ClickDetector") then
										if game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part1:FindFirstChild("ClickDetector") then
											Quest4 = true
											repeat wait() TP(CFrame.new(-9553.5986328125, 65.62338256835938, 6041.58837890625)) until (CFrame.new(-9553.5986328125, 65.62338256835938, 6041.58837890625).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.Settings.Main["Auto Quest Soul Guitar"]
											wait(1)
											TP(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part3.CFrame)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part3.ClickDetector)
											wait(1)
											TP(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part4.CFrame)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part4.ClickDetector)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part4.ClickDetector)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part4.ClickDetector)
											wait(1)
											TP(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part6.CFrame)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part6.ClickDetector)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part6.ClickDetector)
											wait(1)
											TP(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part8.CFrame)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part8.ClickDetector)
											wait(1)
											TP(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part10.CFrame)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part10.ClickDetector)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part10.ClickDetector)
											wait(1)
											fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part10.ClickDetector)
										else
											Quest3 = true
										end
									else
										if game:GetService("Workspace").NPCs:FindFirstChild("Ghost") then
											local args = {
												[1] = "GuitarPuzzleProgress",
												[2] = "Ghost"
											}
	
											game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
										end
										if game.Workspace.Enemies:FindFirstChild("Living Zombie [Lv. 2000]") then
											for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
												if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
													if v.Name == "Living Zombie [Lv. 2000]" then
														EquipWeapon(_G.SelectWeapon)
														v.HumanoidRootPart.Size = Vector3.new(60,60,60)
														v.HumanoidRootPart.Transparency = 1
														v.Humanoid.JumpPower = 0
														v.Humanoid.WalkSpeed = 0
														v.HumanoidRootPart.CanCollide = false
														v.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,20,0)
														TP(CFrame.new(-10160.787109375, 138.6616973876953, 5955.03076171875))
														game:GetService'VirtualUser':CaptureController()
														game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
													end
												end
											end
										else
											TP(CFrame.new(-10160.787109375, 138.6616973876953, 5955.03076171875))
										end
									end
								else    
									if string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("gravestoneEvent",2), "Error") then
										local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
										local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
										wait(1)
										Notification:Notify(
											{Title = "Pado Hub", Description = "Go to Grave."},
											{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
										)
	
										TP(CFrame.new(-8653.2060546875, 140.98487854003906, 6160.033203125))
									elseif string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("gravestoneEvent",2), "Nothing") then
                		          local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
	                              local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
	                              wait(1)
	                              Notification:Notify(
	                              {Title = "Pado Hub", Description = "Wait Next Night."},
	                         	  {OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
	                             )
									else
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("gravestoneEvent",2,true)
									end
								end
							end
						else
							TP(CFrame.new(-9681.458984375, 6.139880657196045, 6341.3720703125))
						end
					end
				end
			end)
		end
	end)
	end
	
		if World3 then
			Quest:Toggle("Auto Dough King",_G.Auto_Open_Dough_Dungeo,function(value)
				if _G.SelectWeapon == nil then
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
						{Title = "Pado Hub", Description = "Select Weapon"},
						{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
					)
				else
			_G.Auto_Open_Dough_Dungeon = value
			StopTween(_G.Auto_Open_Dough_Dungeon)
			end
			end)
			
			spawn(function()
				while wait() do
					if _G.Auto_Open_Dough_Dungeon then
						pcall(function()
						if game.Players.LocalPlayer.Backpack:FindFirstChild("God's Chalice") or game.Players.LocalPlayer.Character:FindFirstChild("God's Chalice") then
							if string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SweetChaliceNpc"),"Where") then
								local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
								local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
								wait(1)
								Notification:Notify(
									{Title = "Pado Hub", Description = "Not Have Enough Material"},
									{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
								)								
							else
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SweetChaliceNpc")
								end
							elseif game.Players.LocalPlayer.Backpack:FindFirstChild("Sweet Chalice") or game.Players.LocalPlayer.Character:FindFirstChild("Sweet Chalice") then
								if string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"),"Do you want to open the portal now?") then
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")
								else
									if game.Workspace.Enemies:FindFirstChild("Baking Staff [Lv. 2250]") or game.Workspace.Enemies:FindFirstChild("Head Baker [Lv. 2275]") or game.Workspace.Enemies:FindFirstChild("Cake Guard [Lv. 2225]") or game.Workspace.Enemies:FindFirstChild("Cookie Crafter [Lv. 2200]")  then
										for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do  
											if (v.Name == "Baking Staff [Lv. 2250]" or v.Name == "Head Baker [Lv. 2275]" or v.Name == "Cake Guard [Lv. 2225]" or v.Name == "Cookie Crafter [Lv. 2200]") and v.Humanoid.Health > 0 then
												repeat task.wait()
													AutoHaki()
													EquipWeapon(_G.SelectWeapon)
													StartCakeMagnetOwn = true
													v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)  
													POSCAKEOwn = v.HumanoidRootPart.CFrame
													TP(v.HumanoidRootPart.CFrame * Farm_Mode)
													game:GetService'VirtualUser':CaptureController()
													game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
												until _G.Auto_Open_Dough_Dungeon == false or game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") or not v.Parent or v.Humanoid.Health <= 0
											end
										end
									else
										StartCakeMagnetOwn = false
										TP(CFrame.new(-1820.0634765625, 210.74781799316406, -12297.49609375))
									end
								end						
							elseif game.ReplicatedStorage:FindFirstChild("Dough King [Lv. 2300] [Raid Boss]") or game:GetService("Workspace").Enemies:FindFirstChild("Dough King [Lv. 2300] [Raid Boss]") then
								if game:GetService("Workspace").Enemies:FindFirstChild("Dough King [Lv. 2300] [Raid Boss]") then
									for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do 
										if v.Name == "Dough King [Lv. 2300] [Raid Boss]" then
											repeat task.wait()
												AutoHaki()
												EquipWeapon(_G.SelectWeapon)
												v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
												v.HumanoidRootPart.CanCollide = false
												TP(v.HumanoidRootPart.CFrame * Farm_Mode)
												game:GetService'VirtualUser':CaptureController()
												game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
											until _G.Auto_Open_Dough_Dungeon == false or not v.Parent or v.Humanoid.Health <= 0
										end    
									end    
								else
									TP(CFrame.new(-2009.2802734375, 4532.97216796875, -14937.3076171875)) 
								end
							elseif game.Players.LocalPlayer.Backpack:FindFirstChild("Red Key") or game.Players.LocalPlayer.Character:FindFirstChild("Red Key") then
								local args = {
									[1] = "CakeScientist",
									[2] = "Check"
								}
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
							else
								if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
									if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text,"Diablo") or string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text,"Deandre") or string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text,"Urban") then
										if game:GetService("Workspace").Enemies:FindFirstChild("Diablo [Lv. 1750]") or game:GetService("Workspace").Enemies:FindFirstChild("Deandre [Lv. 1750]") or game:GetService("Workspace").Enemies:FindFirstChild("Urban [Lv. 1750]") then
											for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
												if v.Name == "Diablo [Lv. 1750]" or v.Name == "Deandre [Lv. 1750]" or v.Name == "Urban [Lv. 1750]" then
													if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
														repeat task.wait()
															AutoHaki()
															EquipWeapon(_G.SelectWeapon)
															v.HumanoidRootPart.CanCollide = false
															v.Humanoid.WalkSpeed = 0
															v.HumanoidRootPart.Size = Vector3.new(50,50,50)
															TP(v.HumanoidRootPart.CFrame * Farm_Mode)
															game:GetService("VirtualUser"):CaptureController()
															game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
															sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
														until _G.Auto_Open_Dough_Dungeon == false or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.Backpack:FindFirstChild("God's Chalice") or game.Players.LocalPlayer.Character:FindFirstChild("God's Chalice")
													end
												end
											end
										else
											if game:GetService("ReplicatedStorage"):FindFirstChild("Diablo [Lv. 1750]") then
												TP(game:GetService("ReplicatedStorage"):FindFirstChild("Diablo [Lv. 1750]").HumanoidRootPart.CFrame * Farm_Mode)
											elseif game:GetService("ReplicatedStorage"):FindFirstChild("Deandre [Lv. 1750]") then
												TP(game:GetService("ReplicatedStorage"):FindFirstChild("Deandre [Lv. 1750]").HumanoidRootPart.CFrame * Farm_Mode)
											elseif game:GetService("ReplicatedStorage"):FindFirstChild("Urban [Lv. 1750]") then
												TP(game:GetService("ReplicatedStorage"):FindFirstChild("Urban [Lv. 1750]").HumanoidRootPart.CFrame * Farm_Mode)
											end
										end                    
									end
								else
									wait(0.5)
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter")
								end
							end
						end)
					end
				end
			end)
			end
		
		Quest:Toggle("Auto Holy Torch",_G.HolyTorch,function(value)
		_G.HolyTorch = value
		StopTween(_G.HolyTorch)
		end)
		
		spawn(function()
			while wait() do
				if _G.HolyTorch then
					if game.ReplicatedStorage:FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") or game.Workspace.Enemies:FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") and game:GetService("Workspace").Map.Turtle.TushitaGate.TushitaGate.Transparency == 1 then
						if game.Players.LocalPlayer.Backpack:FindFirstChild("Holy Torch") then
							EquipWeapon("Holy Torch")
						elseif game.Players.LocalPlayer.Character:FindFirstChild("Holy Torch") then
							if game:GetService("Workspace").Map.Turtle.QuestTorches.Torch1.Particles.Main.Enabled ~= true then
								if (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch1.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
									HolyTorchtween = TP2(game:GetService("Workspace").Map.Turtle.QuestTorches.Torch1.Position,game:GetService("Workspace").Map.Turtle.QuestTorches.Torch1.CFrame)
								elseif (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch1.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
									if HolyTorchtween then
										HolyTorchtween:Stop()
									end
									game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Map.Turtle.QuestTorches.Torch1.CFrame
								end
							elseif game:GetService("Workspace").Map.Turtle.QuestTorches.Torch2.Particles.Main.Enabled ~= true then
								if (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch2.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
									HolyTorchtween = TP2(game:GetService("Workspace").Map.Turtle.QuestTorches.Torch2.Position,game:GetService("Workspace").Map.Turtle.QuestTorches.Torch2.CFrame)
								elseif (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch2.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
									if HolyTorchtween then
										HolyTorchtween:Stop()
									end
									game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Map.Turtle.QuestTorches.Torch2.CFrame
								end
							elseif game:GetService("Workspace").Map.Turtle.QuestTorches.Torch3.Particles.Main.Enabled ~= true then
								if (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch3.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
									HolyTorchtween = TP2(game:GetService("Workspace").Map.Turtle.QuestTorches.Torch3.Position,game:GetService("Workspace").Map.Turtle.QuestTorches.Torch3.CFrame)
								elseif (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch3.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
									if HolyTorchtween then
										HolyTorchtween:Stop()
									end
									game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Map.Turtle.QuestTorches.Torch3.CFrame
								end
							elseif game:GetService("Workspace").Map.Turtle.QuestTorches.Torch4.Particles.Main.Enabled ~= true then
								if (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch4.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
									HolyTorchtween = TP2(game:GetService("Workspace").Map.Turtle.QuestTorches.Torch4.Position,game:GetService("Workspace").Map.Turtle.QuestTorches.Torch4.CFrame)
								elseif (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch4.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
									if HolyTorchtween then
										HolyTorchtween:Stop()
									end
									game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Map.Turtle.QuestTorches.Torch4.CFrame
								end
							elseif game:GetService("Workspace").Map.Turtle.QuestTorches.Torch5.Particles.Main.Enabled ~= true then
								if (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch5.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 300 then
									HolyTorchtween = TP2(game:GetService("Workspace").Map.Turtle.QuestTorches.Torch5.Position,game:GetService("Workspace").Map.Turtle.QuestTorches.Torch5.CFrame)
								elseif (game:GetService("Workspace").Map.Turtle.QuestTorches.Torch5.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 300 then
									if HolyTorchtween then
										HolyTorchtween:Stop()
									end
									game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Map.Turtle.QuestTorches.Torch5.CFrame
								end
							end
						else
							game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Waterfall.SecretRoom.Room.Door.Door.Hitbox.CFrame
						end
					end
				end
			end
		end)
		end
		
		if World3 then
			Quest:Toggle("Auto Phoenix Advance Dungeon",_G.AutoAdvanceDungeon,function(value)
			_G.AutoAdvanceDungeon = value
			StopTween(_G.AutoAdvanceDungeon)
		end)
		
		spawn(function()
			while wait() do
				if _G.AutoAdvanceDungeon then
					pcall(function()
						if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird-Bird: Phoenix") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird-Bird: Phoenix") then
							if game.Players.LocalPlayer.Backpack:FindFirstChild(game.Players.LocalPlayer.Data.DevilFruit.Value) then
								if game.Players.LocalPlayer.Backpack:FindFirstChild(game.Players.LocalPlayer.Data.DevilFruit.Value).Level.Value >= 400 then
									TP(CFrame.new(-2812.76708984375, 254.803466796875, -12595.560546875))
									if (CFrame.new(-2812.76708984375, 254.803466796875, -12595.560546875).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 10 then
										wait(1.5)
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SickScientist","Check")
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SickScientist","Heal")
									end
								end
							elseif game.Players.LocalPlayer.Character:FindFirstChild(game.Players.LocalPlayer.Data.DevilFruit.Value) then
								if game.Players.LocalPlayer.Character:FindFirstChild(game.Players.LocalPlayer.Data.DevilFruit.Value).Level.Value >= 400 then
									TP(CFrame.new(-2812.76708984375, 254.803466796875, -12595.560546875))
									if (CFrame.new(-2812.76708984375, 254.803466796875, -12595.560546875).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 10 then
										wait(1.5)
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SickScientist","Check")
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SickScientist","Heal")
									end
								end
							end
						end
					end)
				end
			end
		end)
	end

		-- BringMonster
		
		spawn(function()
			while task.wait() do
				if setscriptable then
					setscriptable(game.Players.LocalPlayer, "SimulationRadius", true)
				end
				if sethiddenproperty then
					sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
				end
			end
		end)
	
		spawn(function()
			while task.wait() do
				pcall(function()
					if _G.BringMonster then
						CheckLevel()
						for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do 
								if _G.Auto_Farm_Level and StartMagnet and v.Name == Ms and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= _G.MagnitudeSpeed then
									v.HumanoidRootPart.CFrame = PosMon
									v.Humanoid.JumpPower = 0
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.Size = Vector3.new(60,60,60)
									v.HumanoidRootPart.Transparency = 1
									v.HumanoidRootPart.CanCollide = false
									v.Head.CanCollide = false
									if v.Humanoid:FindFirstChild("Animator") then
										v.Humanoid.Animator:Destroy()
									end
								end
								if _G.AutoFarmKaitan and StartMagnet and v.Name == Ms and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= _G.MagnitudeSpeed then
									v.HumanoidRootPart.CFrame = PosMon
									v.Humanoid.JumpPower = 0
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.Size = Vector3.new(60,60,60)
									v.HumanoidRootPart.Transparency = 1
									v.HumanoidRootPart.CanCollide = false
									v.Head.CanCollide = false
									if v.Humanoid:FindFirstChild("Animator") then
										v.Humanoid.Animator:Destroy()
									end
								end
								if _G.AutoEctoplasm and StartEctoplasmMagnet then
									if string.find(v.Name, "Ship") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - EctoplasmMon.Position).Magnitude <= _G.MagnitudeSpeed then
										v.HumanoidRootPart.CFrame = EctoplasmMon
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoRengoku and StartRengokuMagnet then
									if (v.Name == "Snow Lurker [Lv. 1375]" or v.Name == "Arctic Warrior [Lv. 1350]") and (v.HumanoidRootPart.Position - RengokuMon.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = RengokuMon
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoMusketeerHat and StartMagnetMusketeerhat then
									if v.Name == "Forest Pirate [Lv. 1825]" and (v.HumanoidRootPart.Position - MusketeerHatMon.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = MusketeerHatMon
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.Auto_EvoRace and StartEvoMagnet then
									if v.Name == "Zombie [Lv. 950]" and (v.HumanoidRootPart.Position - PosMonEvo.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = PosMonEvo
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoBartilo and AutoBartiloBring then
									if v.Name == "Swan Pirate [Lv. 775]" and (v.HumanoidRootPart.Position - PosMonBarto.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = PosMonBarto
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoFarmFruitMastery and StartMasteryFruitMagnet then
									if v.Name == "Monkey [Lv. 14]" then
										if (v.HumanoidRootPart.Position - PosMonMasteryFruit.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											v.HumanoidRootPart.CFrame = PosMonMasteryFruit
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(60,60,60)
											v.HumanoidRootPart.Transparency = 1
											v.HumanoidRootPart.CanCollide = false
											v.Head.CanCollide = false
											if v.Humanoid:FindFirstChild("Animator") then
												v.Humanoid.Animator:Destroy()
											end
										end
									elseif v.Name == "Factory Staff [Lv. 800]" then
										if (v.HumanoidRootPart.Position - PosMonMasteryFruit.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											v.HumanoidRootPart.CFrame = PosMonMasteryFruit
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(60,60,60)
											v.HumanoidRootPart.Transparency = 1
											v.HumanoidRootPart.CanCollide = false
											v.Head.CanCollide = false
											if v.Humanoid:FindFirstChild("Animator") then
												v.Humanoid.Animator:Destroy()
											end
										end
									elseif v.Name == Ms then
										if (v.HumanoidRootPart.Position - PosMonMasteryFruit.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											v.HumanoidRootPart.CFrame = PosMonMasteryFruit
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(60,60,60)
											v.HumanoidRootPart.Transparency = 1
											v.HumanoidRootPart.CanCollide = false
											v.Head.CanCollide = false
											if v.Humanoid:FindFirstChild("Animator") then
												v.Humanoid.Animator:Destroy()
											end
										end
									end
								end
								if _G.AutoFarmGunMastery and StartMasteryGunMagnet then
									if v.Name == "Monkey [Lv. 14]" then
										if (v.HumanoidRootPart.Position - PosMonMasteryGun.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											v.HumanoidRootPart.CFrame = PosMonMasteryGun
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(60,60,60)
											v.HumanoidRootPart.Transparency = 1
											v.HumanoidRootPart.CanCollide = false
											v.Head.CanCollide = false
											if v.Humanoid:FindFirstChild("Animator") then
												v.Humanoid.Animator:Destroy()
											end
										end
									elseif v.Name == "Factory Staff [Lv. 800]" then
										if (v.HumanoidRootPart.Position - PosMonMasteryGun.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											v.HumanoidRootPart.CFrame = PosMonMasteryGun
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(60,60,60)
											v.HumanoidRootPart.Transparency = 1
											v.HumanoidRootPart.CanCollide = false
											v.Head.CanCollide = false
											if v.Humanoid:FindFirstChild("Animator") then
												v.Humanoid.Animator:Destroy()
											end
										end
									elseif v.Name == Ms then
										if (v.HumanoidRootPart.Position - PosMonMasteryGun.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
											v.HumanoidRootPart.CFrame = PosMonMasteryGun
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(60,60,60)
											v.HumanoidRootPart.Transparency = 1
											v.HumanoidRootPart.CanCollide = false
											v.Head.CanCollide = false
											if v.Humanoid:FindFirstChild("Animator") then
												v.Humanoid.Animator:Destroy()
											end
										end
									end
								end
								if _G.Auto_Bone and StartMagnetBoneMon then
									if (v.Name == "Reborn Skeleton [Lv. 1975]" or v.Name == "Living Zombie [Lv. 2000]" or v.Name == "Demonic Soul [Lv. 2025]" or v.Name == "Posessed Mummy [Lv. 2050]") and (v.HumanoidRootPart.Position - PosMonBone.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = PosMonBone
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoDoughtBoss or _G.Auto_Spikey_Trident and StartCakeMagnet then
									if (v.Name == "Cookie Crafter [Lv. 2200]" or v.Name == "Cake Guard [Lv. 2225]" or v.Name == "Baking Staff [Lv. 2250]" or v.Name == "Head Baker [Lv. 2275]") and (v.HumanoidRootPart.Position - POSCAKE.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = POSCAKE
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.Auto_Open_Dough_Dungeon and StartCakeMagnetOwn then
									if (v.Name == "Cookie Crafter [Lv. 2200]" or v.Name == "Cake Guard [Lv. 2225]" or v.Name == "Baking Staff [Lv. 2250]" or v.Name == "Head Baker [Lv. 2275]") and (v.HumanoidRootPart.Position - POSCAKEOwn.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = POSCAKEOwn
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoHearts and StartHeartsMagnet then
									if (v.Name == "Snow Demon [Lv. 2425]" or v.Name == "Candy Pirate [Lv. 2400]" or v.Name == "Candy Rebel [Lv. 2375]" or v.Name == "Sweet Thief [Lv. 2350]") and (v.HumanoidRootPart.Position - HeartsMon.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = HeartsMon
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoFarmCandy and StartCandyMagnet then
									if (v.Name == "Snow Demon [Lv. 2425]" or v.Name == "Candy Pirate [Lv. 2400]") and (v.HumanoidRootPart.Position - CandyMon.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
									v.HumanoidRootPart.CFrame = CandyMon
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoCandy and StartMagnetCandy then
									if (v.HumanoidRootPart.Position - PosMonCandy.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = PosMonCandy
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								  if _G.AutoMobAura and StartMagnetKill then
									if (v.HumanoidRootPart.Position - PosMonAura.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = PosMonAura
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								  if _G.Raid and StartMagnetRaid then
									if (v.HumanoidRootPart.Position - PosMonRaid.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = PosMonRaid
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoFarmMaterial and StartMagnetMaterial then
									if v.Name == MMon and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= _G.MagnitudeSpeed then
										v.HumanoidRootPart.CFrame = MatPos
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
								if _G.AutoFarmtribe and StarttribeMagnet then
									if (v.HumanoidRootPart.Position - tribeMon.Position).Magnitude <= _G.MagnitudeSpeed and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										v.HumanoidRootPart.CFrame = tribeMon
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.Size = Vector3.new(60,60,60)
										v.HumanoidRootPart.Transparency = 1
										v.HumanoidRootPart.CanCollide = false
										v.Head.CanCollide = false
										if v.Humanoid:FindFirstChild("Animator") then
											v.Humanoid.Animator:Destroy()
										end
									end
								end
							end
						end
					end)
				end
			end)				
	
		  AutoMisc:Seperator("Others")
				
		_G.FastAttack = true
		AutoMisc:Toggle("Fast Attack",_G.FastAttack,function(value)
			_G.FastAttack = value
		end)
	
				spawn(function()
					while wait() do
						pcall(function()
							if _G.FastAttack then
									require(game.ReplicatedStorage.Util.CameraShaker):Stop()
									local padosen = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework)
									local pado = debug.getupvalues(padosen)[2]
									spawn(function()
										if _G.FastAttack then
											if typeof(pado) == "table" then
												pcall(function()
														pado.activeController.timeToNextAttack = 0
														pado.activeController.hitboxMagnitude = 70
													    pado.activeController.DamageIndicator = 3
														pado.activeController.Hit = 0
														pado.activeController.Block = 0
														pado.activeController.attacking = false
														pado.activeController.blocking = false
														pado.activeController.active = false
														pado.activeController.focusStart = 0
														pado.activeController.increment = 4
														pado.activeController.humanoid.AutoRotate = 50
													end)
												end
											end
										end)
									end
								end)
							end
						end)

		AutoMisc:Toggle("Magnet",true,function(value)
				_G.BringMonster = value
			end)				
	
						AutoMisc:Toggle("Camera Shaker",false,function(value)
							_G.CameraShaker = value
						end)
					
						AutoMisc:Toggle("Disabled Damage",false,function(value)
							_G.DisabledDamage = value
						end)
					
					local CombatFramework = require(game:GetService("Players").LocalPlayer.PlayerScripts:WaitForChild("CombatFramework"))
					local CombatFrameworkR = getupvalues(CombatFramework)[2]
					local RigController = require(game:GetService("Players")["LocalPlayer"].PlayerScripts.CombatFramework.RigController)
					local RigControllerR = getupvalues(RigController)[2]
					local realbhit = require(game.ReplicatedStorage.CombatFramework.RigLib)
					local cooldownfastattack = tick()
					
						spawn(function()
							while wait() do
								pcall(function()
									if _G.DisabledDamage then
										game.Players.LocalPlayer.PlayerGui.Main.DmgCounter.Text.Visible = false
										game.Players.LocalPlayer.PlayerGui.Main.DmgCounter.BarFrame.Visible = false 
									else
										game.Players.LocalPlayer.PlayerGui.Main.DmgCounter.Text.Visible = true
										game.Players.LocalPlayer.PlayerGui.Main.DmgCounter.BarFrame.Visible = true 
									end
								end)
							end
						end)
					
						spawn(function()
							pcall(function()
								while wait() do
									local Camera = require(game.Players.LocalPlayer.PlayerScripts.CombatFramework.CameraShaker)
										if _G.CameraShaker then
											Camera.CameraShakeInstance.CameraShakeState.Inactive = 0
										else
											Camera.CameraShakeInstance.CameraShakeState.Inactive = 3
										end
									end
								end)
							end)
	
		AutoMisc:Toggle("Invisble Mob",false,function(value)
			_G.inv = value
			while _G.inv do wait()
				pcall(function()
		for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
			if v.ClassName == "MeshPart" then
			v.Transparency = 1
		end
		end
		for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
			if v.Name == "Head" then
			v.Transparency = 1
		end
		end
			for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
				if v.ClassName == "Accessory" then
					v.Handle.Transparency = 1
				end
			end
			for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
				if v.ClassName == "Decal" then
				v.Transparency = 1
				end
		end
		end)
		end
		end)
		
		 AutoMisc:Toggle("White Screen",_G.WhiteScreen,function(value)
			_G.WhiteScreen = value
		if _G.WhiteScreen  then
			game:GetService("RunService"):Set3dRenderingEnabled(false)
		else
			game:GetService("RunService"):Set3dRenderingEnabled(true)
		end
		end)
		
		AutoMisc:Toggle("Black Screen",_G.BlackScreen,function(value)
			_G.BlackScreen = value
		end)
		
		spawn(function()
			while wait() do
	        	if _G.BlackScreen then
			        game:GetService("Players").LocalPlayer.PlayerGui.Main.Blackscreen.Size = UDim2.new(500, 0, 500, 500)
			    else
			     	game:GetService("Players").LocalPlayer.PlayerGui.Main.Blackscreen.Size = UDim2.new(1, 0, 500, 500)
				end
			end
		end)

			AutoMisc:Toggle("Remove Effect Death",_G.Remove_EffectDeath,function(value)
			 _G.Remove_EffectDeath = value
			end)
		
			spawn(function()
				pcall(function()
					while wait() do
						if _G.Remove_EffectDeath then
							for i, v in pairs(game:GetService("ReplicatedStorage").Effect.Container:GetChildren()) do
								if v.Name == "Death" then
									v:Destroy()
								end
							end
						end
					end
				end)
			end)
	
		AutoMisc:Toggle("Remove Notification Death",false,function(value)
			if value == true then
				game:GetService("Players").LocalPlayer.PlayerGui.Notifications.Enabled = false
			else          
				game:GetService("Players").LocalPlayer.PlayerGui.Notifications.Enabled = true
			end
		end)
		
			AutoMisc:Toggle("Remove Sound",_G.Remove_Sound,function(value)
				_G.Remove_Sound = value
			end)
		
		spawn(function()
			game:GetService('RunService').Stepped:Connect(function()
				if _G.Remove_Sound then
					for i, v in pairs(game.Workspace["_WorldOrigin"]:GetChildren()) do
						if v.Name == "CurvedRing" or v.Name == "SwordSlash" or v.Name == "Sounds" or v.Name == "SlashHit" or v.Name == "DamageCounter" or v.Name == "eff" or v.Name == "Comm" then
							v:Destroy() 
						end
					end
				end
			end)
		end)
	
		  AutoMisc:Toggle("Remove Attack",_G.RemoveAnimation,function(value)
				 _G.RemoveAnimation = value
			end)
		
				local Client = game.Players.LocalPlayer
				local STOP = require(Client.PlayerScripts.CombatFramework.Particle)
				local STOPRL = require(game:GetService("ReplicatedStorage").CombatFramework.RigLib)
				if not shared.orl then
				shared.orl = STOPRL.wrapAttackAnimationAsync
				end
				if not shared.cpc then
				shared.cpc = STOP.play 
				end
				spawn(function()
				game:GetService("RunService").Stepped:Connect(function()
					STOPRL.wrapAttackAnimationAsync = function(a,b,c,d,func)
						local Hits = STOPRL.getBladeHits(b,c,d)
						if Hits then
							if _G.RemoveAnimation or _G.Auto_Farm_Level then
								STOP.play = function() end
								a:Play(0.01,0.01,0.01)
								func(Hits)
								STOP.play = shared.cpc
								wait(a.length * 0.5)
								a:Stop()
							else
								func(Hits)
								STOP.play = shared.cpc
								wait(a.length * 0.5)
								a:Stop()
							end
						end
					end
				end)
			end)

			AutoMisc:Toggle("Auto Set Spawn Points",false,function(value)
				_G.AutoSetSpawn = value
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.AutoSetSpawn then
							if game:GetService("Players").LocalPlayer.Character.Humanoid.Health > 0 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
							end
						end
					end
				end)
			end)

					AutoMisc:Seperator("Codes")
			
					local x2Code = {
						"FUDD10",
						"BIGNEWS",
						"THEGREATACE",
						"SUB2GAMERROBOT_EXP1",
						"StrawHatMaine",
						"Sub2OfficialNoobie",
						"SUB2NOOBMASTER123",
						"Sub2Daigrock",
						"Axiore",
						"TantaiGaming",
						"JCWK",
						"Starcodeheo",
						"Sub2Fer999",
						"Magicbus",
						"Enyu_is_Pro",
						"Bluxxy",
						"fudd10_v2",
						"3BVISITS",
						"KittGaming",
						"SUB2GAMERROBOT_RESET1",
						"GAMERROBOT_YT",
						"Sub2UncleKizaru",
						"UPD16",
						"UPD15",
						"GAMER_ROBOT_1M",
					   }
				
					   AutoMisc:Button("Redeem All Codes",function()
						function RedeemCode(value)
							game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(value)
						end
						for i,v in pairs(x2Code) do
							RedeemCode(v)
						end
					end)
					
					AutoMisc:Dropdown("Selected Codes",{"FUDD10","KittGaming","BIGNEWS","THEGREATACE","SUB2GAMERROBOT_EXP1","StrawHatMaine","Sub2OfficialNoobie","SUB2NOOBMASTER123","Sub2Daigrock","Axiore","TantaiGaming","JCWK","Starcodeheo","Sub2Fer999","Magicbus","Enyu_is_Pro","Bluxxy","fudd10_v2","3BVISITS","SUB2GAMERROBOT_RESET1","GAMERROBOT_YT","Sub2UncleKizaru","UPD16","UPD15","GAMER_ROBOT_1M"},function(value)
						_G.CodeSelect = value
					end)
					
					AutoMisc:Button("Redeem Code",function()
						game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(_G.CodeSelect)
					end)
	
					AutoMisc:Seperator("Mob Aura")
		
					_G.DistanceMobAura = 1000
					AutoMisc:Slider("Distance",1,10000,1000,function(value)
						_G.DistanceMobAura = value
					end)
	
					_G.URL = "" 
					AutoMisc:Seperator("Webhook")
				
					AutoMisc:Textbox("Webhook Link","Type You Link",function(t)
					_G.URL = t
					end)
				
						AutoMisc:Button("Webhook",function()
				local exploits = identifyexecutor()
				local text = "Level:"..game:GetService("Players").LocalPlayer.Data.Level.Value.."\nBeli:"..game:GetService("Players").LocalPlayer.Data.Beli.Value.."\nFragments:"..game:GetService("Players").LocalPlayer.Data.Fragments.Value.."\nEXP:"..game:GetService("Players").LocalPlayer.Data.Exp.Value.."\nSpawnPoint:"..game:GetService("Players").LocalPlayer.Data.LastSpawnPoint.Value.."\n DevilFruit: "..game:GetService("Players").LocalPlayer.Data.DevilFruit.Value.."\n Bounty/Honor: "..game:GetService("Players").LocalPlayer.leaderstats["Bounty/Honor"].Value.."\n Points: "..game:GetService("Players").LocalPlayer.Data.Points.Value.."\n Race : "..game:GetService("Players").LocalPlayer.Data.Race.Value.."\n Game Name : "..game:GetService("MarketplaceService"):GetProductInfo(game.PlaceId).Name
				local url = _G.URL
				local data = {
				   ["content"] = "",
				   ["embeds"] = {
					   {
						   ["title"] = "New Information", 
						   ["description"] = "Username: " ..game.Players.LocalPlayer.Name.. " \n" ..text,
						   ["type"] = "rich",
						   ["color"] = tonumber(0x7269da),
						   ["image"] = {
							   ["url"] = "http://www.roblox.com/Thumbs/Avatar.ashx?x=150&y=150&Format=Png&username=" ..
								   tostring(game:GetService("Players").LocalPlayer.Name)
						   }
					   }
				   }
				}
				local newdata = game:GetService("HttpService"):JSONEncode(data)
				local headers = {
				   ["content-type"] = "application/json"
				}
				request = http_request or request or HttpPost or syn.request
				local abcdef = {Url = url, Body = newdata, Method = "POST", Headers = headers}
				request(abcdef)
				end)
		
					AutoMisc:Toggle("Send\nYou Informations Every 60 Seconds",_G.SendWeb,function(value)
						_G.SendWeb = value
					end)
				
					 spawn(function()
						while wait(60) do
							if _G.SendWeb then			
				local exploits = identifyexecutor()
				local text = "Level:"..game:GetService("Players").LocalPlayer.Data.Level.Value.."\nBeli:"..game:GetService("Players").LocalPlayer.Data.Beli.Value.."\nFragments:"..game:GetService("Players").LocalPlayer.Data.Fragments.Value.."\nEXP:"..game:GetService("Players").LocalPlayer.Data.Exp.Value.."\nSpawnPoint:"..game:GetService("Players").LocalPlayer.Data.LastSpawnPoint.Value.."\n DevilFruit: "..game:GetService("Players").LocalPlayer.Data.DevilFruit.Value.."\n Bounty/Honor: "..game:GetService("Players").LocalPlayer.leaderstats["Bounty/Honor"].Value.."\n Points: "..game:GetService("Players").LocalPlayer.Data.Points.Value.."\n Race : "..game:GetService("Players").LocalPlayer.Data.Race.Value.."\n Game Name : "..game:GetService("MarketplaceService"):GetProductInfo(game.PlaceId).Name
				local url = _G.URL
				  
				  local data = {
				   ["content"] = "",
				   ["embeds"] = {
					   {
						   ["title"] = "New Information", 
						   ["description"] = "Username: " ..game.Players.LocalPlayer.DisplayName.. "                                               " ..text,
						   ["type"] = "rich",
						   ["color"] = tonumber(0x7269da),
						   ["image"] = {
							   ["url"] = "http://www.roblox.com/Thumbs/Avatar.ashx?x=150&y=150&Format=Png&username=" ..
								   tostring(game:GetService("Players").LocalPlayer.Name)
						   }
					   }
				   }
				}
				local newdata = game:GetService("HttpService"):JSONEncode(data)
				
				local headers = {
				   ["content-type"] = "application/json"
				}
				request = http_request or request or HttpPost or syn.request
				local abcdef = {Url = url, Body = newdata, Method = "POST", Headers = headers}
				request(abcdef)
					   end
					end
				end)		
	
		AutoMisc:Seperator("Jobid")
	
		AutoMisc:Button("Copy Jobid",function()
			setclipboard(tostring(game.JobId))
		end)
	
		AutoMisc:Textbox("join jobid Link","Type You Link",function(t)
			_G.joinjobid = t
		end)
	
		_G.joinjobid = ""
	
		AutoMisc:Button("Join",function()
			game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId,_G.joinjobid)
		end)
	
		AutoMisc:Seperator("Distance Magnitude Farm Settings")
		
		_G.MagnitudeSpeed = 200
	
		AutoMisc:Slider("Magnitude Farm",1,350,200,function(value)
			_G.MagnitudeSpeed = value
		end)
		
		AutoMisc:Seperator("Distance Tween Speed Farm Settings")
		
		_G.TweenSpeed = 260
	
		AutoMisc:Slider("Tween Speed Farm",1,350,260,function(value)
			_G.TweenSpeed = value
		end)
			
		AutoMisc:Seperator("Distance X/Y/Z Settings")
		
		getgenv().Y = 40

		AutoMisc:Slider("(X)",1,60,0,function(value)
			getgenv().X = value
		end)
		
		AutoMisc:Slider("(Y)",1,60,40,function(value)
			getgenv().Y = value
		end)
		
		AutoMisc:Slider("(Z)",1,60,0,function(value)
			getgenv().Z = value
		end)
	
		  AutoMisc:Seperator("List Mastery Skill Fruit")
			
			AutoMisc:Toggle("Skill Z",true,function(value)
				_G.SkillZ = value
			end)
			
			AutoMisc:Toggle("Skill X",true,function(value)
				_G.SkillX = value
			end)
			
			AutoMisc:Toggle("Skill C",true,function(value)
				_G.SkillC = value
			end)
			
			AutoMisc:Toggle("Skill V",true,function(value)
				_G.SkillV = value
			end)
		
			AutoMisc:Toggle("Skill F",true,function(value)
				_G.SkillF = value
			end)
		
		  AutoMisc:Seperator("List Mastery Skill Gun")
			
			AutoMisc:Toggle("Skill Z",true,function(value)
				_G.SkillGunZ = value
			end)
			
			AutoMisc:Toggle("Skill X",true,function(value)
				_G.SkillGunX = value
			end)
		
		  AutoMisc:Seperator("List Mastery Heath %")
	
		_G.Kill_At = 60
		AutoMisc:Slider("Kill At %",1,100,60,function(value)
			_G.Kill_At = value
		end)
	
		AutoMisc:Seperator("Lock Function")
		
			_G.LockLevel = false
			_G.LockBeli = false
			_G.LockFragments = false
			_G.Levelclose = 2450
			_G.LevelcloseBeli = 1000000
			_G.LevelcloseFragments = 1000000
			_G.Lock_Candy = 100000
			_G.Lock_Bone = 100000
		
			AutoMisc:Toggle("Lock Level",false,function(value)
				_G.LockLevel = value
			end)
		
			spawn(function()
				while wait() do
					if _G.LockLevel then
						if game.Players.localPlayer.Data.Level.Value >= LockLevelValue then
							game.Players.localPlayer:Kick("Level Lock OFF")
						end
					end
				end
			end)
			
		LockLevelValue = 2450
		OldLevel = game.Players.localPlayer.Data.Level.Value
		AutoMisc:Slider("Select Level Lock Farm",1,LockLevelValue,LockLevelValue,nil,function(value)
			LockLevelValue = value
		end)
		
			AutoMisc:Toggle("Lock Beli",false,function(value)
				_G.LockBeli = value
			end)
		
			spawn(function()
				while wait() do
					if _G.Open_LockBone then
						if Boneremote() == _G.Lock_Bone then
							game.Players.LocalPlayer:Kick("Lock Bone Success")
						end
					end
				end
			end)
		
			AutoMisc:Slider("Beli Lock",0,_G.LevelcloseBeli,100000,function(value)
				_G.LevelcloseBeli = value
			end)
		
			AutoMisc:Toggle("Lock Fragments",false,function(value)
				_G.LockFragments = value
			end)
		
			AutoMisc:Slider("Fragments Lock",0,_G.LevelcloseFragments,_G.LevelcloseFragments,100000,function(value)
				_G.LevelcloseFragments = value
			end)
		
			function Boneremote()
				return game:GetService("ReplicatedStorage").Remotes["CommF_"]:InvokeServer("Bones","Check")
			end
	
			function Boneremote()
				return game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Candies","Check")
			end
	
			AutoMisc:Toggle("Lock Bone",false,function(vv)
				_G.Open_LockBone = vv
			end)
		
			AutoMisc:Slider("Lock Bone",1,100000,100,_G.Lock_Bone,_G.Lock_Bone,function(value)
				_G.Lock_Bone = value
			end)
		
			AutoMisc:Toggle("Lock Candy",false,function(vu)
				_G.Open_LockCandy = vu
			end)
			
			spawn(function()
				while wait() do
					if _G.Open_LockCandy then
						if Boneremote() == _G.Lock_Bone then
							game.Players.LocalPlayer:Kick("Lock Candy Success")
						end
					end
				end
			end)
		
			AutoMisc:Slider("Lock Candy",1,100000,100,_G.Lock_Candy,_G.Lock_Candy,function(value)
				_G.Lock_Candy = value
			end)
	
			if World1 or World2 then
				Race:Label("Do Not Race World First Sea and Second Sea ")
			end
	
				if World3 then
	
					Race:Seperator("Mirage Island")
					
					local FM = Race:Label('...')
					local Mirragecheck = Race:Label('...')
					
							spawn(function()
								while wait(.1) do
									pcall(function()
										if game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709149431" then
											FM:Set("🌑 : Full Moon 100%")
										elseif game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709149052" then
											FM:Set("🌒 : Full Moon 75%")
										elseif game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709143733" then
											FM:Set("🌓 : Full Moon 50%")
										elseif game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709150401" then
											FM:Set("🌗 : Full Moon 25%")
										elseif game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709149680" then
											FM:Set("🌖 : Full Moon 15%")
										else
											FM:Set("🌚 : Full Moon 0%")
										end
									end)
								end
							end)
					
					spawn(function()
						pcall(function()
							while wait(.1) do
								if game.Workspace._WorldOrigin.Locations:FindFirstChild('Mirage Island') then
								  Mirragecheck:Set('🏝️ : Mirage Island is Spawning ✅')
								else
								  Mirragecheck:Set('🏝️ : Mirage Island Not Found ❌')
							   end
							end
						end)
					end)
	
					spawn(function()
						pcall(function()
							while wait(2) do
								if game.Workspace._WorldOrigin.Locations:FindFirstChild('Mirage Island') then
									Moon()
									break
								elseif game.ReplicatedStorage:FindFirstChild("Dough King [Lv. 2300] [Raid Boss]") then
									DoughKing()
									break
							   end
							end
						end)
					end)
	
					Race:Toggle("Auto Mirage Island",false,function(value)
					  _G.Mirage = value
					  StopTween(_G.Mirage)
					end)
		
					  Race:Toggle("Auto Mirage Island Hop",false,function(value)
					  _G.MirageHop = value
					  end)
					
					  Race:Toggle("Teleport To Gear",false,function(value)
					  TP(game:GetService("Workspace").Map.MysticIsland:FindFirstChildOfClass("MeshPart").CFrame)
					end)
					
					Race:Toggle("Mirage Island Notification",false,function(value)
					 _G.NotificationMirage = value
					end)

					Race:Toggle("Teleport NPC Shop",false,function()
						TP(game:GetService("Workspace").Map.MysticIsland.npcspawn:FindFirstChild("npcSpawn").CFrame)
					end)

					Race:Button("Remove Fog",function()
						game:GetService("Lighting").BaseAtmosphere:Destroy()
					end)

					Race:Button("Enabled Press W Button",function()
						game:GetService("VirtualInputManager"):SendKeyEvent(true,"W",false,game)
					end)
	
					Race:Button("Enabled Press E Button Lever Pull",function()
						Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(28286.35546875, 14895.3017578125, 102.62469482421875)
                        wait(1)
						TP(CFrame.new(28575.181640625, 14936.6279296875, 72.31636810302734))
						wait(5)
						game:GetService("VirtualInputManager"):SendKeyEvent(true,"E",false,game)
					end)
	
						spawn(function()
							pcall(function()
								while wait(1) do
									if _G.NotificationMirage then
									if game.Workspace._WorldOrigin.Locations:FindFirstChild('Mirage Island') then
										local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
										local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
										wait(1)
										Notification:Notify(
											{Title = "Pado Hub", Description = "Mirage Island is Spawning!"},
											{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
										)										
									end
								end
							end
						end)
					end)
					
					spawn(function()
							pcall(function()
								while wait(.1) do
								 if _G.Mirage then
								  if game:GetService("Workspace").Map:FindFirstChild("MysticIsland") then
									function toTargetWait(a)local b=(a.p-game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position).Magnitude;tweenrach=game:GetService('TweenService'):Create(game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart"),TweenInfo.new(b/250,Enum.EasingStyle.Linear),{CFrame=a})tweenrach:Play()end;toTargetWait(workspace.Map.MysticIsland.PrimaryPart.CFrame*CFrame.new(0,250,0))
									else
										local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
										local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
										wait(1)
										Notification:Notify(
											{Title = "Pado Hub", Description = "Mirage Not Found!"},
											{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
										)					
									if _G.MirageHop and not game:GetService("Workspace").Map:FindFirstChild("MysticIsland") then
									wait(6)
								Hop()
								end          
							end
						end
					end
					end)
					end)

					Race:Seperator("ESP")
	
					Race:Toggle("ESP Diamond Chest",DiamondChestESP,function(value)
						DiamondChestESP = value
						while DiamondChestESP do wait()
							UpdateDiamondChestESP() 
						end
					end)
	
					Race:Toggle("ESP Fragments Chest",FragChestESP,function(value)
						FragChestESP = value
						while FragChestESP do wait()
							UpdateFragChestESP() 
						end
					end)	
	
					Race:Toggle("ESP Npc Spawn",npcspawnESP,function(value)
						npcspawnESP = value
						while npcspawnESP do wait()
							UpdatenpcspawnESP() 
						end
					end)

					Race:Toggle("ESP Mirage Island",MirageIslandESP,function(a)
							MirageIslandESP = a
							   while MirageIslandESP do wait()
								UpdateMirageIslandChams() 
							end
						end)
	
				Race:Seperator("Race V4")
			
				Race:Toggle("Auto Hit and open tribe V4",false,function(value)
					_G.AutoFarmtribe = value
					StopTween(_G.AutoFarmtribe)
				end)

				spawn(function()
					while wait(.1) do
						pcall(function()
							if _G.AutoFarmtribe then
									 if game:GetService("Workspace").Enemies:FindFirstChild("Marine Commodore [Lv. 1700]") then
										for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
											 if v.Name == "Marine Commodore [Lv. 1700]" then
												 if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
												  repeat task.wait()
													AutoHaki()
													EquipWeapon(_G.SelectWeapon)
													tribeMon = v.HumanoidRootPart.CFrame
													StarttribeMagnet = true
													v.HumanoidRootPart.Size = Vector3.new(60,60,60)
													v.Humanoid.JumpPower = 0
													v.Humanoid.WalkSpeed = 0
													v.HumanoidRootPart.CanCollide = false
													v.Humanoid:ChangeState(11)
													TP(v.HumanoidRootPart.CFrame * Farm_Mode) 
													game:GetService("VirtualUser"):CaptureController()
													game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
													game:GetService("VirtualInputManager"):SendKeyEvent(true,"Y",false,game) 
												until not _G.AutoFarmtribe or v.Humanoid.Health <= 0 or not v.Parent or v.Humanoid.Health <= 0
											end
										end
									end
								else
									StarttribeMagnet = false
									TP(CFrame.new(2731.40479, 167.299362, -7935.44873, -0.755688131, 3.78607545e-08, 0.654931605, 3.15500799e-08, 1, -2.14048814e-08, -0.654931605, 4.48773152e-09, -0.755688131))
									 end
								end
							end)
						 end
					end)

				Race:Button("Teleport To the V tribe room",function()
					Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(28286.35546875, 14895.3017578125, 102.62469482421875)
				end)
	
				Race:Button("Teleport To Top Of GreatTree",function()
				  TP(CFrame.new(2947.556884765625, 2281.630615234375, -7213.54931640625))
				end)
					
				Race:Button("Teleport To Timple Of Time",function()
				  Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(28286.35546875, 14895.3017578125, 102.62469482421875)
				end)
					
				Race:Button("Teleport To Lever Pull",function()
				  TP(CFrame.new(28575.181640625, 14936.6279296875, 72.31636810302734))
				end)
			
				Race:Button("Teleport To Acient One (Must Be in Temple Of Time!)",function()
					TP(CFrame.new(28981.552734375, 14888.4267578125, -120.245849609375))
				end)
				   
				Race:Button("Unlock Lever.", function()
				if game:GetService("Workspace").Map["Temple of Time"].Lever.Prompt:FindFirstChild("ProximityPrompt") then
					game:GetService("Workspace").Map["Temple of Time"].Lever.Prompt:FindFirstChild("ProximityPrompt"):Remove()
				else
				--[[]]
				end
				wait(0.1)
				local ProximityPrompt = Instance.new("ProximityPrompt")
				ProximityPrompt.Parent = game:GetService("Workspace").Map["Temple of Time"].Lever.Prompt
				ProximityPrompt.MaxActivationDistance = 10
				ProximityPrompt.ActionText = "Secrets Beholds Inside"
				ProximityPrompt.ObjectText = "An unknown lever of time"
				
				function onProximity()
				local part = game:GetService("Workspace").Map["Temple of Time"].MainDoor1
				local TweenService = game:GetService("TweenService")
				
				local startPosition = part.Position
				local endPosition = startPosition + Vector3.new(0, -50, 0)
				
				local tweenInfo = TweenInfo.new(10, Enum.EasingStyle.Linear, Enum.EasingDirection.Out)
				local tween = TweenService:Create(part, tweenInfo, {Position = endPosition})
				
				tween:Play()
				
				local partnew = game:GetService("Workspace").Map["Temple of Time"].MainDoor2
				local TweenService = game:GetService("TweenService")
				
				local startPosition = partnew.Position
				local endPosition = startPosition + Vector3.new(0, -50, 0)
				
				local tweenInfo = TweenInfo.new(10, Enum.EasingStyle.Linear, Enum.EasingDirection.Out)
				local tween = TweenService:Create(partnew, tweenInfo, {Position = endPosition})
				
				tween:Play()
				
				local SoundSFX = Instance.new("Sound")
				SoundSFX.Parent = workspace
				SoundSFX.SoundId = "rbxassetid://1904813041"
				SoundSFX:Play()
				SoundSFX.Name = "POwfpxzxzfFfFF"
				game:GetService("Workspace").Map["Temple of Time"].Lever.Prompt:FindFirstChild("ProximityPrompt"):Remove()
				wait(5)
				workspace:FindFirstChild("POwfpxzxzfFfFF"):Remove()
				game:GetService("Workspace").Map["Temple of Time"].NoGlitching:Remove()
				game:GetService("Workspace").Map["Temple of Time"].NoGlitching:Remove()
				game:GetService("Workspace").Map["Temple of Time"].NoGlitching:Remove()
				end
				
				ProximityPrompt.Triggered:Connect(onProximity)
				end)
				
				Race:Button("Clock Acces.", function()
					game:GetService("Workspace").Map["Temple of Time"].DoNotEnter:Remove()
					game:GetService("Workspace").Map["Temple of Time"].ClockRoomExit:Remove()
				end)
				
				Race:Toggle("Disabled Inf Stairs", nil, function(value)
					game.Players.LocalPlayer.Character.InfiniteStairs.Disabled = value
				end)
				 
				Race:Button("Teleport Cyborg Door (Must Be in Temple Of Time!)",function()
				  TP(CFrame.new(28492.4140625, 14894.4267578125, -422.1100158691406))
				  end)
				  
				  Race:Button("Teleport Fish Door (Must Be in Temple Of Time!)",function()
				  TP(CFrame.new(28224.056640625, 14889.4267578125, -210.5872039794922))
				  end)
				  
				  Race:Button("Teleport Ghoul Door (Must Be in Temple Of Time!)",function()
				  TP(CFrame.new(28672.720703125, 14889.1279296875, 454.5961608886719))
				  end)
				  
				  Race:Button("Teleport Human Door (Must Be in Temple Of Time!)",function()
				  TP(CFrame.new(29237.294921875, 14889.4267578125, -206.94955444335938))
				  end)
				  
				  Race:Button("Teleport Mink Door (Must Be in Temple Of Time!)",function()
				  TP(CFrame.new(29020.66015625, 14889.4267578125, -379.2682800292969))
				  end)
				  
				  Race:Button("Teleport Sky Door (Must Be in Temple Of Time!)",function()
				  TP(CFrame.new(28967.408203125, 14918.0751953125, 234.31198120117188))
				  end)
				
				  Race:Seperator("Auto Trials")
	
				  Race:Button("Auto Complete Angel Trial",function(t)
				  game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.Map.SkyTrial.Model.FinishPart.CFrame
				  end)
				
				  Race:Button("Auto Complete Rabbit Trial",function(t)
				  game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.MinkTrial.Ceiling.CFrame * CFrame.new(0,-5,0)
				  end)
				
				  Race:Button("Auto Complete Cyborg Trial",function(t)
				  game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,300,0)
				  end)
				  
				  Race:Button("Teleport To Safe Zone When Pvp (Must Be in Temple Of Time!)",function()
				  TP(CFrame.new(28273.0859375, 14896.5078125, 157.42063903808594))
				  end)
				  
				  Race:Button("Teleport Pvp Zone (Must Be in Temple Of Time!)",function()
				  TP(CFrame.new(28766.681640625, 14967.1455078125, -164.13290405273438))
				end)
			end
	
			Combat:Seperator("Players")
	
			Playerslist = {}
			
			for i,v in pairs(game:GetService("Players"):GetChildren()) do
				table.insert(Playerslist,v.Name)
			end
			
			local SelectedPly = Combat:Dropdown("Select Players",Playerslist,function(value)
				_G.SelectPly = value
			end)
			
			Combat:Button("Refresh Player",function()
				Playerslist = {}
				SelectedPly:Clear()
				for i,v in pairs(game:GetService("Players"):GetChildren()) do  
					SelectedPly:Add(v.Name)
				end
			end)
			
			Combat:Toggle("Spectate Player",false,function(value)
				SpectatePlys = value
				local plr1 = game:GetService("Players").LocalPlayer.Character.Humanoid
				local plr2 = game:GetService("Players"):FindFirstChild(_G.SelectPly)
				repeat wait(.1)
					game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players"):FindFirstChild(_G.SelectPly).Character.Humanoid
				until SpectatePlys == false 
				game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players").LocalPlayer.Character.Humanoid
			end)
			
			Combat:Toggle("Teleport Tween",false,function(value)
				_G.TeleportPly = value
				pcall(function()
					if _G.TeleportPly then
						repeat TP(game:GetService("Players")[_G.SelectPly].Character.HumanoidRootPart.CFrame) task.wait() until _G.TeleportPly == false
					end
					StopTween(_G.TeleportPly)
				end)
			end)
		
			Combat:Toggle("Teleport Bypass",false,function(bool)
				_G.Teleport = bool
			if _G.Teleport == false then
				game.Players:FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.Size = Vector3.new(2, 2, 1)
			end
			while _G.Teleport do task.wait()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players:FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.CFrame * CFrame.new(0, 0, 0)
				end
			end)
		
			Combat:Seperator("body") 
		
			Combat:Slider("Jump Hight",0,400,50,function(Value)
					   game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value            
				   end)
		 
			Combat:Slider("Gravity",0,400,0, function(value)
					   workspace.Gravity = value
				   end)

			  Combat:Seperator("Float")
		
	Combat:Fly()
	
			  Combat:Seperator("Aimbot")
		
			  Combat:Toggle("Aimbot Skill",false,function(value)
				_G.Aimbot_Skill = value
			end)
			
			spawn(function()
				pcall(function()
					while task.wait() do
						if _G.Aimbot_Skill ~= nil and game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool") and game.Players.LocalPlayer.Character[game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool").Name]:FindFirstChild("MousePos") then
							local args = {
								[1] = game:GetService("Players"):FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.Position
							}
							game:GetService("Players").LocalPlayer.Character:FindFirstChild(game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool").Name).RemoteEvent:FireServer(unpack(args))
						end
					end
				end)
			end)
			
			Combat:Toggle("Aimbot Gun",false,function(value)
				_G.Aimbot_Gun = value
			end)
			
			spawn(function()
				while task.wait() do
					if _G.Aimbot_Gun and game:GetService("Players").LocalPlayer.Character:FindFirstChild(SelectWeaponGun) then
						pcall(function()
							game:GetService("Players").LocalPlayer.Character[SelectWeaponGun].Cooldown.Value = 0
							local args = {
								[1] = game:GetService("Players"):FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.Position,
								[2] = game:GetService("Players"):FindFirstChild(_G.SelectPly).Character.HumanoidRootPart
							}
							game:GetService("Players").LocalPlayer.Character[SelectWeaponGun].RemoteFunctionShoot:InvokeServer(unpack(args))
						end)
					end
				end
			end)
	

			  Combat:Toggle("Aim Lock",false,function(value)
				_G.AimLock  = value
			end)

			local camera = game.Workspace.CurrentCamera
			local localplayer = game:GetService("Players").LocalPlayer

			spawn(function()
				pcall(function()
					while wait() do
						if _G.AimLock then
							function closestplayer()
								local dist = _G.dist
								local target = nil 
								for i,v in pairs(game:GetService("Players"):GetPlayers()) do
									if v ~= localplayer then
										if v.Character and v.Character:FindFirstChild("Head") and _G.AimLock and v.Character.Humanoid.Health > 0 then --- creating the checks
											local magnitude = (v.Character.Head.Position - localplayer.Character.Head.Position).magnitude
												if magnitude < dist then
													dist = magnitude
													target = v
												end
											end
										end
									end
								return target
							end
						end
					end
				end)
			end)
	 
			game:GetService("RunService").RenderStepped:Connect(function()
				if _G.AimLock then
					camera.CFrame = CFrame.new(camera.CFrame.Position,closestplayer().Character.Head.Position) -- locks into the HEAD
				end
			end)

			_G.dist = 100

			Combat:Slider("Lock Magnitude",1,1000,100,function(value)
				_G.dist = value
			end)

		Combat:Toggle("Aim Bot Skill And Gun",false,function(value)
				_G.Aimvotskillgun  = value
			end)

			Combat:Toggle("Show Fov",false,function(value)
				_G.ShowFov = value
			end)
			
			_G.FOVSize = 200
			
			Combat:Slider("Fov Size",1,700,200,function(value)
				_G.FOVSize = value
			end)
			
			Combat:Slider("Fov Thickness",1,100,2,function(value)
				_G.Thicknessz = value
			end)

			local FOVCircle = Drawing.new("Circle")
			FOVCircle.Thickness = 1
			FOVCircle.NumSides = 460
			FOVCircle.Filled = false
			FOVCircle.Transparency = 0.5
			FOVCircle.Radius = 200
			FOVCircle.Color = Color3.fromRGB(255, 255, 255)
			
			game:GetService("RunService").Stepped:Connect(function()
				FOVCircle.Radius = _G.FOVSize
				FOVCircle.Thickness = _G.Thicknessz
				FOVCircle.NumSides = 55
				FOVCircle.Position = game:GetService('UserInputService'):GetMouseLocation()
				if _G.ShowFov then
					FOVCircle.Visible = true
				else
					FOVCircle.Visible = false
				end
			end)
			
			local lp = game:GetService('Players').LocalPlayer
			local mouse = lp:GetMouse()
			spawn(function()
				while wait() do
					if _G.Aimvotskillgun  then
						pcall(function()
							local MaxDist, Closest = math.huge
							for i,v in pairs(game:GetService("Players"):GetChildren()) do 
								local Head = v.Character:FindFirstChild("HumanoidRootPart")
								local Pos, Vis = game.Workspace.CurrentCamera.WorldToScreenPoint(game.Workspace.CurrentCamera, Head.Position)
								local MousePos, TheirPos = Vector2.new(mouse.X, mouse.Y), Vector2.new(Pos.X, Pos.Y)
								local Dist = (TheirPos - MousePos).Magnitude
								if Dist < MaxDist and Dist <= _G.FOVSize and v.Name ~= game.Players.LocalPlayer.Name then
									MaxDist = Dist
									_G.SelectAim  = v
								end
							end
						end)
					end
				end
			end)
			
			spawn(function()
				local gg = getrawmetatable(game)
				local old = gg.__namecall
				setreadonly(gg,false)
				gg.__namecall = newcclosure(function(...)
					local method = getnamecallmethod()
					local args = {...}
					if tostring(method) == "FireServer" then
						if tostring(args[1]) == "RemoteEvent" then
							if tostring(args[2]) ~= "true" and tostring(args[2]) ~= "false" then
								if _G.Aimvotskillgun  then
									args[2] = _G.SelectAim.Character.HumanoidRootPart.Position
									return old(unpack(args))
								end
							end
						end
					end
					return old(...)
				end)
			end)
	
			game:GetService('RunService').RenderStepped:connect(function()
			if _G.Disabled then
			for i,v in next, game:GetService('Players'):GetPlayers() do
			if v.Name ~= game:GetService('Players').LocalPlayer.Name then
			pcall(function()
			v.Character.HumanoidRootPart.Size = Vector3.new(_G.HeadSize,_G.HeadSize,_G.HeadSize)
			v.Character.HumanoidRootPart.Transparency = 1 
			v.Character.HumanoidRootPart.BrickColor = BrickColor.new("Really blue")
			v.Character.HumanoidRootPart.Material = "Smooth Plastic"
			v.Character.HumanoidRootPart.CanCollide = false
		end)
	end
	end
	end
	end)
	
	 _G.HeadSize = 1

			Combat:Toggle("Hitbox",false,function(value)
				_G.Disabled = value
			end)

			Combat:Slider("Hitbox Size",0,150,1,function(value)
				_G.HeadSize = value
			end)

			Combat:Seperator("PvP")
			
			Combat:Toggle("Enabled PvP",false,function(value)
				_G.EnabledPvP = value
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.EnabledPvP then
							if game:GetService("Players").LocalPlayer.PlayerGui.Main.PvpDisabled.Visible == true then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EnablePvP")
							end
						end
					end
				end)
			end)
		
		Combat:Toggle("Full Bright",nil,function(value)
		_G.FullBright = value
				if _G.FullBright then
					game:GetService("Lighting").Ambient = Color3.new(1, 1, 1)
					game:GetService("Lighting").ColorShift_Bottom = Color3.new(1, 1, 1)
					game:GetService("Lighting").ColorShift_Top = Color3.new(1, 1, 1)
				else
					game:GetService("Lighting").Ambient = Color3.new(0, 0, 0)
					game:GetService("Lighting").ColorShift_Bottom = Color3.new(0, 0, 0)
					game:GetService("Lighting").ColorShift_Top = Color3.new(0, 0, 0)
				end
		game.Lighting.Changed:connect(
			function()
				if _G.FullBright then
					game:GetService("Lighting").Ambient = Color3.new(1, 1, 1)
					game:GetService("Lighting").ColorShift_Bottom = Color3.new(1, 1, 1)
					game:GetService("Lighting").ColorShift_Top = Color3.new(1, 1, 1)
				else
					game:GetService("Lighting").Ambient = Color3.new(0, 0, 0)
					game:GetService("Lighting").ColorShift_Bottom = Color3.new(0, 0, 0)
					game:GetService("Lighting").ColorShift_Top = Color3.new(0, 0, 0)
				end
			end
		)
		end)
			
			 Combat:Button("Player Hunter",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PlayerHunter")
			end)
			
			Combat:Seperator("Bounty")
			
			Combat:Toggle("Auto Farm Bounty",_G.AutoFarmBounty,function(value)
				_G.AutoFarmBounty = value
				AutoFarmBounty()
				StopTween(_G.AutoFarmBounty)
			end)
		
			CastlePostoMansion = CFrame.new(-5084.8447265625, 316.48101806641, -3145.3752441406)
			MansiontoCastlePos = CFrame.new(-12464.596679688, 376.30590820312, -7567.2626953125)
			Castletophydra = CFrame.new(-5095.33984375, 316.48101806641, -3168.3134765625)
			HydratoCastle = CFrame.new(5741.869140625, 611.94750976562, -282.61154174805)
	
					function AutoFarmBounty()
						pcall(function()
							for i,v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
								if v.Name ~= game.Players.LocalPlayer.Name then
									if v:WaitForChild("Humanoid").Health > 0 and (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 17000 then
										plyselecthunthelpold = v.Humanoid.Health
										repeat task.wait()
											NameTarget = v.Name
											if tostring(game.Players.LocalPlayer.Team) == "Pirates" then
											TP(v.HumanoidRootPart.CFrame * Farm_Mode)
											if _G.AutoFarmBounty and (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 60 then
												game:service('VirtualInputManager'):SendKeyEvent(true, "Z", false, game)
												game:service('VirtualInputManager'):SendKeyEvent(false, "Z", false, game)
												if _G.AutoFarmBounty and (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 60 then
												game:service('VirtualInputManager'):SendKeyEvent(true, "X", false, game)
												game:service('VirtualInputManager'):SendKeyEvent(false, "X", false, game)
												if _G.AutoFarmBounty and (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 60 then
												game:service('VirtualInputManager'):SendKeyEvent(true, "C", false, game)
												game:service('VirtualInputManager'):SendKeyEvent(false, "C", false, game)
											end
										end
									end
										elseif tostring(game.Players.LocalPlayer.Team) == "Marines" then
									if game.Players[NameTarget].Team ~= game.Players.LocalPlayer.Team then
										TP(v.HumanoidRootPart.CFrame * Farm_Mode)
										if _G.AutoFarmBounty and (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 60 then
											game:service('VirtualInputManager'):SendKeyEvent(true, "Z", false, game)
											game:service('VirtualInputManager'):SendKeyEvent(false, "Z", false, game)
											if _G.AutoFarmBounty and (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 60 then
											game:service('VirtualInputManager'):SendKeyEvent(true, "X", false, game)
											game:service('VirtualInputManager'):SendKeyEvent(false, "X", false, game)
											if _G.AutoFarmBounty and (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 60 then
											game:service('VirtualInputManager'):SendKeyEvent(true, "C", false, game)
											game:service('VirtualInputManager'):SendKeyEvent(false, "C", false, game)
										end
									end
								end
							end
						end
							if game.Players.LocalPlayer.Character.Humanoid.Health > 0 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
							end
							if not game:GetService("Players").LocalPlayer.Character:FindFirstChild("HasBuso") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buso")
							end
							if game:GetService("Players").LocalPlayer.PlayerGui.Main.PvpDisabled.Visible == true then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EnablePvp")
							end
							game:GetService("Players").LocalPlayer.PlayerGui.Main.InCombat.Visible = false
							game:GetService("Players").LocalPlayer.PlayerGui.Main.SafeZone.Visible = false
							TargetSelectHunt = v.Humanoid
						until _G.AutoFarmBounty == false or v.Humanoid.Health == 0 or not v:FindFirstChild("HumanoidRootPart") or not v:FindFirstChild("Humanoid") or not v.Parent or NextplySelect == true
						NextplySelect = false
						StartCheckTarget = false
					end
				end
			end
		end)
	end
	
			spawn(function()
				pcall(function()
					while wait(.1) do
						if _G.AutoFarmBounty then
							if TargetSelectHunt ~= nil then
								if StartCheckTarget then
									wait(6.5)
									if TargetSelectHunt.Health == TargetSelectHunt.MaxHealth or TargetSelectHunt.Health >= plyselecthunthelpold then
										NextplySelect = true
										TargetSelectHunt = nil
									end
								end
							end
						end
					end
				end)
			end)

			Combat:Toggle("Auto Farm Bounty Hop",_G.AutoFarmBounty_Hop,function(value)
				_G.AutoFarmBounty_Hop = value
			end)
			
			spawn(function()
				while wait() do
					if _G.AutoFarmBounty then
						if _G.AutoFarmBounty_Hop then
							pcall(function()
								wait(120)
								Hop()
							end)
						end
					end
				end
			end)

			Combat:Button("Next Player",function()
				NextplySelect = true
				wait()
				NextplySelect = false
			end)

			Combat:Seperator("ESP")
			
			Combat:Toggle("ESP Player",false,function(value)
				ESPPlayer = value
				while ESPPlayer do wait()
					UpdatePlayerChams()
				end
			end)
			
			Combat:Toggle("ESP Chest",false,function(value)
				ChestESP = value
				while ChestESP do wait()
					UpdateChestEsp() 
				end
			end)
			
			Combat:Toggle("ESP Fruit",false,function(value)
				DevilFruitESP = value
				while DevilFruitESP do wait()
					UpdateBfEsp() 
				end
			end)
			
		if World2 then
			Combat:Toggle("ESP Flower",false,function(value)
				FlowerESP = value
				while FlowerESP do wait()
					UpdateFlowerEsp() 
				end
			end)
		end
			
		Combat:Toggle("ESP Island",IslandESP,function(value)
				IslandESP = value
				while IslandESP do wait()
					UpdateIslandESP() 
				end
			end)
		
		if World2 or World3 then
			Combat:Toggle("ESP Sea Beast",SeaBeastsESP,function(value)
				SeaBeastsESP = value
				while SeaBeastsESP do wait()
					UpdateSeaBeastsESP() 
				end
			end)
		end

		if World3 then
			Combat:Toggle("ESP Real Fruit",RealFruitESP,function(a)
				RealFruitESP = a
				   while RealFruitESP do wait()
					UpdateRealFruitChams() 
				end
			end)
		end

		Combat:Toggle('ESP Npc', false, function(nec)
			NpcESP = nec
		end)

		spawn(function()
			while wait() do
				pcall(function()
					if NpcESP then
						for i,v in pairs(game:GetService("Workspace").NPCs:GetChildren()) do
							if v:FindFirstChild('HumanoidRootPart') then
								if not v:FindFirstChild("NpcEspes") then
									local BillboardGui = Instance.new("BillboardGui")
									local TextLabel = Instance.new("TextLabel")
		
									BillboardGui.Parent = v
									BillboardGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
									BillboardGui.Active = true
									BillboardGui.Name = "NpcEspes"
									BillboardGui.AlwaysOnTop = true
									BillboardGui.LightInfluence = 1.000
									BillboardGui.Size = UDim2.new(1,200,1,30)
									BillboardGui.StudsOffset = Vector3.new(0, 2.5, 0)
		
									TextLabel.Parent = BillboardGui
									TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
									TextLabel.BackgroundTransparency = 1.000
									TextLabel.Size = UDim2.new(1,0,1,0)
									TextLabel.Font = "GothamSemibold"
									TextLabel.FontSize = "Size14"
									TextLabel.TextColor3 = Color3.fromRGB(0, 255, 255)
								end
								local Dis = math.floor((game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude)
								v.NpcEspes.TextLabel.Text = v.Name.." - ["..Dis.." M]"
							end
						end
					else
						for i,v in pairs (game:GetService("Workspace").NPCs:GetChildren()) do
							if v:FindFirstChild("NpcEspes") then
								v.NpcEspes:Destroy()
							end
						end
					end
				end)
			end
		end)

		   Stats:Seperator("Stats")
		
			Stats:Toggle("Auto Stats Kaitan", _G.Fullystats, function(state)
			_G.Fullystats = state
		end)
		
			Stats:Toggle("Auto Melee",_G.Auto_Melee,function(value)
				_G.Auto_Melee = value
			end)
			
			Stats:Toggle("Auto Defense",_G.Auto_Defense,function(value)
				_G.Auto_Defense = value
			end)
			
			Stats:Toggle("Auto Sword",_G.Auto_Sword,function(value)
				_G.Auto_Sword = value
			end)
			
			Stats:Toggle("Auto Gun",_G.Auto_Gun,function(value)
				_G.Auto_Gun = value
			end)
			
			Stats:Toggle("Auto Devil Fruits",_G.Auto_DevilFruit,function(value)
				_G.Auto_DevilFruit = value
			end)
			
			_G.PointStats = 1
			Stats:Slider("Select Point",1,100,1,function(value)
				_G.PointStats = value
			end)
			
			spawn(function()
				while wait() do
					pcall(function()
						if _G.Auto_Melee then
							if game:GetService("Players")["LocalPlayer"].Data.Points.Value ~= 0 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint","Melee",_G.PointStats)
							end
						end
						if _G.Auto_Defense then
							if game:GetService("Players")["LocalPlayer"].Data.Points.Value ~= 0 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint","Defense",_G.PointStats)
							end
						end
						if _G.Auto_Sword then
							if game:GetService("Players")["LocalPlayer"].Data.Points.Value ~= 0 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint","Sword",_G.PointStats)
							end
						end
						if _G.Auto_Gun then
							if game:GetService("Players")["LocalPlayer"].Data.Points.Value ~= 0 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint","Gun",_G.PointStats)
							end
						end
						if _G.Auto_DevilFruit then
							if game:GetService("Players")["LocalPlayer"].Data.Points.Value ~= 0 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint","Demon Fruit",_G.PointStats)
							end
						end
					end)
				end
			end)
			
		spawn(function()
			repeat wait()
				if _G.Fullystats then
					pcall(function()
						Mpoint = game.Players.localPlayer.Data.Stats.Melee.Level.Value
						Dpoint = game.Players.localPlayer.Data.Stats.Defense.Level.Value
						Dvilpoint = game.Players.localPlayer.Data.Stats["Demon Fruit"].Level.Value
						stat = game.Players.localPlayer.Data.Points.Value
						if stat >= 2 then
							if Dpoint <= 249 then
								spawn(function()
									local args = {
										[1] = "AddPoint",
										[2] = "Melee",
										[3] = 1
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end)
								spawn(function()
									local args = {
										[1] = "AddPoint",
										[2] = "Defense",
										[3] = 1
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end)
							end
		
							if Dpoint >= 250 and Mpoint < 2200 then
								spawn(function()
									local args = {
										[1] = "AddPoint",
										[2] = "Melee",
										[3] = 1
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end)
							end
		
							
							if Mpoint == 2200 and Dpoint <= 1800 then
								spawn(function()
									local args = {
										[1] = "AddPoint",
										[2] = "Defense",
										[3] = 1
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end)
							end
							
							if Mpoint == 2100 and Dpoint >= 1800 and Dvilpoint <= 1500 then
								spawn(function()
									local args = {
										[1] = "AddPoint",
										[2] = "Demon Fruit",
										[3] = 1
									}
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
								end)
							end
						end
					end)
				end
			until Mpoint == 2200 and Dpoint >= 1800 and Dvilpoint >= 1500
		end)
	
			Teleport:Seperator("Worlds")
			
			Teleport:Button("Teleport To First Sea",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelMain")
			end)
			
			Teleport:Button("Teleport To Second Sea",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
			end)
			
			Teleport:Button("Teleport To Third Sea",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
			end)
	
			Teleport:Seperator("Island")
		
			if World1 then
				Teleport:Dropdown("Select Island",{
					"WindMill",
					"Marine",
					"Middle Town",
					"Jungle",
					"Pirate Village",
					"Desert",
					"Snow Island",
					"MarineFord",
					"Colosseum",
					"Sky Island 1",
					"Sky Island 2",
					"Sky Island 3",
					"Prison",
					"Magma Village",
					"Under Water Island",
					"Fountain City",
					"Shank Room",
					"Mob Island"
					},function(value)
					_G.SelectIsland = value
				end)
			end
			
			if World2 then
				Teleport:Dropdown("Select Island",{
					"The Cafe",
					"Frist Spot",
					"Dark Area",
					"Flamingo Mansion",
					"Flamingo Room",
					"Green Zone",
					"Factory",
					"Colossuim",
					"Zombie Island",
					"Two Snow Mountain",
					"Punk Hazard",
					"Cursed Ship",
					"Ice Castle",
					"Forgotten Island",
					"Ussop Island",
					"Mini Sky Island",
					"Raid Oder",
					"Awakening Room 2",
					"Teleport to Lab 2"
					},function(value)
					_G.SelectIsland = value
				end)
			end
			
			if World3 then
				Teleport:Dropdown("Select Island",{
					"Mansion",
					"Port Town",
					"Great Tree",
					"Castle On The Sea",
					"MiniSky", 
					"Hydra Island",
					"Floating Turtle",
					"Haunted Castle",
					"Ice Cream Island",
					"Peanut Island",
					"Cake Island",
					"Sea to Treats New",
					"Awakening Room 3",
					"Teleport to Lab 3",
					"Mysterious Force",
					"TikiOutpost"
					},function(value)
					_G.SelectIsland = value
				end)
			end
			
			Teleport:Toggle("Teleport",false,function(value)
				_G.TeleportIsland = value
				if _G.TeleportIsland == true then
					repeat wait()
						if _G.SelectIsland == "WindMill" then
							TP(CFrame.new(979.79895019531, 16.516613006592, 1429.0466308594))
						elseif _G.SelectIsland == "Marine" then
							TP(CFrame.new(-2566.4296875, 6.8556680679321, 2045.2561035156))
						elseif _G.SelectIsland == "Middle Town" then
							TP(CFrame.new(-690.33081054688, 15.09425163269, 1582.2380371094))
						elseif _G.SelectIsland == "Jungle" then
							TP(CFrame.new(-1612.7957763672, 36.852081298828, 149.12843322754))
						elseif _G.SelectIsland == "Pirate Village" then
							TP(CFrame.new(-1181.3093261719, 4.7514905929565, 3803.5456542969))
						elseif _G.SelectIsland == "Desert" then
							TP(CFrame.new(944.15789794922, 20.919729232788, 4373.3002929688))
						elseif _G.SelectIsland == "Snow Island" then
							TP(CFrame.new(1347.8067626953, 104.66806030273, -1319.7370605469))
						elseif _G.SelectIsland == "MarineFord" then
							TP(CFrame.new(-4914.8212890625, 50.963626861572, 4281.0278320313))
						elseif _G.SelectIsland == "Colosseum" then
							TP( CFrame.new(-1427.6203613281, 7.2881078720093, -2792.7722167969))
						elseif _G.SelectIsland == "Sky Island 1" then
							TP(CFrame.new(-4869.1025390625, 733.46051025391, -2667.0180664063))
						elseif _G.SelectIsland == "Sky Island 2" then  
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-4607.82275, 872.54248, -1667.55688))
						elseif _G.SelectIsland == "Sky Island 3" then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
						elseif _G.SelectIsland == "Prison" then
							TP( CFrame.new(4875.330078125, 5.6519818305969, 734.85021972656))
						elseif _G.SelectIsland == "Magma Village" then
							TP(CFrame.new(-5247.7163085938, 12.883934020996, 8504.96875))
						elseif _G.SelectIsland == "Under Water Island" then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
						elseif _G.SelectIsland == "Fountain City" then
							TP(CFrame.new(5127.1284179688, 59.501365661621, 4105.4458007813))
						elseif _G.SelectIsland == "Shank Room" then
							TP(CFrame.new(-1442.16553, 29.8788261, -28.3547478))
						elseif _G.SelectIsland == "Mob Island" then
							TP(CFrame.new(-2850.20068, 7.39224768, 5354.99268))
						elseif _G.SelectIsland == "The Cafe" then
							TP(CFrame.new(-380.47927856445, 77.220390319824, 255.82550048828))
						elseif _G.SelectIsland == "Frist Spot" then
							TP(CFrame.new(-11.311455726624, 29.276733398438, 2771.5224609375))
						elseif _G.SelectIsland == "Dark Area" then
							TP(CFrame.new(3780.0302734375, 22.652164459229, -3498.5859375))
						elseif _G.SelectIsland == "Flamingo Mansion" then
							TP(CFrame.new(-483.73370361328, 332.0383605957, 595.32708740234))
						elseif _G.SelectIsland == "Flamingo Room" then
							TP(CFrame.new(2284.4140625, 15.152037620544, 875.72534179688))
						elseif _G.SelectIsland == "Green Zone" then
							TP( CFrame.new(-2448.5300292969, 73.016105651855, -3210.6306152344))
						elseif _G.SelectIsland == "Factory" then
							TP(CFrame.new(424.12698364258, 211.16171264648, -427.54049682617))
						elseif _G.SelectIsland == "Colossuim" then
							TP( CFrame.new(-1503.6224365234, 219.7956237793, 1369.3101806641))
						elseif _G.SelectIsland == "Zombie Island" then
							TP(CFrame.new(-5622.033203125, 492.19604492188, -781.78552246094))
						elseif _G.SelectIsland == "Two Snow Mountain" then
							TP(CFrame.new(753.14288330078, 408.23559570313, -5274.6147460938))
						elseif _G.SelectIsland == "Punk Hazard" then
							TP(CFrame.new(-6127.654296875, 15.951762199402, -5040.2861328125))
						elseif _G.SelectIsland == "Cursed Ship" then
							TP(CFrame.new(923.40197753906, 125.05712890625, 32885.875))
						elseif _G.SelectIsland == "Ice Castle" then
							TP(CFrame.new(6148.4116210938, 294.38687133789, -6741.1166992188))
						elseif _G.SelectIsland == "Forgotten Island" then
							TP(CFrame.new(-3032.7641601563, 317.89672851563, -10075.373046875))
						elseif _G.SelectIsland == "Ussop Island" then
							TP(CFrame.new(4816.8618164063, 8.4599885940552, 2863.8195800781))
						elseif _G.SelectIsland == "Mini Sky Island" then
							TP(CFrame.new(-288.74060058594, 49326.31640625, -35248.59375))
						elseif _G.SelectIsland == "Great Tree" then
							TP(CFrame.new(2681.2736816406, 1682.8092041016, -7190.9853515625))
						elseif _G.SelectIsland == "Castle On The Sea" then
							TP(CFrame.new(-5074.45556640625, 314.5155334472656, -2991.054443359375))
						elseif _G.SelectIsland == "MiniSky" then
							TP(CFrame.new(-260.65557861328, 49325.8046875, -35253.5703125))
						elseif _G.SelectIsland == "Port Town" then
							TP(CFrame.new(-290.7376708984375, 6.729952812194824, 5343.5537109375))
						elseif _G.SelectIsland == "Hydra Island" then
							TP(CFrame.new(5228.8842773438, 604.23400878906, 345.0400390625))
						elseif _G.SelectIsland == "Floating Turtle" then
							TP(CFrame.new(-13274.528320313, 531.82073974609, -7579.22265625))
						elseif _G.SelectIsland == "Mansion" then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-12471.169921875, 374.94024658203, -7551.677734375))
						elseif _G.SelectIsland == "Haunted Castle" then
							TP(CFrame.new(-9515.3720703125, 164.00624084473, 5786.0610351562))
						elseif _G.SelectIsland == "Ice Cream Island" then
							TP(CFrame.new(-902.56817626953, 79.93204498291, -10988.84765625))
						elseif _G.SelectIsland == "Peanut Island" then
							TP(CFrame.new(-2062.7475585938, 50.473892211914, -10232.568359375))
						elseif _G.SelectIsland == "Cake Island" then
							TP(CFrame.new(-1884.7747802734375, 19.327526092529297, -11666.8974609375))
						elseif _G.SelectIsland == "Sea to Treats New" then
							TP(CFrame.new(-1141.0223388671875, 47.25519561767578, -14204.609375))
						elseif _G.SelectIsland == "Cake Loaf" then
							TP(CFrame.new(-1992.12476, 218.663116, -12415.583, 0.258864343, -0, -0.965913713, 0, 1, -0, 0.965913713, 0, 0.258864343))
						elseif _G.SelectIsland == "Candy Cane" then
							TP(CFrame.new(-1130.41296, 50.7674675, -14567.3242, 0, 0, -1, 0, 1, 0, 1, 0, 0))
						elseif _G.SelectIsland == "Raid Oder" then
							TP(CFrame.new(-5534, 329, -5922))
						elseif _G.SelectIsland == "Teleport to Lab 2" then
							TP(CFrame.new(-6438.73535, 250.645355, -4501.50684))	
						elseif _G.SelectIsland == "Teleport to Lab 3" then
							TP(CFrame.new(-5017.40869, 314.844055, -2823.0127, -0.925743818, 4.48217499e-08, -0.378151238, 4.55503146e-09, 1, 1.07377559e-07, 0.378151238, 9.7681621e-08, -0.925743818))	
						elseif _G.SelectIsland == "Awakening Room 2" then
							TP(CFrame.new(266.227783, 1.39509034, 1857.00732))
						elseif _G.SelectIsland == "Awakening Room 3" then
							TP(CFrame.new(-11571.440429688, 49.172668457031, -7574.7368164062))	
						elseif _G.SelectIsland == "TikiOutpost" then
							TP(CFrame.new(-16233.5947, 9.40381718, 442.631927, 0.0325263776, 4.53748115e-08, -0.99947089, -4.209965e-08, 1, 4.40287593e-08, 0.99947089, 4.06452756e-08, 0.0325263776))
						end					
					until not _G.TeleportIsland
				end
				StopTween(_G.TeleportIsland)
			end)
		
		if World1 then
			Dungeon:Label("Do Not Dungeon World First One")
		end
		
		if World2 or World3 then
			local TimeRaid = Dungeon:Label("Wait For Dungeon")
	
			local island = Dungeon:Label("Wait For Island")
	
			spawn(function()
				pcall(function()
					while wait(.1) do
						if game:GetService("Players").LocalPlayer.PlayerGui.Main.Timer.Visible == true then
							TimeRaid:Set(game:GetService("Players").LocalPlayer.PlayerGui.Main.Timer.Text)
						else
							TimeRaid:Set("Wait For Dungeon")
							island:Set("Wait For Island")
						end
					end
				end)
			end)
	
			spawn(function()
				pcall(function()
					while wait(.1) do
						  if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true then
								if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
									island:Set("Island Left : 5")
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
									island:Set("Island Left : 4")
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
									island:Set("Island Left : 3")
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
									island:Set("Island Left : 2")
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
									island:Set("Island Left : 1")
							end
						end
					end
				end)
			end)
		
			Dungeon:Toggle("Auto Farm Dungeon\nis to release commands to kill around",_G.Auto_Dungeon,function(value)
				_G.Auto_Dungeon = value
				StopTween(_G.Auto_Dungeon)
			end)
			
			spawn(function()
				pcall(function() 
					while wait() do
						if _G.Auto_Dungeon then
							if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true then
								for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
									if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
										pcall(function()
											repeat task.wait()
												sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
												v.Humanoid.Health = 0
												v.HumanoidRootPart.CanCollide = false
											until not _G.Auto_Dungeon or not v.Parent or v.Humanoid.Health <= 0
										end)
									end
								end
							end
						end
					end
				end)
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.Auto_Dungeon then
						  if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true then
								if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
									TP(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame*CFrame.new(0,80,100))
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
									TP(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame*CFrame.new(0,80,100))
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
									TP(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame*CFrame.new(0,80,100))
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
									TP(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame*CFrame.new(0,80,100))
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
									TP(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame*CFrame.new(0,80,100))
								end
							end
						end
					end
				end)
			end)
		
		Dungeon:Toggle("Auto Farm Aura Mon\nis to hit monsters around",_G.Raid,function(value)
			_G.Raid = value
			StopTween(_G.Raid)
		 end)
		
		 spawn(function()
			pcall(function()
				while wait() do
					if _G.Raid then
						for i,v in pairs(game.Workspace.Enemies:GetDescendants()) do
							if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
								Pos = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
								if Pos <= 1000 then
									pcall(function()
										repeat task.wait()
											v.HumanoidRootPart.CanCollide = false
											v.Head.CanCollide = false
											v.HumanoidRootPart.Size = Vector3.new(60,60,60)
											EquipWeapon(_G.SelectWeapon)
											TP(v.HumanoidRootPart.CFrame * CFrame.new(0,40,0))
											PosMonRaid = v.HumanoidRootPart.CFrame
											StartMagnetRaid = true
											game:GetService'VirtualUser':CaptureController()
											game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
										until not _G.Raid or not v.Parent or v.Humanoid.Health <= 0 or not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1")
										StartMagnetRaid = false
									end)
								end
							else
								if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
									Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
									Speed = 260
									tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
									tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame*CFrame.new(0,20,0)})
									tween:Play()
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
									Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
									Speed = 260
									tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
									tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame*CFrame.new(0,20,0)})
									tween:Play()
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
									Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
									Speed = 260
									tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
									tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame*CFrame.new(0,20,0)})
									tween:Play()
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
									Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
									Speed = 260
									tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
									tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame*CFrame.new(0,20,0)})
									tween:Play()
								elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
									Distance = (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
									Speed = 260
									tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
									tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame*CFrame.new(0,20,0)})
									tween:Play()
								end
							end
						end
					end
				end
			end)
		end)
		
			Dungeon:Line()
		
		Dungeon:Toggle("Auto Raid",_G.Auto_Raid,function(vu)
			_G.Auto_Raid = vu
			StopTween(_G.Auto_Raid)
		end)
		
		Dungeon:Toggle("Auto Raid Hop",_G.Auto_Raid_Hop,function(vu)
			_G.Auto_Raid_Hop = vu
		end)
		
			Dungeon:Toggle("Kill Aura",_G.KillAura,function(vu)
		   _G.KillAura = vu
		end)
		
		spawn(function()
		  pcall(function() 
		  while wait() do
			   if _G.KillAura then
				   for i,v in pairs(game.Workspace.Enemies:GetDescendants()) do
					   if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
						   pcall(function()
							   repeat wait()
								   sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								   v.Humanoid.Health = 0
								   v.HumanoidRootPart.CanCollide = false
								   v.HumanoidRootPart.Size = Vector3.new(80,80,80)
							   until not _G.KillAura or not v.Parent or v.Humanoid.Health <= 0
						   end)
					   end
				   end
			   end
		   end
		  end)
		end)
		
		Dungeon:Toggle("Next Islands",_G.Next_Islands,function(vu)
			_G.Next_Islands = vu
			StopTween(_G.Next_Islands)
		end)
	
		if type(_G.SelectChip) ~= 'string' then
			_G.SelectChip = "Flame"
		end
	
		function Buy_Chip()
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("RaidsNpc", "Select", _G.SelectChip)
		end
	
		spawn(function()
			while wait() do
				pcall(function()
					if _G.Auto_Raid then
						if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true then
							for i,v in pairs(game.Workspace.Enemies:GetDescendants()) do
								if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
									repeat wait(.1)
										sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
										v.Humanoid.Health = 0
										v.HumanoidRootPart.CanCollide = false
										v.HumanoidRootPart.Size = Vector3.new(50,50,50)
										v.HumanoidRootPart.Transparency = 1
									until not _G.Auto_Raid or not v.Parent or v.Humanoid.Health <= 0
								end
							end
						end
					else
						wait(3)
					end
				end)
			end
		end)
	
		spawn(function()
			while wait() do
				pcall(function()
					if _G.Next_Islands or _G.Auto_Raid then
						if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
							for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
								if v.Name == "Island 5" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 2300 then
									TP(v.CFrame*CFrame.new(0,70,0))
								end
							end
						elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
							for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
								if v.Name == "Island 4" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 2000 then
									TP(v.CFrame*CFrame.new(0,70,0))
								end
							end
						elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
							for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
								if v.Name == "Island 3" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 2100 then
									TP(v.CFrame*CFrame.new(0,70,0))
								end
							end
						elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
							for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
								if v.Name == "Island 2" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 2000 then
									TP(v.CFrame*CFrame.new(0,70,0))
								end
							end
						elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
							for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
								if v.Name == "Island 1" and (v.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 2000 then
									TP(v.CFrame*CFrame.new(0,70,0))
								end
							end
						else
							wait(1)
						end
					else
						wait(2)
					end
				end)
			end
		end)
		
		spawn(function()
			while wait() do
				pcall(function()
					if _G.Auto_Raid_Farm then
						if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
							_G.StopTween = true
						elseif game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true then
							_G.StopTween = false
						end
					end
				end)
			end
		end)
		
		spawn(function()
			while wait() do
				pcall(function()
					if _G.Auto_Raid then
						if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
							if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Special Microchip") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Special Microchip") then
								_G.Auto_Raid_Farm = true
								if World2 then
									fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
									repeat wait(1)
									until game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true
								elseif World3 then
									fireclickdetector(game:GetService("Workspace").Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
									repeat wait(1)
									until game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true
								end
							else
								if _G.Auto_Raid_Hop then
									_G.Have_Fruit = nil
								end
								Buy_Chip()
								wait(1)
								if _G.Auto_Raid_Hop and not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Special Microchip") and not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Special Microchip") then
									Hop()
									wait(50)
								elseif _G.Auto_Raid_Farm and not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Special Microchip") and not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Special Microchip") then
									_G.Stop_Tween = nil
									_G.Auto_Raid_Farm = nil
									local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
									local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
									wait(1)
									Notification:Notify(
										{Title = "Pado Hub", Description = "There are no devil fruits left."},
										{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 3, Type = "default"}
									)
								end
							end
						elseif game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true then
							repeat wait(1)
							until game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false
							if _G.Auto_Awaken then
								wait(2)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Awakener","Check")
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Awakener","Awaken")
							end
						end
					end
				end)
			end
		end)
		
			Dungeon:Toggle("Auto Awakener",_G.Auto_Awakener,function(value)
				_G.Auto_Awakener = value
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.Auto_Awakener then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Awakener","Check")
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Awakener","Awaken")
						end
					end
				end)
			end)
		end
		
		if World2 or World3 then
		
			Dungeon:Line()
	
			Dungeon:Dropdown("Select Chips",{"Flame","Ice","Quake","Light","Dark","String","Rumble","Magma","Human: Buddha","Sand","Bird: Phoenix","Dough"},function(value)
				_G.SelectChip = value
			end)
																									
			Dungeon:Toggle("Auto Select Dungeon",_G.AutoSelectDungeon,function(value)
				_G.AutoSelectDungeon = value
			end)
			
			spawn(function()
				while wait() do
					if _G.AutoSelectDungeon then
						pcall(function()
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flame-Flame") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flame-Flame") then
								_G.SelectChip = "Flame"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Ice-Ice") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Ice-Ice") then
								_G.SelectChip = "Ice"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Quake-Quake") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Quake-Quake") then
								_G.SelectChip = "Quake"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Light-Light") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Light-Light") then
								_G.SelectChip = "Light"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dark-Dark") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dark-Dark") then
								_G.SelectChip = "Dark"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("String-String") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("String-String") then
								_G.SelectChip = "String"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rumble-Rumble") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rumble-Rumble") then
								_G.SelectChip = "Rumble"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Magma-Magma") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Magma-Magma") then
								_G.SelectChip = "Magma"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Human-Human: Buddha Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Human-Human: Buddha Fruit") then
								_G.SelectChip = "Human: Buddha"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sand-Sand") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Sand-Sand") then
								_G.SelectChip = "Sand"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird-Bird: Phoenix") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird-Bird: Phoenix") then
								_G.SelectChip = "Bird: Phoenix"
							elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dough") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dough") then
								_G.SelectChip = "Dough"
							else
								_G.SelectChip = "Flame"
							end
						end)
					end
				end
			end)
			
			Dungeon:Toggle("Auto Start Raid",_G.Auto_StartRaid,function(value)
				_G.Auto_StartRaid = value
			end)
			
			spawn(function()
				while wait() do
					pcall(function()
						if _G.Auto_StartRaid then
							if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
								if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") and game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Special Microchip") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Special Microchip") then
									if World2 then
										fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
									elseif World3 then
										fireclickdetector(game:GetService("Workspace").Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
									end
								end
							end
						end
					end)
				end
			end)
			
			Dungeon:Button("Start Raid",function()
				if World2 then
					fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
				elseif World3 then
					fireclickdetector(game:GetService("Workspace").Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
				end
			end)
		
			Dungeon:Toggle("Auto Buy Chip",_G.AutoBuyChip,function(value)
				_G.AutoBuyChip = value
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.AutoBuyChip then
							if not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Special Microchip") or not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Special Microchip") then
								if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("RaidsNpc", "Select", _G.SelectChip)
								end
							end
						end
					end
				end)
			end)
		
			Dungeon:Button("Buy Chip Select",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("RaidsNpc","Select",_G.SelectChip)
			end)
		end
		
			DevilFruit:Seperator("Sniper")
		
			FruitList = {
				"Spike-Spike",
				"Chop-Chop",
				"Spring-Spring",
				"Kilo-Kilo",
				"Spin-Spin",
				"Bomb-Bomb",
				"Bird: Falcon",
				"Smoke-Smoke",
				"Flame-Flame",
				"Ice-Ice",
				"Sand-Sand",
				"Dark-Dark",
				"Revive-Revive",
				"Diamond-Diamond",
				"Light-Light",
				"Love-Love",
				"Rubber-Rubber",
				"Barrier-Barrier",
				"Magma-Magma",
				"Quake-Quake",
				"Human-Human: Buddha",
				"String-String",
				"Portal-Portal",
				"Bird-Bird: Phoenix",
				"Rumble-Rumble",
				"Paw-Paw",
				"Blizzard-Blizzard",
				"Gravity-Gravity",
				"Dough-Dough",
				"Venom-Venom",
				"Shadow-Shadow",
				"Control-Control",
				"Spirit-Spirit",
				"Dragon-Dragon",
				"Leopard-Leopard"
			}
			
			_G.SelectFruit = ""
			DevilFruit:Dropdown("Select Fruits Sniper",FruitList,function(value)
				_G.SelectFruit = value
			end)
			
			DevilFruit:Toggle("Auto Buy Fruit Sniper",_G.AutoBuyFruitSniper,function(value)
				_G.AutoBuyFruitSniper = value
			end)
	
			DevilFruit:Seperator("Eat")
	
			DevilFruit:Dropdown("Select Fruits Eat",FruitList,function(value)
				_G.SelectFruitEat = value
			end)
			
			DevilFruit:Toggle("Auto Eat Fruit",_G.AutoEatFruit,function(value)
				_G.AutoEatFruit = value
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.AutoEatFruit then
							game:GetService("Players").LocalPlayer.Character:FindFirstChild(_G.SelectFruitEat).EatRemote:InvokeServer()
						end
					end
				end)
			end)
			
			DevilFruit:Toggle("Auto Eat Fruit Hop",_G.AutoEatFruitHop,function(value)
				_G.AutoEatFruitHop = value
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.AutoEatFruitHop and _G.SelectFruitEat ~= nil then
							if not game:GetService("Players").LocalPlayer.Character:FindFirstChild(_G.SelectFruitEat) or not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild(_G.SelectFruitEat) then
								Hop()
							else
								game:GetService("Players").LocalPlayer.Character:FindFirstChild(_G.SelectFruitEat).EatRemote:InvokeServer()
							end
						end
					end
				end)
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.AutoBuyFruitSniper then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("GetFruits")
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PurchaseRawFruit",_G.SelectFruit)
						end 
					end
				end)
			end)
	
			DevilFruit:Seperator("Other")
		
			DevilFruit:Toggle("Get Fruit Inventory",_G.Get_Fruit,function(vu)
				_G.Get_Fruit = vu
			end)
			
			spawn(function()
				while wait() do
					pcall(function()
						if _G.Get_Fruit then
							if Inventory_Fruit then
								Inventory_Fruit = nil
							end
							fruit = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getInventoryFruits")
							for i,v in pairs(fruit) do
								if v["Price"] < 10000000 then
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("LoadFruit",v["Name"])
								end
							end
						else
							wait(2)
						end
					end)
				end
			end)
		
			DevilFruit:Button("Random Fruit",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
			end)
		
			DevilFruit:Toggle("Auto Random Fruit",_G.Random_Auto,function(value)
				_G.Random_Auto = value
			end)
		
		 spawn(function()
				pcall(function()
					while wait() do
						if _G.Random_Auto then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
						end 
					end
				end)
			end)
		
			DevilFruit:Toggle("Auto Drop Fruit",_G.DropFruit,function(value)
				_G.DropFruit = value
			end)
				
			spawn(function()
				while wait() do
				if _G.DropFruit then
					pcall(function()
						if _G.DropFruit then
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bomb Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bomb Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bomb Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spike Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spike Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spike Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Chop Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Chop Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Chop Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spring Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spring Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spring Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Kilo Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Kilo Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Kilo Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Smoke Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Smoke Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Smoke Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spin Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spin Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spin Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flame Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flame Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flame Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird: Falcon Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird: Falcon Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird: Falcon Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Ice Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Ice Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Ice Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sand Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Sand Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sand Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dark Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dark Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dark Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Revive Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Revive Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Revive Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Diamond Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Diamond Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Diamond Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Light Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Light Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Light Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Love Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Love Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Love Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rubber Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rubber Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rubber Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Barrier Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Barrier Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Barrier Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Magma Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Magma Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Magma Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Portal Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Portal Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Portal Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Quake Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Quake Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Quake Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Human-Human: Buddha Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Human-Human: Buddha Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Human-Human: Buddha Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spider Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spider Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spider Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird: Phoenix Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird: Phoenix Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird: Phoenix Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rumble Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rumble Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rumble Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Paw Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Paw Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Paw Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Gravity Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Gravity Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Gravity Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dough Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dough Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dough Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Shadow Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Shadow Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Shadow Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Venom Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Venom Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Venom Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Control Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Control Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Control Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spirit Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Soul Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spirit Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon Fruit").EatRemote:InvokeServer("Drop")
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Leopard Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Leopard Fruit") then
								game:GetService("Players").LocalPlayer.Character:FindFirstChild("Leopard Fruit").EatRemote:InvokeServer("Drop")
							end
						end
					end)
				end
			end
		end)
	
			spawn(function()
				while wait() do
					if _G.DropFruit then
						pcall(function()
							for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
								if string.find(v.Name, "Fruit") then
									EquipWeapon(v.Name)
								end
							end
						for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetChildren()) do
								if string.find(v.Name, "Fruit") then
									EquipWeapon(v.Name)
								end
							end
						end)
					end
				end
			end)
			
			DevilFruit:Toggle("Auto Store Fruit",_G.AutoStoreFruit,function(value)
				_G.AutoStoreFruit = value
			end)
			
			spawn(function()
				while wait() do
				if _G.AutoStoreFruit then
					pcall(function()
						if _G.AutoStoreFruit then
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bomb Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bomb Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Bomb-Bomb",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bomb Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spike Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spike Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Spike-Spike",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spike Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Chop Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Chop Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Chop-Chop",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Chop Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spring Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spring Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Spring-Spring",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spring Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Kilo Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Kilo Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Kilo-Kilo",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Kilo Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Smoke Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Smoke Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Smoke-Smoke",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Smoke Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spin Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spin Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Spin-Spin",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spin Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flame Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flame Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Flame-Flame",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flame Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird: Falcon Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird: Falcon Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Bird-Bird: Falcon",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird: Falcon Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Ice Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Ice Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Ice-Ice",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Ice Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sand Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Sand Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Sand-Sand",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Sand Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dark Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dark Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Dark-Dark",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dark Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Revive Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Revive Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Revive-Revive",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Revive Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Diamond Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Diamond Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Diamond-Diamond",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Diamond Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Light Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Light Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Light-Light",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Light Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Love Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Love Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Love-Love",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Love Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rubber Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rubber Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Rubber-Rubber",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rubber Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Barrier Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Barrier Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Barrier-Barrier",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Barrier Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Magma Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Magma Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Magma-Magma",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Magma Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Door Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Door Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Door-Door",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Door Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Quake Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Quake Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Quake-Quake",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Quake Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Human-Human: Buddha Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Human-Human: Buddha Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Human-Human: Buddha",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Human-Human: Buddha Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("String Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("String Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","String-String",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("String Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird: Phoenix Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird: Phoenix Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Bird-Bird: Phoenix",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird: Phoenix Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rumble Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rumble Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Rumble-Rumble",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rumble Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Paw Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Paw Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Paw-Paw",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Paw Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Gravity Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Gravity Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Gravity-Gravity",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Gravity Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dough Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dough Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Dough-Dough",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dough Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Shadow Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Shadow Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Shadow-Shadow",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Shadow Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Venom Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Venom Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Venom-Venom",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Venom Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Control Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Control Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Control-Control",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Control Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Soul Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Soul Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Soul-Soul",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Soul Fruit"))
							end
							if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Fruit") then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Dragon-Dragon",game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Fruit"))
							end
						end
					end)
				end
			end
		end)
	
		DevilFruit:Toggle("Auto Bring Fruit",_G.AutoBringFruit,function(value)
			_G.AutoBringFruit = value
		end)
		
		spawn(function()
			pcall(function()
				while wait() do
					if _G.AutoBringFruit then
						for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
							if string.find(v.Name, "Fruit") then
								if v:IsA("Tool") then
									v.Handle.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0, 50, 0)
									wait(.2)
									firetouchinterest(game.Players.LocalPlayer.Character.HumanoidRootPart,v.Handle,0)
								end
							end
						end
					else
						wait(1)
					end
				end
			end)
		end)
	
			Shop:Seperator("Abilities")
			
			Shop:Button("Buy Geppo [ Use $10,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Geppo")
			end)
			
			Shop:Button("Buy Buso Haki [ Use $25,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Buso")
			end)
			
			Shop:Button("Buy Soru [ Use $25,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Soru")
			end)
			
			Shop:Button("Buy Observation Haki [ Use $750,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("KenTalk","Buy")
			end)
			
		Shop:Toggle("Auto Buy Abilities", false, function(t)
			Abilities = t
			while Abilities do wait(.1)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Geppo")
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Buso")
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Soru")
			end
		end)
		
		Shop:Seperator("Boats")
		
		BoatList = {
			"Pirate Sloop",
			"Enforcer",
			"Rocket Boost",
			"Dinghy",
			"Pirate Basic",
			"Pirate Brigade"
		}
		
		spawn(function()
			while wait() do
				pcall(function()
					if SelectBoat == "Pirate Sloop" then
						_G.SelectBoat = "PirateSloop"
					else
						if SelectBoat == "Enforcer" then
							_G.SelectBoat = "Enforcer"
						else
							if SelectBoat == "RocketBoost" then
								_G.SelectBoat = "RocketBoost"
							else
								if SelectBoat == "PirateBasic" then
									_G.SelectBoat = "PirateBasic"
								else
									if SelectBoat == "PirateBrigade" then
										_G.SelectBoat = "PirateBrigade"
									end
								end
							end
						end
					end
				end)
			end
		end)
		
		Shop:Dropdown("Select Boats",BoatList,function(value)
			SelectBoat = value
		end)
		
		Shop:Button("Buy Boat",function()
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyBoat",_G.SelectBoat)
		end)
		
			Shop:Seperator("Fighting Style")
			
			Shop:Button("Buy Black Leg [ Use $150,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyBlackLeg")
			end)
			
			Shop:Button("Buy Electro [ Use $550,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro")
			end)
			
			Shop:Button("Buy Fishman Karate [ Use $750,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyFishmanKarate")
			end)
			
			Shop:Button("Buy Dragon Claw [ Use $1,500 Fragments ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","1")
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","2")
			end)
			
			Shop:Button("Buy Superhuman [ Use $3,000,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySuperhuman")
			end)
			
			Shop:Button("Buy Death Step [ Use $5,000 Fragments $5,000,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDeathStep")
			end)
			
			Shop:Button("Buy Sharkman Karate [ Use $5,000 Fragments $2,500,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true)
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate")
			end)
			
			Shop:Button("Buy Electric Claw [ Use $5,000 Fragments $3,000,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
			end)
			
			Shop:Button("Buy Dragon Talon [ Use $5,000 Fragments $3,000,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon")
			end)
		
			Shop:Button("Buy God Human [ Use $5,000 Fragments $5,000,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyGodhuman")
			end)
			-----Shop----------------
			
			Shop:Seperator("Sword")
			
			Shop:Button("Cutlass [ Use $1,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Cutlass")
			end)
		
			Shop:Button("Katana [ Use $1,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Katana")
			end)
			
			Shop:Button("Iron Mace [ Use $25,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Iron Mace")
			end)
			
			Shop:Button("Dual Katana [ Use $12,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Duel Katana")
			end)
			
			Shop:Button("Triple Katana [ Use $60,000 Beli ]", function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Triple Katana")
			end)
			
			Shop:Button("Pipe [ Use $100,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Pipe")
			end)
			
			Shop:Button("Dual-Headed Blade [ Use $400,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Dual-Headed Blade")
			end)
		
			Shop:Button("Bisento [ Use $1,200,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Bisento")
			end)
			
			Shop:Button("Soul Cane [ Use $750,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Soul Cane")
			end)
		
			Shop:Button("Pole v.2 [ Use 5,000 Fragments ]",function()
				game.ReplicatedStorage.Remotes.CommF_:InvokeServer("ThunderGodTalk")
			end)
	
			Shop:Button("Yoru v2 [ Quest Yoru ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack({
					[1] = "RobotTalk"
				  }))
				  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack({
					[1] = "IndraTalk"
				  }))
				  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack({
					[1] = "LoveLetter",
					[2] = 1
				  }))
				  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack({
					[1] = "LoveLetter",
					[2] = 2
				  }))
				  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack({
					[1] = "LoveLetter",
					[2] = 3
				  }))
				  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack({
					[1] = "RobotTalk"
				  }))
				end)
		
			Shop:Toggle("Yama Sword [ Use Elite Hunter 30 ]",_G.AutoYama,function(value)
				_G.AutoYama = value
			end)
			
			spawn(function()
				while wait() do
					if _G.AutoYama then
						if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter","Progress") >= 30 then
							repeat wait(.1)
								fireclickdetector(game:GetService("Workspace").Map.Waterfall.SealedKatana.Handle.ClickDetector)
							until game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Yama") or not _G.AutoYama
						end
					end
				end
			end)
	
			Shop:Seperator("Gun")
			
			Shop:Button("Slingshot [ Use $5,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Slingshot")
			end)
			
			Shop:Button("Musket [ Use $8,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Musket")
			end)
			
			Shop:Button("Flintlock [ Use $10,500 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Flintlock")
			end)
			
			Shop:Button("Refined Slingshot [ Use $30,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Refined Flintlock")
			end)
			
			Shop:Button("Refined Flintlock [ Use $65,000 Beli ]",function()
				local args = {
					[1] = "BuyItem",
					[2] = "Refined Flintlock"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
			
			Shop:Button("Cannon [ Use $100,000 Beli ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Cannon")
			end)
			
			Shop:Button("Kabucha [ Use 1,500 Fragments]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Slingshot","1")
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Slingshot","2")
			end)
		
				  Shop:Button("Bizarre Rifle [ 250 Ectoplasm ]", function()
											local A_1 = "Ectoplasm"
											local A_2 = "Buy"
											local A_3 = 1
											local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
											Event:InvokeServer(A_1, A_2, A_3) 
											local A_1 = "Ectoplasm"
											local A_2 = "Buy"
											local A_3 = 1
											local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
											Event:InvokeServer(A_1, A_2, A_3)
										end)
		
			------------Bone------------------
			
			Shop:Seperator("Bones")
			
			Shop:Button("Buy Surprise [ Use $50 Bone ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Bones","Buy",1,1)
			end)
			
			Shop:Button("Stat Refund [ Use $50 Bone ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Bones","Buy",1,2)
			end)
				
			Shop:Button("Race Reroll [ Use $50 Bone ]",function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Bones","Buy",1,3)
			end)
			
			------------Stat------------------
			
			Shop:Seperator("Stat")
		
		Shop:Button("Reset Stats [ Use 2.5K Fragments ]", function()
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Refund","1")
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Refund","2")
		end)
		
		Shop:Button("Random Race [ Use 3K Fragments ]", function()
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Reroll","1")
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Reroll","2")
		end)
			--------------Accessories-----------------
				Shop:Seperator("Accessories")
			Shop:Button("Black Cape [ Use $50,000 Beli ]",function()
				local args = {
					[1] = "BuyItem",
					[2] = "Black Cape"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
			Shop:Button("Swordsman Hat [ Use $150,000 Beli ]",function()
				local args = {
					[1] = "BuyItem",
					[2] = "Swordsman Hat"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
			Shop:Button("Tomoe Ring [ Use $500,000 Beli ]",function()
				local args = {
					[1] = "BuyItem",
					[2] = "Tomoe Ring"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
			
			Shop:Seperator("Race & etc")
			
			Shop:Button("Race Ghoul [ Use 2.5K Fragments ]",function()
				local args = {
					[1] = "Ectoplasm",
					[2] = "BuyCheck",
					[3] = 4
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
				local args = {
					[1] = "Ectoplasm",
					[2] = "Change",
					[3] = 4
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
			
			Shop:Button("Race Cyborg [ Use 2.5K Fragments ]",function()
				local args = {
					[1] = "CyborgTrainer",
					[2] = "Buy"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
	
			Misc:Seperator("Server")
			
			Misc:Button("Copy discord Server",function()
				setclipboard("https://discord.gg/aQEPQA9a8e")
			end)
	
			Misc:Button("Rejoin Server",function()
				game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
			end)
		
		  Misc:Button("Hop Server",function()
		   Hop()
		  end)
		  
			Misc:Button("Hop Lower Server",function()
				local Player = game.Players.LocalPlayer    
				local Http = game:GetService("HttpService")
				local TPS = game:GetService("TeleportService")
				local Api = "https://games.roblox.com/v1/games/"
				
				local _place,_id = game.PlaceId, game.JobId
				local _servers = Api.._place.."/servers/Public?sortOrder=Desc&limit=100"
				function ListServers(cursor)
				   local Raw = game:HttpGet(_servers .. ((cursor and "&cursor="..cursor) or ""))
				   return Http:JSONDecode(Raw)
				end
				
				local Next; repeat
				   local Servers = ListServers(Next)
				   for i,v in next, Servers.data do
					   if v.playing < v.maxPlayers and v.id ~= _id then
						   local s,r = pcall(TPS.TeleportToPlaceInstance,TPS,_place,v.id,Player)
						   if s then break end
					   end
				   end
				   
				   Next = Servers.nextPageCursor
				until not Next
			  end)
			
			Misc:Button("Destroy Ui",function()
				if game.CoreGui:FindFirstChild("Pado Hub") then
					game.CoreGui:FindFirstChild("Pado Hub"):Destroy()
					game.CoreGui:FindFirstChild("PADOXHUBMODILE"):Destroy()
				end
			end)

			Misc:Seperator("Ui")
			
			Misc:Button("Open Title Name",function()
				game.Players.localPlayer.PlayerGui.Main.Titles.Visible = true
			end)
			
			Misc:Button("Open Color Haki",function()
				game.Players.localPlayer.PlayerGui.Main.Colors.Visible = true
			end)
			
			Misc:Button("Open Awakenings Expert",function()
			 game.Players.LocalPlayer.PlayerGui.Main.AwakeningToggler.Visible = true
		    end)
		
			Misc:Seperator("Teams")
			
		Misc:Button("Join Pirates Team", function()
			local args = {
				[1] = "SetTeam",
				[2] = "Pirates"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
			local args = {
				[1] = "BartiloQuestProgress"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end)
		
		Misc:Button("Join Marines Team",function()
			local args = {
				[1] = "SetTeam",
				[2] = "Marines"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			local args = {
				[1] = "BartiloQuestProgress"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end)
	
		   Misc:Seperator("Special")
			
				Misc:Button("Remove Lave",function()
				for i,v in pairs(game.Workspace:GetDescendants()) do
					if v.Name == "Lava" then   
						v:Destroy()
					end
				end
				for i,v in pairs(game.ReplicatedStorage:GetDescendants()) do
					if v.Name == "Lava" then   
						v:Destroy()
					end
				end
			end)
	
			Misc:Toggle("Ctrl + Click = TP",false,function(vu)
				CTRL = vu
			 end)
			 
			 local Plr = game:GetService("Players").LocalPlayer
			 local Mouse = Plr:GetMouse()
			 Mouse.Button1Down:connect(
				function()
					if not game:GetService("UserInputService"):IsKeyDown(Enum.KeyCode.LeftControl) then
						return
					end
					if not Mouse.Target then
						return
					end
					if CTRL then
						Plr.Character:MoveTo(Mouse.Hit.p)
					end
				end
			 )
			 
			 Misc:Toggle("Ctrl + Click = Tween",false,function(vu)
				getgenv().Enabled = vu -- false ปิด
			 
				local speed = 200
				local bodyvelocityenabled = true
			 
				local UIS = game:GetService("UserInputService")
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
			 
				UIS.InputBegan:Connect(function(input)
					if input.UserInputType == Enum.UserInputType.MouseButton1 and UIS:IsKeyDown(Enum.KeyCode.LeftControl) and Enabled then
						To(Mouse.Hit.p)
					end
				end)
			 end)
			 local Plr = game:GetService("Players").LocalPlayer
			 local Mouse = Plr:GetMouse()
			 Mouse.Button1Down:connect(function()
				if not game:GetService("UserInputService"):IsKeyDown(Enum.KeyCode.LeftControl) then
					return
				end
				if not Mouse.Target then
					return
				end
				if CTRL then
					Plr.Character:MoveTo(Mouse.Hit.p)
				end
			 end)
			 
			 Misc:Button("Ctrl + Click = TP Tool", function()
			 local plr = game:GetService("Players").LocalPlayer
			 local mouse = plr:GetMouse()
			 
			 local Tool1 = Instance.new("Tool")
			 Tool1.RequiresHandle = false
			 Tool1.Name = "Click To Teleport"
			 Tool1.Parent = plr.Backpack
			 Tool1.Activated:Connect(function()
			local root = plr.Character.HumanoidRootPart
			local pos = mouse.Hit.Position+Vector3.new(0,2.5,0)
			local offset = pos-root.Position
			root.CFrame = root.CFrame+offset
			end)
		end)
		
			Misc:Button("Invisible (lag Ping)",function()
			game.Players.LocalPlayer.Character.LowerTorso.Root:Destroy()
		end)
			
			Misc:Button("Invisible (Remove body)",function()
		local removeNametags = true -- remove custom billboardgui nametags from hrp, could trigger anticheat
		local plr = game:GetService("Players").LocalPlayer
		local character = plr.Character
		local hrp = character.HumanoidRootPart
		local old = hrp.CFrame
		
		if not character:FindFirstChild("LowerTorso") or character.PrimaryPart ~= hrp then
		return print("unsupported")
		end
		
		if removeNametags then
		local tag = hrp:FindFirstChildOfClass("BillboardGui")
		if tag then tag:Destroy() end
		
		hrp.ChildAdded:Connect(function(item)
		if item:IsA("BillboardGui") then
		task.wait()
		item:Destroy()
		end
		end)
		end
		
		local newroot = character.LowerTorso.Root:Clone()
		hrp.Parent = workspace
		character.PrimaryPart = hrp
		character:MoveTo(Vector3.new(old.X,9e9,old.Z))
		hrp.Parent = character
		task.wait(0.5)
		newroot.Parent = hrp
		hrp.CFrame = old
		end)
			
		Misc:Button("Animations (emoji)",function()
			local animations = {
				["Dophin Dance"] = 5918726674,
				["Applaud"] = 5915693819,
				["Country Line  Dance"] = 5915712534,
				["Floss  Dance"] = 5917459365,
				["Panini Dance"] = 5915713518,
				["Rock On"] = 5915714366,
				["Rodeo Dance"] = 5918728267,
				["Break Dance"] = 5915648917,
				["High Wave"] = 5915690960,
				["Holiday Dance"] = 5937558680,
				["Old Town Road Dance"] = 5937560570,
				["Around Town"] = 3303391864,
				["Top Rock"] = 3361276673,
				["Fashionable"] = 3333331310,
				["Robot"] = 3338025566,
				["Twirl"] = 3334968680,
				["Jacks"] = 3338066331,
				["T"] = 3338010159,
				["Shy"] = 3337978742,
				["Monkey"] = 3333499508,
				["Borock's Rage"] = 3236842542,
				["Ud'zal's Summoning"] = 3303161675,
				["Hype Dance"] = 3695333486,
				["Godlike"] = 3337994105,
				["Swoosh"] = 3361481910,
				["Sneaky"] = 3334424322,
				["Side to Side"] = 3333136415,
				["Greatest"] = 3338042785,
				["Louder"] = 3338083565,
				["Beckon"] = 5230598276,
				["Bored"] = 5230599789,
				["Cower"] = 4940563117,
				["Tantrum"] = 5104341999,
				["Hero Landing"] = 5104344710,
				["Confused"] = 4940561610,
				["Jumping Wave"] = 4940564896,
				["Keeping Time"] = 4555808220,
				["Agree"] = 4841397952,
				["Power Blast"] = 4841403964,
				["Disagree"] = 4841401869,
				["Sleep"] = 4686925579,
				["Sad"] = 4841407203,
				["Happy"] = 4841405708,
				["Chicken Dance"] = 4841399916,
				["Bunny Hop"] = 4641985101,
				["Air Dance"] = 4555782893,
				["Curtsy"] = 4555816777,
				["Zombie"] = 4210116953,
				["Fast Hands"] = 4265701731,
				["Baby Dance"] = 4265725525,
				["Celebrate"] = 3338097973,
				["Fancy Feet"] = 3333432454,
				["Y"] = 4349285876,
				["Shuffle"] = 4349242221,
				["Bodybuilder"] = 3333387824,
				["Sandwich Dance"] = 4406555273,
				["Dorky Dance"] = 4212455378,
				["Heisman Pose"] = 3695263073,
				["Superhero Reveal"] = 3695373233,
				["Dizzy"] = 3361426436,
				["Get Out"] = 3333272779,
				["Fishing"] = 3334832150,
				["Tree"] = 4049551434,
				["Line Dance"] = 4049037604,
				["Idol"] = 4101966434,
				["Haha"] = 3337966527,
				["Salute"] = 3333474484,
				["Hello"] = 3344650532,
				["Air Guitar"] = 3695300085,
				["Cha Cha"] = 3695322025,
				["Shrug"] = 3334392772,
				["Point2"] = 3344585679,
				["Tilt"] = 3334538554,
				["Drum Master"] = 6531483720,
				["Saturday Dance"] = 7422807549,
				["It Ain't My Fault"] = 6797891807,
				["Flare"] = 10214311282,
				["SIDE KICKS"] = 10370362157,
				["BOOM BOOM CLAP"] = 10370346995,
				["CARTWHEEL"] = 10370351535,
				["V Pose"] = 10214319518,
				["drumsolo"] = 6532839007,
				["supercharge"] = 10478338114,
				["Floor Rock Freeze - Tommy Hilfiger"] = 10214314957,
				["Alo Yoga Pose - Lotus Position"] = 12507085924,
				["Ay-Yo Dance Move - NCT 127"] = 12804157977,
				["Stadium"] = 3338055167
			}
			
			local plr = game.Players.LocalPlayer
			local LoganWS = Instance.new('Folder', game)
			LoganWS.Name = 'LoganWS'
			
			local buttonHolder = Instance.new('Folder', LoganWS)
			buttonHolder.Name = "Buttons"
			
			
			local Animations = Instance.new("ScreenGui")
			local MainFrame = Instance.new("Frame")
			local UIGradient = Instance.new("UIGradient")
			local Title = Instance.new("TextLabel")
			local SearchBox = Instance.new("TextBox")
			local Container = Instance.new("ScrollingFrame")
			local Button = Instance.new("TextButton")
			local UIListLayout = Instance.new("UIListLayout")
			local UIListLayout2 = Instance.new("UIListLayout")
			local UIListLayout3 = Instance.new("UIListLayout")
			local StopAnim = Instance.new("TextButton")
			local PauseAnim = Instance.new("TextButton")
			local ReplayAnim = Instance.new("TextButton")
			local ReverseAnim = Instance.new("TextButton")
			local Exit = Instance.new("TextButton")
			local Mini = Instance.new("TextButton")
			local titleFrame = Instance.new("Frame")
			local slideFrame = Instance.new("Frame")
			local SlideBar = Instance.new("Frame")
			local SlideButton = Instance.new("TextButton")
			local creds = Instance.new("TextLabel")
			
			Animations.Name = "Animations"
			Animations.Parent = plr:WaitForChild("PlayerGui")
			
			MainFrame.Name = "MainFrame"
			MainFrame.Parent = Animations
			MainFrame.BackgroundColor3 = Color3.fromRGB(195, 195, 195)
			MainFrame.BorderColor3 = Color3.fromRGB(195, 195, 195)
			MainFrame.BorderSizePixel = 1
			MainFrame.Position = UDim2.new(0.4, 0, 0.2, 0)
			MainFrame.Size = UDim2.new(0.1, 0, 0.415, 0)
						spawn(function()
						while wait() do
							pcall(function()
								wait(0.1) 
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 0, 0)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 155, 0)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 255, 0)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(0, 255, 0)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(0, 255, 255)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(0, 155, 255)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 0, 255)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 0, 155)}
								):Play() 
								wait(.5)
							end)
						end
					end)
			
			titleFrame.Name = "TitleFrame"
			titleFrame.Parent = MainFrame
			titleFrame.BorderSizePixel = 0
			titleFrame.LayoutOrder = 0
			titleFrame.BackgroundTransparency = 1
			titleFrame.Size = UDim2.new(1, 0, 0.05, 0)
			
			slideFrame.Name = "SlideFrame"
			slideFrame.Parent = MainFrame
			slideFrame.BorderSizePixel = 0
			slideFrame.LayoutOrder = 3
			slideFrame.BackgroundTransparency = 1
			slideFrame.Size = UDim2.new(1, 0, 0.01, 0)
			
			UIListLayout3.Parent = titleFrame
			UIListLayout3.FillDirection = Enum.FillDirection.Horizontal
			UIListLayout3.SortOrder = Enum.SortOrder.LayoutOrder
			
			UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(102, 45, 113)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(197, 66, 110))}
			UIGradient.Parent = MainFrame
			
			Title.Name = "Title"
			Title.Parent = titleFrame
			Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			Title.BackgroundTransparency = 1.000
			Title.Size = UDim2.new(1, 0, 1, 0)
			Title.Font = Enum.Font.GothamSemibold
			Title.Text = "Animation"
			Title.TextColor3 = Color3.fromRGB(255, 255, 255)
			Title.TextScaled = true
			Title.TextSize = 14.000
			Title.TextWrapped = true
			Title.LayoutOrder = 0
			
			SearchBox.Name = "SearchBox"
			SearchBox.Parent = MainFrame
			SearchBox.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			SearchBox.BackgroundTransparency = 0.750
			SearchBox.BorderSizePixel = 0
			SearchBox.Size = UDim2.new(1, 0, 0.045, 0)
			SearchBox.Font = Enum.Font.GothamSemibold
			SearchBox.PlaceholderColor3 = Color3.fromRGB(255, 255, 255)
			SearchBox.PlaceholderText = "Search bar..."
			SearchBox.Text = ""
			SearchBox.TextColor3 = Color3.fromRGB(255, 255, 255)
			SearchBox.TextScaled = true
			SearchBox.TextSize = 14.000
			SearchBox.TextWrapped = true
			SearchBox.LayoutOrder = 1
			
			Container.Name = "Container"
			Container.Parent = MainFrame
			Container.Active = true
			Container.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			Container.BackgroundTransparency = 0.750
			Container.BorderSizePixel = 0
			Container.Size = UDim2.new(1, 0, 0.5, 0)
			Container.ScrollBarThickness = 5
			Container.VerticalScrollBarPosition = Enum.VerticalScrollBarPosition.Left
			Container.LayoutOrder = 2
			
			Button.Name = "Button"
			Button.Parent = LoganWS
			Button.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			Button.BackgroundTransparency = 0.850
			Button.BorderSizePixel = 0
			Button.Size = UDim2.new(1, 0, 0, 38)
			Button.Font = Enum.Font.GothamSemibold
			Button.Text = "Test"
			Button.TextColor3 = Color3.fromRGB(255, 255, 255)
			Button.TextScaled = true
			Button.TextSize = 14.000
			Button.TextWrapped = true
			
			UIListLayout.Parent = Container
			UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
			UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
			UIListLayout.Padding = UDim.new(0, 5)
			
			UIListLayout2.Parent = MainFrame
			UIListLayout2.HorizontalAlignment = Enum.HorizontalAlignment.Center
			UIListLayout2.SortOrder = Enum.SortOrder.LayoutOrder
			UIListLayout2.Padding = UDim.new(0, 5)
			
			ReverseAnim.Name = "ReverseAnim"
			ReverseAnim.Parent = MainFrame
			ReverseAnim.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			ReverseAnim.BackgroundTransparency = 0.750
			ReverseAnim.BorderColor3 = Color3.fromRGB(27, 42, 53)
			ReverseAnim.BorderSizePixel = 0
			ReverseAnim.LayoutOrder = 4
			ReverseAnim.Size = UDim2.new(0.85, 0, 0.06, 0)
			ReverseAnim.Font = Enum.Font.GothamSemibold
			ReverseAnim.Text = "Reverse animation"
			ReverseAnim.TextColor3 = Color3.fromRGB(255, 255, 255)
			ReverseAnim.TextScaled = true
			ReverseAnim.TextSize = 14.000
			ReverseAnim.TextWrapped = true
			
			StopAnim.Name = "StopAnim"
			StopAnim.Parent = MainFrame
			StopAnim.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			StopAnim.BackgroundTransparency = 0.750
			StopAnim.BorderColor3 = Color3.fromRGB(27, 42, 53)
			StopAnim.BorderSizePixel = 0
			StopAnim.LayoutOrder = 5
			StopAnim.Size = UDim2.new(0.85, 0, 0.06, 0)
			StopAnim.Font = Enum.Font.GothamSemibold
			StopAnim.Text = "Stop animation"
			StopAnim.TextColor3 = Color3.fromRGB(255, 255, 255)
			StopAnim.TextScaled = true
			StopAnim.TextSize = 14.000
			StopAnim.TextWrapped = true
			
			Exit.Name = "Exit"
			Exit.Parent = titleFrame
			Exit.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			Exit.BackgroundTransparency = 1.000
			Exit.Size = UDim2.new(0.1, 0, 0.7, 0)
			Exit.Font = Enum.Font.GothamSemibold
			Exit.Text = "X"
			Exit.TextColor3 = Color3.fromRGB(255, 255, 255)
			Exit.TextScaled = true
			Exit.TextSize = 14.000
			Exit.TextWrapped = true
			Exit.LayoutOrder = 2
			
			SlideBar.Name = "SlideBar"
			SlideBar.Parent = slideFrame
			SlideBar.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			SlideBar.BackgroundTransparency = 0.750
			SlideBar.BorderSizePixel = 0
			SlideBar.Size = UDim2.new(1, 0, 0.3, 0)
			SlideBar.AnchorPoint = Vector2.new(0.5,0.5)
			SlideBar.Position = UDim2.new(0.5,0,0.5,0)
			
			
			SlideButton.Name = "SlideButton"
			SlideButton.Parent = SlideBar
			SlideButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			SlideButton.BorderSizePixel = 0
			SlideButton.Position = UDim2.new(0.5, 0, -1.5, 0)
			SlideButton.Size = UDim2.new(0, 10, 0, 26)
			SlideButton.Font = Enum.Font.SourceSans
			SlideButton.TextColor3 = Color3.fromRGB(0, 0, 0)
			SlideButton.TextSize = 14.000
			SlideButton.TextTransparency = 1.000
			
			MainFrame.Active = true
			MainFrame.Draggable = true
			
			local LayOut = 0
			local CurrentAni = nil
			local neg = false
			
			
			function StopAnims()
				for _,v in pairs(animations) do
					v:Stop()
				end
			end
			
			function LoadAnims()
				for i,v in pairs(animations) do
					local Anim = Instance.new("Animation", LoganWS)
					Anim.AnimationId = "rbxassetid://"..v
					animations[i] = plr.Character.Humanoid:LoadAnimation(Anim)
					CreateButton(i)
				end
			end
			
			function Snap(number, factor)
				if factor == 0 then
					return number
				else
					return math.floor(number/factor+0.5)*factor
				end
			end
			
			function AutoScale()
				local number = (#Container:GetChildren()-1)*38
				number = number + (#Container:GetChildren()-1)*5
				Container.CanvasSize = UDim2.new(0,0,0,number)
			end
			
			
			
			function CreateButton(AnimationName)
				local ButtonClone = Button:Clone()
				ButtonClone.LayoutOrder = LayOut
				LayOut = LayOut + 1
				ButtonClone.Parent = buttonHolder
				ButtonClone.Name = AnimationName
				ButtonClone.Text = AnimationName
				ButtonClone.MouseButton1Click:Connect(function()
					StopAnims()
					CurrentAni = animations[ButtonClone.Name]
					CurrentAni:Play()
				end)
			end
			
			function FindAnim() 
				local text = string.lower(SearchBox.Text)
				if SearchBox.Text == "" or SearchBox.Text == nil then
					for _,v in pairs(buttonHolder:GetChildren()) do
						v.Parent = Container
					end
				else
					for i,v in pairs(buttonHolder:GetChildren()) do
						if string.find(string.lower(v.Name), text) then
							v.Parent = Container
						end
					end
					for i,v in pairs(Container:GetChildren()) do
						if not string.find(string.lower(v.Name), text) and v.Name ~= "UIListLayout" then
							v.Parent = buttonHolder
						end
					end
				end
			end
			
			ReverseAnim.MouseButton1Click:Connect(function()
				neg = not neg
			end)
			StopAnim.MouseButton1Click:Connect(StopAnims)
			PauseAnim.MouseButton1Click:Connect(function()
				plr.Character.Animate.Disabled = true
			end)
			ReplayAnim.MouseButton1Click:Connect(function()
				plr.Character.Animate.Disabled = false
			end)
			
			local TS = game:GetService("TweenService")
			local tweenclose = TS:Create(MainFrame, TweenInfo.new(1), {Size = UDim2.new(0.135, 0, 0.03, 0)})
			local tweenclose2 = TS:Create(titleFrame, TweenInfo.new(1), {Size = UDim2.new(1, 0, 1, 0)})
			local tweenopen = TS:Create(MainFrame, TweenInfo.new(1), {Size = UDim2.new(0.135, 0, 0.6, 0)})
			local tweenopen2 = TS:Create(titleFrame, TweenInfo.new(1), {Size = UDim2.new(1, 0, 0.05, 0)})
			local open = true
			Mini.MouseButton1Click:Connect(function()
				if open then
					Mini.Text = "o"
					for _,v in pairs(MainFrame:GetChildren()) do
						if v.Name ~= titleFrame.Name and not string.find(v.Name, "UI") then
							v.Visible = false
						end
					end
					tweenclose:Play()
					tweenclose2:Play()
				else
					Mini.Text = "-"
					for _,v in pairs(MainFrame:GetChildren()) do
						if not string.find(v.Name, "UI") then
							v.Visible = true
						end
					end
					tweenopen:Play()
					tweenopen2:Play()
				end
				open = not open
			end)
			
			LoadAnims()
			
			
			
			local held = false
			SlideButtonPos = SlideButton.Position
			local UIS = game:GetService("UserInputService")
			local RuS = game:GetService("RunService")
			local step = 0.01
			local percentage = 0
			
			UIS.InputEnded:connect(function(input, processed)
				if input.UserInputType == Enum.UserInputType.MouseButton1 then
					held = false
				end
			end)
			
			SlideButton.MouseButton1Down:Connect(function()
				held = true
			end)
			
			local con = RuS.RenderStepped:connect(function()
				if held then
					local MousePos = UIS:GetMouseLocation().X
					local BtnPos = SlideButton.Position
					local SliderSize = SlideBar.AbsoluteSize.X
					local SliderPos = SlideBar.AbsolutePosition.X
					local pos = Snap((MousePos-SliderPos)/SliderSize,step)
					percentage = math.clamp(pos,0,0.96)
					SlideButton.Position = UDim2.new(percentage,0,BtnPos.Y.Scale, BtnPos.Y.Offset)
				end
				local axis = SlideButton.Position.X.Scale*2
				if neg then
					axis = -axis
				end
				if CurrentAni ~= nil then
					CurrentAni:AdjustSpeed(axis)
				end
				FindAnim()
				AutoScale()
			end)
			
			Exit.MouseButton1Click:Connect(function()
				StopAnims()
				plr.Character.Animate.Disabled = false
				Animations:Destroy()
				LoganWS:Destroy()
				con:Disconnect()
			end)
			end)
			
				Misc:Button("Animations (Blox fruit)",function()
			local animations = {
				["SuperHumanV2Z"] = 10275674268,
				["SuperHumanV2C"] = 10275680692,
				["SuperHumanV2X"] = 10275676392,
				["SuperHuman ldle"] = 9841361789,
				["DarkBladeSkillZHold"] = 5174585335,
				["DarkBladeSkillZ"] = 5174526481,
				["DarkBladeSkillX"] = 5174270737,
				["TrideThrow"] = 3341408890,
				["TridentThrow"] = 8349216001,
				["Run"] = 9884584522,
				["fire throw Dai Enkai"] = 2797894116,
				["SitV2"] = 2506281703,
				["Hold Trident ldle"] = 10375964637,
				["TridenSend"] = 10275680692,
				["TridenSend"] = 10275680692,
				["tridentStab"] = 6515126214,
				["Hold Trident 1"] = 10375957814,
				["Hold Trident 2"] = 10375959340,
				["Hold Trident 3"] = 10375962019,
				["Hold Trident 4"] = 10375963331,
				["GravC ldle"] = 10129711980,
				["SoulZHold"] = 3305041045,
				["SoulZ"] = 3304940294,
				["GravC 1"] = 10129707298,
				["GravC 2"] = 10129708538,
				["GravC 3"] = 10129709852,
				["GravC 4"] = 10129710763,
				["Triple"] = 4535879191,
				["Triple 2nd Ability"] = 4535877786,
				["HookedBladersX"] = 7302432705,
				["toranadoscythe"] = 7846555569,
				["BombMove1Startup"] = 9906540249,
				["BombMove1Attack"] = 9906525070,
				["lmported Animation Clip"] = 9908589111,
				["DonutRolLoop"] = 4490571442,
				["DragonClawBreath"] = 4403107485,
				["ShadowC"] = 7860960861,
				["ShadowV"] = 7860962774,
				["stringflight"] = 6033403573,
				["Walk"] = 9802959564,
				["partyTalbleStart"] = 10581386092,
				["partyTalbleLoop"] = 10581389297,
				["partyTalbleEnd"] = 10581396234,
				["consussSpin"] = 10581410118,
				["consussStart"] = 10581404276,
				["KickBarryage"] = 10581399083,
				["diavloActivate"] = 10581401357,
				["Gatling Startup"] = 10166333910,
				["Gatling AttactLoop"] = 10166337224,
				["Gatling End"] = 10166340559,
				["Gatling End"] = 10166340559,
				["phoenixswing"] = 2908113208,
				["phoenixhold"] = 2908113768,
				["TransformRubber"] = 10166634301,
				["Midnight Blade 1"] = 10166200938,
				["Midnight Blade 2"] = 10375981285,
				["Midnight Blade 3"] = 10375982688,
				["Midnight Blade 4"] = 10375984145,
				["taclke hold frame_StucksDucks"] = 9868735722,
				["taclke attack_StuckDucks"] = 9868736872,
				["360 slashes end_StucksDuck"] = 9868496368,
				["taclke attack_StuckDucks"] = 9868736872,
				["fistSlashesAttackLoo_StuckDuck"] = 9874750712,
				["fightstart"] = 9868502797,
				["loopfight"] = 9868499868,
				["Fall"] = 9811521002,
				["flight loop_StucksDucks"] = 9868618350,
				["fire throw Dai Enkai"] = 2797894116,
				["TransformRubber"] = 10166634301,
				["stringflight"] = 6033403573,
				["TransformRubber"] = 10166634301,
				["Geppo Left Foot"] = 9799138662,
				["Geppo Right Foot"] = 9799139408,
				["Double jump2"] = 9886242181,
				["ShadowX"] = 7846478951
				}
			
			local plr = game.Players.LocalPlayer
			local LoganWS = Instance.new('Folder', game)
			LoganWS.Name = 'LoganWS'
			
			local buttonHolder = Instance.new('Folder', LoganWS)
			buttonHolder.Name = "Buttons"
			
			
			local Animations = Instance.new("ScreenGui")
			local MainFrame = Instance.new("Frame")
			local UIGradient = Instance.new("UIGradient")
			local Title = Instance.new("TextLabel")
			local SearchBox = Instance.new("TextBox")
			local Container = Instance.new("ScrollingFrame")
			local Button = Instance.new("TextButton")
			local UIListLayout = Instance.new("UIListLayout")
			local UIListLayout2 = Instance.new("UIListLayout")
			local UIListLayout3 = Instance.new("UIListLayout")
			local StopAnim = Instance.new("TextButton")
			local PauseAnim = Instance.new("TextButton")
			local ReplayAnim = Instance.new("TextButton")
			local ReverseAnim = Instance.new("TextButton")
			local Exit = Instance.new("TextButton")
			local Mini = Instance.new("TextButton")
			local titleFrame = Instance.new("Frame")
			local slideFrame = Instance.new("Frame")
			local SlideBar = Instance.new("Frame")
			local SlideButton = Instance.new("TextButton")
			local creds = Instance.new("TextLabel")
			
			Animations.Name = "Animations"
			Animations.Parent = plr:WaitForChild("PlayerGui")
			
			MainFrame.Name = "MainFrame"
			MainFrame.Parent = Animations
			MainFrame.BackgroundColor3 = Color3.fromRGB(195, 195, 195)
			MainFrame.BorderColor3 = Color3.fromRGB(195, 195, 195)
			MainFrame.BorderSizePixel = 1
			MainFrame.Position = UDim2.new(0.4, 0, 0.2, 0)
			MainFrame.Size = UDim2.new(0.1, 0, 0.415, 0)
						spawn(function()
						while wait() do
							pcall(function()
								wait(0.1) 
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 0, 0)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 155, 0)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 255, 0)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(0, 255, 0)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(0, 255, 255)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(0, 155, 255)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 0, 255)}
								):Play() 
								wait(.5)            
								game:GetService('TweenService'):Create(
									Title,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.InOut),
									{TextColor3 = Color3.fromRGB(255, 0, 155)}
								):Play() 
								wait(.5)
							end)
						end
					end)
			
			titleFrame.Name = "TitleFrame"
			titleFrame.Parent = MainFrame
			titleFrame.BorderSizePixel = 0
			titleFrame.LayoutOrder = 0
			titleFrame.BackgroundTransparency = 1
			titleFrame.Size = UDim2.new(1, 0, 0.05, 0)
			
			slideFrame.Name = "SlideFrame"
			slideFrame.Parent = MainFrame
			slideFrame.BorderSizePixel = 0
			slideFrame.LayoutOrder = 3
			slideFrame.BackgroundTransparency = 1
			slideFrame.Size = UDim2.new(1, 0, 0.01, 0)
			
			UIListLayout3.Parent = titleFrame
			UIListLayout3.FillDirection = Enum.FillDirection.Horizontal
			UIListLayout3.SortOrder = Enum.SortOrder.LayoutOrder
			
			UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(102, 45, 113)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(197, 66, 110))}
			UIGradient.Parent = MainFrame
			
			Title.Name = "Title"
			Title.Parent = titleFrame
			Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			Title.BackgroundTransparency = 1.000
			Title.Size = UDim2.new(1, 0, 1, 0)
			Title.Font = Enum.Font.GothamSemibold
			Title.Text = "Animation Effect"
			Title.TextColor3 = Color3.fromRGB(255, 255, 255)
			Title.TextScaled = true
			Title.TextSize = 14.000
			Title.TextWrapped = true
			Title.LayoutOrder = 0
			
			SearchBox.Name = "SearchBox"
			SearchBox.Parent = MainFrame
			SearchBox.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			SearchBox.BackgroundTransparency = 0.750
			SearchBox.BorderSizePixel = 0
			SearchBox.Size = UDim2.new(1, 0, 0.045, 0)
			SearchBox.Font = Enum.Font.GothamSemibold
			SearchBox.PlaceholderColor3 = Color3.fromRGB(255, 255, 255)
			SearchBox.PlaceholderText = "Search bar..."
			SearchBox.Text = ""
			SearchBox.TextColor3 = Color3.fromRGB(255, 255, 255)
			SearchBox.TextScaled = true
			SearchBox.TextSize = 14.000
			SearchBox.TextWrapped = true
			SearchBox.LayoutOrder = 1
			
			Container.Name = "Container"
			Container.Parent = MainFrame
			Container.Active = true
			Container.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			Container.BackgroundTransparency = 0.750
			Container.BorderSizePixel = 0
			Container.Size = UDim2.new(1, 0, 0.5, 0)
			Container.ScrollBarThickness = 5
			Container.VerticalScrollBarPosition = Enum.VerticalScrollBarPosition.Left
			Container.LayoutOrder = 2
			
			Button.Name = "Button"
			Button.Parent = LoganWS
			Button.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			Button.BackgroundTransparency = 0.850
			Button.BorderSizePixel = 0
			Button.Size = UDim2.new(1, 0, 0, 38)
			Button.Font = Enum.Font.GothamSemibold
			Button.Text = "Test"
			Button.TextColor3 = Color3.fromRGB(255, 255, 255)
			Button.TextScaled = true
			Button.TextSize = 14.000
			Button.TextWrapped = true
			
			UIListLayout.Parent = Container
			UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
			UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
			UIListLayout.Padding = UDim.new(0, 5)
			
			UIListLayout2.Parent = MainFrame
			UIListLayout2.HorizontalAlignment = Enum.HorizontalAlignment.Center
			UIListLayout2.SortOrder = Enum.SortOrder.LayoutOrder
			UIListLayout2.Padding = UDim.new(0, 5)
			
			ReverseAnim.Name = "ReverseAnim"
			ReverseAnim.Parent = MainFrame
			ReverseAnim.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			ReverseAnim.BackgroundTransparency = 0.750
			ReverseAnim.BorderColor3 = Color3.fromRGB(27, 42, 53)
			ReverseAnim.BorderSizePixel = 0
			ReverseAnim.LayoutOrder = 4
			ReverseAnim.Size = UDim2.new(0.85, 0, 0.06, 0)
			ReverseAnim.Font = Enum.Font.GothamSemibold
			ReverseAnim.Text = "Reverse animation"
			ReverseAnim.TextColor3 = Color3.fromRGB(255, 255, 255)
			ReverseAnim.TextScaled = true
			ReverseAnim.TextSize = 14.000
			ReverseAnim.TextWrapped = true
			
			StopAnim.Name = "StopAnim"
			StopAnim.Parent = MainFrame
			StopAnim.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			StopAnim.BackgroundTransparency = 0.750
			StopAnim.BorderColor3 = Color3.fromRGB(27, 42, 53)
			StopAnim.BorderSizePixel = 0
			StopAnim.LayoutOrder = 5
			StopAnim.Size = UDim2.new(0.85, 0, 0.06, 0)
			StopAnim.Font = Enum.Font.GothamSemibold
			StopAnim.Text = "Stop animation"
			StopAnim.TextColor3 = Color3.fromRGB(255, 255, 255)
			StopAnim.TextScaled = true
			StopAnim.TextSize = 14.000
			StopAnim.TextWrapped = true
			
			Exit.Name = "Exit"
			Exit.Parent = titleFrame
			Exit.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			Exit.BackgroundTransparency = 1.000
			Exit.Size = UDim2.new(0.1, 0, 0.7, 0)
			Exit.Font = Enum.Font.GothamSemibold
			Exit.Text = "X"
			Exit.TextColor3 = Color3.fromRGB(255, 255, 255)
			Exit.TextScaled = true
			Exit.TextSize = 14.000
			Exit.TextWrapped = true
			Exit.LayoutOrder = 2
			
			SlideBar.Name = "SlideBar"
			SlideBar.Parent = slideFrame
			SlideBar.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			SlideBar.BackgroundTransparency = 0.750
			SlideBar.BorderSizePixel = 0
			SlideBar.Size = UDim2.new(1, 0, 0.3, 0)
			SlideBar.AnchorPoint = Vector2.new(0.5,0.5)
			SlideBar.Position = UDim2.new(0.5,0,0.5,0)
			
			
			SlideButton.Name = "SlideButton"
			SlideButton.Parent = SlideBar
			SlideButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			SlideButton.BorderSizePixel = 0
			SlideButton.Position = UDim2.new(0.5, 0, -1.5, 0)
			SlideButton.Size = UDim2.new(0, 10, 0, 26)
			SlideButton.Font = Enum.Font.SourceSans
			SlideButton.TextColor3 = Color3.fromRGB(0, 0, 0)
			SlideButton.TextSize = 14.000
			SlideButton.TextTransparency = 1.000
			
			MainFrame.Active = true
			MainFrame.Draggable = true
			
			local LayOut = 0
			local CurrentAni = nil
			local neg = false
			
			
			function StopAnims()
				for _,v in pairs(animations) do
					v:Stop()
				end
			end
			
			function LoadAnims()
				for i,v in pairs(animations) do
					local Anim = Instance.new("Animation", LoganWS)
					Anim.AnimationId = "rbxassetid://"..v
					animations[i] = plr.Character.Humanoid:LoadAnimation(Anim)
					CreateButton(i)
				end
			end
			
			function Snap(number, factor)
				if factor == 0 then
					return number
				else
					return math.floor(number/factor+0.5)*factor
				end
			end
			
			function AutoScale()
				local number = (#Container:GetChildren()-1)*38
				number = number + (#Container:GetChildren()-1)*5
				Container.CanvasSize = UDim2.new(0,0,0,number)
			end
			
			
			
			function CreateButton(AnimationName)
				local ButtonClone = Button:Clone()
				ButtonClone.LayoutOrder = LayOut
				LayOut = LayOut + 1
				ButtonClone.Parent = buttonHolder
				ButtonClone.Name = AnimationName
				ButtonClone.Text = AnimationName
				ButtonClone.MouseButton1Click:Connect(function()
					StopAnims()
					CurrentAni = animations[ButtonClone.Name]
					CurrentAni:Play()
				end)
			end
			
			function FindAnim() 
				local text = string.lower(SearchBox.Text)
				if SearchBox.Text == "" or SearchBox.Text == nil then
					for _,v in pairs(buttonHolder:GetChildren()) do
						v.Parent = Container
					end
				else
					for i,v in pairs(buttonHolder:GetChildren()) do
						if string.find(string.lower(v.Name), text) then
							v.Parent = Container
						end
					end
					for i,v in pairs(Container:GetChildren()) do
						if not string.find(string.lower(v.Name), text) and v.Name ~= "UIListLayout" then
							v.Parent = buttonHolder
						end
					end
				end
			end
			
			ReverseAnim.MouseButton1Click:Connect(function()
				neg = not neg
			end)
			StopAnim.MouseButton1Click:Connect(StopAnims)
			PauseAnim.MouseButton1Click:Connect(function()
				plr.Character.Animate.Disabled = true
			end)
			ReplayAnim.MouseButton1Click:Connect(function()
				plr.Character.Animate.Disabled = false
			end)
			
			local TS = game:GetService("TweenService")
			local tweenclose = TS:Create(MainFrame, TweenInfo.new(1), {Size = UDim2.new(0.135, 0, 0.03, 0)})
			local tweenclose2 = TS:Create(titleFrame, TweenInfo.new(1), {Size = UDim2.new(1, 0, 1, 0)})
			local tweenopen = TS:Create(MainFrame, TweenInfo.new(1), {Size = UDim2.new(0.135, 0, 0.6, 0)})
			local tweenopen2 = TS:Create(titleFrame, TweenInfo.new(1), {Size = UDim2.new(1, 0, 0.05, 0)})
			local open = true
			Mini.MouseButton1Click:Connect(function()
				if open then
					Mini.Text = "o"
					for _,v in pairs(MainFrame:GetChildren()) do
						if v.Name ~= titleFrame.Name and not string.find(v.Name, "UI") then
							v.Visible = false
						end
					end
					tweenclose:Play()
					tweenclose2:Play()
				else
					Mini.Text = "-"
					for _,v in pairs(MainFrame:GetChildren()) do
						if not string.find(v.Name, "UI") then
							v.Visible = true
						end
					end
					tweenopen:Play()
					tweenopen2:Play()
				end
				open = not open
			end)
			
			LoadAnims()
			
			
			
			local held = false
			SlideButtonPos = SlideButton.Position
			local UIS = game:GetService("UserInputService")
			local RuS = game:GetService("RunService")
			local step = 0.01
			local percentage = 0
			
			UIS.InputEnded:connect(function(input, processed)
				if input.UserInputType == Enum.UserInputType.MouseButton1 then
					held = false
				end
			end)
			
			SlideButton.MouseButton1Down:Connect(function()
				held = true
			end)
			
			local con = RuS.RenderStepped:connect(function()
				if held then
					local MousePos = UIS:GetMouseLocation().X
					local BtnPos = SlideButton.Position
					local SliderSize = SlideBar.AbsoluteSize.X
					local SliderPos = SlideBar.AbsolutePosition.X
					local pos = Snap((MousePos-SliderPos)/SliderSize,step)
					percentage = math.clamp(pos,0,0.96)
					SlideButton.Position = UDim2.new(percentage,0,BtnPos.Y.Scale, BtnPos.Y.Offset)
				end
				local axis = SlideButton.Position.X.Scale*2
				if neg then
					axis = -axis
				end
				if CurrentAni ~= nil then
					CurrentAni:AdjustSpeed(axis)
				end
				FindAnim()
				AutoScale()
			end)
			
			Exit.MouseButton1Click:Connect(function()
				StopAnims()
				plr.Character.Animate.Disabled = false
				Animations:Destroy()
				LoganWS:Destroy()
				con:Disconnect()
			end)
			end)
	
			Misc:Button("Max Zoom", function()
				game.Players.LocalPlayer.CameraMaxZoomDistance = math.huge
			end)
		
			Misc:Button("Buddha Big", function()
		local LocalPlayer = game:GetService("Players").LocalPlayer
		local Character = LocalPlayer.Character
		local Humanoid = Character:FindFirstChildOfClass("Humanoid")
		
		function rm()
			for i,v in pairs(Character:GetDescendants()) do
				if v:IsA("BasePart") then
					if v.Name == "Handle" or v.Name == "Head" then
						if Character.Head:FindFirstChild("OriginalSize") then
							Character.Head.OriginalSize:Destroy()
						end
					else
						for i,cav in pairs(v:GetDescendants()) do
							if cav:IsA("Attachment") then
								if cav:FindFirstChild("OriginalPosition") then
									cav.OriginalPosition:Destroy()  
								end
							end
						end
						v:FindFirstChild("OriginalSize"):Destroy()
						if v:FindFirstChild("AvatarPartScaleType") then
							v:FindFirstChild("AvatarPartScaleType"):Destroy()
						end
					end
				end
			end
		end
		
		rm()
		wait(0.5)
		Humanoid:FindFirstChild("BodyProportionScale"):Destroy()
		wait(1)
		end)
		
		Misc:Button("Unlock Portal",function()
			_G.UnlockPortal = true
		end)

		spawn(function()
			while wait() do
				pcall(function()
					if _G.UnlockPortal == true then
						for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Notifications:GetChildren()) do
							if v.Name == "NotificationTemplate" then
								if string.find(v.Text,"cannot") then
									v:Destroy()
								end
							end
						end
					end
				end)
			end
		end)
		
		spawn(function()
			while wait() do
				pcall(function()
					if _G.UnlockPortal == true then
						CastlePostoMansion = CFrame.new(-5084.8447265625, 316.48101806641, -3145.3752441406)
						MansiontoCastlePos = CFrame.new(-12464.596679688, 376.30590820312, -7567.2626953125)
						Castletophydra = CFrame.new(-5095.33984375, 316.48101806641, -3168.3134765625)
						HydratoCastle = CFrame.new(5741.869140625, 611.94750976562, -282.61154174805)
						if (CastlePostoMansion.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 8 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-12471.169921875, 374.94024658203, -7551.677734375))
						end
						if (MansiontoCastlePos.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 8 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-5072.08984375, 314.5412902832, -3151.1098632812))
						end
						if (Castletophydra.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 8 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(5748.7587890625, 610.44982910156, -267.81704711914))
						end
						if (HydratoCastle.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 8 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-5072.08984375, 314.5412902832, -3151.1098632812))
						end
					end
				end)
			end
		end)

		Misc:Button("Unlock Doflamingo",function()
			_G.UnlockDo = true
		end)

		spawn(function()
			while wait() do
				pcall(function()
					if _G.UnlockDo == true then
						for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Notifications:GetChildren()) do
							if v.Name == "NotificationTemplate" then
								if string.find(v.Text,"You cannot access this area yet.") then
									v:Destroy()
								end
							end
						end
					end
				end)
			end
		end)
		
		spawn(function()
			while wait() do
				pcall(function()
					if _G.UnlockDo == true then
						Doflamingo = CFrame.new(-287.0097351074219, 305.98590087890625, 592.8171997070312)
						if (Doflamingo.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 8 then
							game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(2285.079345703125, 15.277364730834961, 910.3013305664062))
						end
					end
				end)
			end
		end)
	
			Misc:Seperator("Kaitun Image")
	
			Misc:Button("Kaitun Cap", function(value)
				local cac = require(game:GetService("Players").LocalPlayer.PlayerGui.Main.UIController.Inventory)
				local Inventory = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getInventory")
				local Items = {}
				local RaityLevel = {"Mythical","Legendary","Rare","Uncommon","Common"}
				local RaityColor =  {
					["Common"] = Color3.fromRGB(179, 179, 179),
					["Uncommon"] = Color3.fromRGB(92, 140, 211),
					["Rare"] =  Color3.fromRGB(140, 82, 255),
					["Legendary"] = Color3.fromRGB(213, 43, 228) ,
					["Mythical"] =  Color3.fromRGB(238, 47, 50)
				}
				function GetRaity(color)
					for k,v in pairs(RaityColor) do 
						if v==color then return k end
					end
				end
		
				for k,v in pairs(Inventory) do 
					Items[v.Name] = v
				end
		
				local total = #getupvalue(cac.UpdateRender,4)
				local rac = {}
				local allitem = {}
				local total2 = 0
				while total2<total do 
					local i = 0
					while i < 25000 and total2<total do 
						game:GetService("Players").LocalPlayer.PlayerGui.Main.InventoryContainer.Right.Content.ScrollingFrame.CanvasPosition = Vector2.new(0,i)
						for k,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Main.InventoryContainer.Right.Content.ScrollingFrame.Frame:GetChildren()) do 
							if v:IsA("Frame") and not rac[v.ItemName.Text] and v.ItemName.Visible==true then 
								local vaihuhu = GetRaity(v.Background.BackgroundColor3)
								if vaihuhu then
									print("Rac")
									if not allitem[vaihuhu] then 
										allitem[vaihuhu] = {}
									end
									table.insert(allitem[vaihuhu],v:Clone())
								end
								total2=total2+1
								rac[v.ItemName.Text] = true
							end
						end
						i=i+20
					end
					wait()
				end
				function GetXY(vec) 
					return vec*100
				end
		
				local tvk = Instance.new("UIListLayout")
				tvk.FillDirection = Enum.FillDirection.Vertical
				tvk.SortOrder = 2
				tvk.Padding = UDim.new(0,10)
		
				local Left = Instance.new("Frame",game.Players.LocalPlayer.PlayerGui.BubbleChat)
				Left.BackgroundTransparency = 1
				Left.Size = UDim2.new(.5,0,1,0) 
				tvk.Parent = Left
		
				local Right = Instance.new("Frame",game.Players.LocalPlayer.PlayerGui.BubbleChat)
				Right.BackgroundTransparency = 1
				Right.Size = UDim2.new(.5,0,1,0) 
				Right.Position = UDim2.new(.6,0,0,0)
				tvk:Clone().Parent = Right

				for k,v in pairs(allitem) do 
					local cac = Instance.new("Frame",Left)
					cac.BackgroundTransparency = 1
					cac.Size = UDim2.new(1,0,0,0) 
					cac.LayoutOrder = table.find(RaityLevel,k)
		
					local cac2 = Instance.new("Frame",Right)
					cac2.BackgroundTransparency = 1
					cac2.Size = UDim2.new(1,0,0,0) 
					cac2.LayoutOrder = table.find(RaityLevel,k)
		
					local tvk = Instance.new("UIGridLayout",cac)
					tvk.CellPadding = UDim2.new(.005,0,.005,0)
					tvk.CellSize =  UDim2.new(0,70,0,70)
					tvk.FillDirectionMaxCells = 100
					tvk.FillDirection = Enum.FillDirection.Horizontal
		
					local ccc = tvk:Clone()
					ccc.Parent = cac2
					for k,v in pairs(v) do wait(0.1)
						if Items[v.ItemName.Text] and Items[v.ItemName.Text].Mastery then 
							if v.ItemLine2.Text~="Accessory" then 
								local bucac = v.ItemName:Clone()
								bucac.BackgroundTransparency = 1
								bucac.TextSize = 10
								bucac.TextXAlignment  = 2
								bucac.TextYAlignment  = 2
								bucac.ZIndex  = 5
								bucac.Text = Items[v.ItemName.Text].Mastery
								bucac.Size = UDim2.new(.5,0,.5,0)
								bucac.Position = UDim2.new(.5,0,.5,0)
								bucac.Parent = v
							end
							v.Parent = cac
						elseif v.ItemLine2.Text == "Blox Fruit" then 
							v.Parent = cac2
						end
					end
					cac.AutomaticSize = 2
					cac2.AutomaticSize = 2
				end
				local ListHuhu = {
					["Superhuman"] = Vector2.new(3,2),
					["GodHuman"] = Vector2.new(3,2),
					["DeathStep"] = Vector2.new(4,3),
					["ElectricClaw"] = Vector2.new(2,0),
					["SharkmanKarate"] = Vector2.new(0,0),
					["DragonTalon"] = Vector2.new(1,5)
				}
				local MeleeG = Instance.new("Frame",Left)
				MeleeG.BackgroundTransparency = 1
				MeleeG.Size = UDim2.new(1,0,0,0) 
				MeleeG.LayoutOrder = table.find(RaityLevel,k)
				MeleeG.AutomaticSize=2
				MeleeG.LayoutOrder = 100
				local tvk = Instance.new("UIGridLayout",MeleeG)
				tvk.CellPadding = UDim2.new(.005,0,.005,0)
				tvk.CellSize =  UDim2.new(0,70,0,70)
				tvk.FillDirectionMaxCells = 100
				tvk.FillDirection = Enum.FillDirection.Horizontal
		
				local cac = {"Superhuman","ElectricClaw","DragonTalon","SharkmanKarate","DeathStep","GodHuman"}
				for k,v in pairs(cac) do
					if ListHuhu[v] and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buy"..v,true) == 1 then 
						local huhu = Instance.new("ImageLabel",MeleeG)
						huhu.Image = "rbxassetid://9945562382"
						huhu.ImageRectSize = Vector2.new(100,100)
						huhu.ImageRectOffset = ListHuhu[v]*100
					end
				end
				function formatNumber(v)
					return tostring(v):reverse():gsub("%d%d%d", "%1,"):reverse():gsub("^,", "")
				end
			end)
		
			Misc:Button("Remove Kaitun Cap",function()
				for _,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.BubbleChat:GetDescendants()) do
					v:Destroy()
				end
			end)
			
			Misc:Seperator("State")
			
			Misc:Dropdown("Select Haki State",{"State 0","State 1","State 2","State 3","State 4","State 5"},function(value)
				_G.SelectStateHaki = value
			end)
			
			Misc:Button("Change Buso Haki State",function()
				if _G.SelectStateHaki == "State 0" then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",0)
				elseif _G.SelectStateHaki == "State 1" then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",1)
				elseif _G.SelectStateHaki == "State 2" then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",2)
				elseif _G.SelectStateHaki == "State 3" then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",3)
				elseif _G.SelectStateHaki == "State 4" then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",4)
				elseif _G.SelectStateHaki == "State 5" then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",5)
				end
			end)
			
			Misc:Seperator("Boost FPS")
			
			local a = game.Lighting
			local c = Instance.new("ColorCorrectionEffect", a)
			local e = Instance.new("ColorCorrectionEffect", a)
			OldAmbient = a.Ambient
			OldBrightness = a.Brightness
			OldColorShift_Top = a.ColorShift_Top
			OldBrightnessc = c.Brightness
			OldContrastc = c.Contrast
			OldTintColorc = c.TintColor
			OldTintColore = e.TintColor
		
			Misc:Toggle("RTX Mode",_G.RTXMode,function(value)
				_G.RTXMode = value
				if not _G.RTXMode then return end
				while _G.RTXMode do wait()
					a.Ambient = Color3.fromRGB(33, 33, 33)
					a.Brightness = 0.3
					c.Brightness = 0.176
					c.Contrast = 0.39
					c.TintColor = Color3.fromRGB(217, 145, 57)
					game.Lighting.FogEnd = 999
					if not game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("PointLight") then
						local a2 = Instance.new("PointLight")
						a2.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						a2.Range = 15
						a2.Color = Color3.fromRGB(217, 145, 57)
					end
					if not _G.RTXMode then
						a.Ambient = OldAmbient
						a.Brightness = OldBrightness
						a.ColorShift_Top = OldColorShift_Top
						c.Contrast = OldContrastc
						c.Brightness = OldBrightnessc
						c.TintColor = OldTintColorc
						e.TintColor = OldTintColore
						game.Lighting.FogEnd = 2500
						game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("PointLight"):Destroy()
					end
				end
			end)
		  
			Misc:Button("FPS Boost",function()
				pcall(function()
					game:GetService("Lighting").FantasySky:Destroy()
					local g = game
					local w = g.Workspace
					local l = g.Lighting
					local t = w.Terrain
					t.WaterWaveSize = 0
					t.WaterWaveSpeed = 0
					t.WaterReflectance = 0
					t.WaterTransparency = 0
					l.GlobalShadows = false
					l.FogEnd = 9e9
					l.Brightness = 0
					settings().Rendering.QualityLevel = "Level01"
					for i, v in pairs(g:GetDescendants()) do
						if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then 
							v.Material = "Plastic"
							v.Reflectance = 0
						elseif v:IsA("Decal") or v:IsA("Texture") then
							v.Transparency = 1
						elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
							v.Lifetime = NumberRange.new(0)
						elseif v:IsA("Explosion") then
							v.BlastPressure = 1
							v.BlastRadius = 1
						elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
							v.Enabled = false
						elseif v:IsA("MeshPart") then
							v.Material = "Plastic"
							v.Reflectance = 0
							v.TextureID = 10385902758728957
						end
					end
					for i, e in pairs(l:GetChildren()) do
						if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
							e.Enabled = false
						end
					end
					for i, v in pairs(game:GetService("Workspace").Camera:GetDescendants()) do
						if v.Name == ("Water;") then
							v.Transparency = 1
							v.Material = "Plastic"
						end
					end
				end)
			end)
			
			Misc:Button("Unlock FPS",function()
				setfpscap(120)
			end)
		
			Misc:Button("FPS delete color",function()
		for _,v in pairs(workspace:GetDescendants()) do
		if v.ClassName == "Part"
		or v.ClassName == "SpawnLocation"
		or v.ClassName == "WedgePart"
		or v.ClassName == "Terrain"
		or v.ClassName == "MeshPart" then
		v.BrickColor = BrickColor.new(155, 155, 155)
		v.Material = "Plastic"
		end
		end
		end)
		
			Misc:Button("FPS Fast Mode",function()
		for _,v in pairs(workspace:GetDescendants()) do
		if v.ClassName == "Part"
		or v.ClassName == "SpawnLocation"
		or v.ClassName == "WedgePart"
		or v.ClassName == "Terrain"
		or v.ClassName == "MeshPart" then
		v.Material = "Plastic"
		end
		end
		end)
	
			Misc:Slider("FPS Lock",0,499,60,function(K)setfpscap(tonumber(K));
			end)
			
			Misc:Seperator("Abilities")
	
			Misc:Toggle("Auto Active Race",_G.AutoAgility,function(value)
				_G.AutoAgility = value
			end)
			
			spawn(function()
				pcall(function()
					while wait() do
						if _G.AutoAgility then
							game:GetService("ReplicatedStorage").Remotes.CommE:FireServer("ActivateAbility")
						end
					end
				end)
			end)
		
			if game.workspace:FindFirstChild("WaterWalk") then
				game.workspace:FindFirstChild("WaterWalk"):Destroy()
			end
			platform = Instance.new("Part")
			platform.Name = "WaterWalk"
			platform.Size = Vector3.new(math.huge, 1, math.huge)
			platform.Transparency = 1
			platform.Anchored = true
			platform.Parent = game.workspace

		 Misc:Toggle("Water Walk",waterwalk,function(value)
				WaterWalk = value
			end)
		
			spawn(function()
				while wait() do
					if WaterWalk then
						platform.CanCollide = true
						platform.Position = Vector3.new(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position.X,game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position.Y * 0 -5, game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position.Z)
					else
						platform.CanCollide = false
						platform.Position = Vector3.new(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position.X,game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position.Y * 0 -6, game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position.Z)
					end
				end
			end)

			Misc:Toggle("Ability Infinite",false,function(infA)
				if infA then
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
						local Agility = game:GetService("ReplicatedStorage").FX["Agility"]:Clone()
					Agility.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
				else
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
					game:GetService("Players").LocalPlayer.Character.HumanoidRootPart["Agility"]:Destroy()
				end
				end)
					
				Misc:Toggle("Obversation Range Infinite",getgenv().InfiniteObRange,function(value)
						getgenv().InfiniteObRange = value
						local VS = game:GetService("Players").LocalPlayer.VisionRadius.Value
						while getgenv().InfiniteObRange do
							wait()
							local player = game:GetService("Players").LocalPlayer
							local char = player.Character
							local VisionRadius = player.VisionRadius
							if player then
								if char.Humanoid.Health <= 0 then 
									wait(5) 
								end
								VisionRadius.Value = math.huge
							elseif getgenv().InfiniteObRange == false and player then
								VisionRadius.Value = VS
							end
						end
					end)
				  
					Misc:Toggle("Jump Infinite", nil, function(State)
				Infinite = State
				game:GetService("UserInputService").JumpRequest:connect(function()
					if Infinite then
						game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
					end
				end) 
				end)	
		
			Misc:Seperator("Highlight")

		Misc:Toggle("Show Chat disabled", _G.chat, function(value)
			_G.chat = value
			if _G.chat == true then
		local StarterGui = game:GetService('StarterGui')
		StarterGui:SetCoreGuiEnabled(Enum.CoreGuiType.Chat, false)    
		elseif _G.chat == false then
		local StarterGui = game:GetService('StarterGui')
		StarterGui:SetCoreGuiEnabled(Enum.CoreGuiType.Chat, true)    
		end
		  end)
		
		  Misc:Toggle("Show leaderboard disabled", _G.leaderboard, function(a)
			_G.leaderboard = a
			if _G.leaderboard == true then
		local StarterGui = game:GetService('StarterGui')
		game:GetService('StarterGui'):SetCoreGuiEnabled(Enum.CoreGuiType.PlayerList, false)   
		elseif _G.leaderboard == false then
		local StarterGui = game:GetService('StarterGui')
		game:GetService('StarterGui'):SetCoreGuiEnabled(Enum.CoreGuiType.PlayerList, true)   
		end
		  end)
	
			Misc:Toggle("Highlight Mode",false,function(value)
				if value == true then
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Beli.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.HP.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.StatsButton.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.ShopButton.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Level.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Code.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Settings.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Mute.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.MenuButton.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Energy.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Compass.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.InventoryButton.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.HomeButton.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.AlliesButton.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Quest.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Chat.Frame.Visible = false
					game:GetService("Players")["LocalPlayer"].PlayerGui.Backpack.Hotbar.Visible = false
				else          
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Beli.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.HP.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.StatsButton.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.ShopButton.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Level.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Code.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Settings.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Mute.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Energy.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.MenuButton.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Compass.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.InventoryButton.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.HomeButton.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.AlliesButton.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Quest.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Backpack.Hotbar.Visible = true
					game:GetService("Players")["LocalPlayer"].PlayerGui.Chat.Frame.Visible = true
				end
			end)
		
		Misc:Toggle("Graphic",false,function(v)
					if v then
						getgenv().mode = "Autumn" -- Choose from Summer and Autumn
						local a = game.Lighting
						a.Ambient = Color3.fromRGB(33, 33, 33)
						a.Brightness = 0.3
						a.ColorShift_Bottom = Color3.fromRGB(0, 0, 0)
						a.ColorShift_Top = Color3.fromRGB(255, 247, 237)
						a.EnvironmentDiffuseScale = 0.105
						a.EnvironmentSpecularScale = 0.522
						a.GlobalShadows = true
						a.OutdoorAmbient = Color3.fromRGB(51, 54, 67)
						a.ShadowSoftness = 0.04
						a.GeographicLatitude = -15.525
						a.ExposureCompensation = 0.75
						local b = Instance.new("BloomEffect", a)
						b.Name = "BloomEffect_Graphic"
						b.Enabled = true
						b.Intensity = 0.04
						b.Size = 1900
						b.Threshold = 0.915
						local c = Instance.new("ColorCorrectionEffect", a)
						c.Name = 'ColorCorrectionEffect1_Graphic'
						c.Brightness = 0.176
						c.Contrast = 0.39
						c.Enabled = true
						c.Saturation = 0.2
						c.TintColor = Color3.fromRGB(217, 145, 57)
						if getgenv().mode == "Summer" then
							c.TintColor = Color3.fromRGB(255, 220, 148)
						elseif getgenv().mode == "Autumn" then
							c.TintColor = Color3.fromRGB(242, 193, 79)
						end
						local d = Instance.new("DepthOfFieldEffect", Graphic)
						d.Name =  'DepthOfFieldEffect_Graphic'
						d.Enabled = true
						d.FarIntensity = 0.077
						d.FocusDistance = 21.54
						d.InFocusRadius = 20.77
						d.NearIntensity = 0.277
						local e = Instance.new("ColorCorrectionEffect", a)
						e.Name = 'ColorCorrectionEffect2_Graphic'
						e.Brightness = 0
						e.Contrast = -0.07
						e.Saturation = 0
						e.Enabled = true
						e.TintColor = Color3.fromRGB(255, 247, 239)
						local e2 = Instance.new("ColorCorrectionEffect", a)
						e2.Name = 'ColorCorrectionEffect3_Graphic'
						e2.Brightness = 0.2
						e2.Contrast = 0.45
						e2.Saturation = -0.1
						e2.Enabled = true
						e2.TintColor = Color3.fromRGB(255, 255, 255)
						local s = Instance.new("SunRaysEffect", a)
						s.Name = 'SunRaysEffect_Graphic'
						s.Enabled = false
						s.Intensity = 0.01
						s.Spread = 0.146
					else
						local a = game.Lighting
						a.Ambient = Color3.fromRGB(170, 170, 170)
						a.Brightness = 2
						a.ColorShift_Bottom = Color3.fromRGB(0, 0, 0)
						a.ColorShift_Top = Color3.fromRGB(0, 0, 0)
						a.EnvironmentDiffuseScale = 0.105
						a.EnvironmentSpecularScale = 0.522
						a.GlobalShadows = false
						a.OutdoorAmbient = Color3.fromRGB(127, 127, 127)
						a.ShadowSoftness = 0
						a.GeographicLatitude = 66
						a.ExposureCompensation = 0.2
						game:GetService("Lighting")["BloomEffect_Graphic"]:Destroy()
						game:GetService("Lighting")["ColorCorrectionEffect1_Graphic"]:Destroy()
						game:GetService("Lighting")["ColorCorrectionEffect2_Graphic"]:Destroy()
						game:GetService("Lighting")["ColorCorrectionEffect3_Graphic"]:Destroy()
						game:GetService("Lighting")["SunRaysEffect_Graphic"]:Destroy()
					end
				end)
		
			Misc:Toggle("Xray",false,function(value)
				NoWorld = value
				if NoWorld == true then
					transparent = true
					x(transparent)
				elseif NoWorld == false then
					transparent = false
					x(transparent)
				end
			end)
		
			local transparent = false -- xray
			function x(v)
				if v then
					for _,i in pairs(workspace:GetDescendants()) do
						if i:IsA("BasePart") and not i.Parent:FindFirstChild("Humanoid") and not i.Parent.Parent:FindFirstChild("Humanoid") then
							i.LocalTransparencyModifier = 0.7
						end
					end
				else
					for _,i in pairs(workspace:GetDescendants()) do
						if i:IsA("BasePart") and not i.Parent:FindFirstChild("Humanoid") and not i.Parent.Parent:FindFirstChild("Humanoid") then
							i.LocalTransparencyModifier = 0
						end
					end
				end
			end
	
			Misc:Seperator("Misc")
		
			   Misc:Toggle("Auto Haki", true,function(vu)
			  _G.AutoHakiBuso = vu
		   end)
		
			 spawn(function()
			  while wait(.1) do
				 if _G.AutoHakiBuso then
					if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
					   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buso")
					end
				 end
			  end
		   end)
		
		Misc:Toggle("Auto Click",_G.autoclick,function(value)
				_G.autoclick = value
			end)
	
			spawn(function()
				while wait() do
					if _G.autoclick then
						Click()
					end
				end
			end)
		
		Misc:Toggle("Anti AFK", true, function()
		local vu = game:GetService("VirtualUser")
		repeat wait() until game:IsLoaded() 
			game:GetService("Players").LocalPlayer.Idled:connect(function()
			game:GetService("VirtualUser"):ClickButton2(Vector2.new())
				vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
				wait(1)
				vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
		   end)
		end)
		
			Misc:Toggle("Auto Rejoin",true,function(value)
				_G.AutoRejoin = value
			end)
		
			spawn(function()
				while wait(.1) do
					if _G.AutoRejoin then
							_G.AutoRejoin = game:GetService("CoreGui").RobloxPromptGui.promptOverlay.ChildAdded:Connect(function(child)
								if child.Name == 'ErrorPrompt' and child:FindFirstChild('MessageArea') and child.MessageArea:FindFirstChild("ErrorFrame") then
									game:GetService("TeleportService"):Teleport(game.PlaceId)
								end
							end)
						end
					end
				end)

				Misc:Toggle("No Clip",getgenv().noclip,function(value)
					getgenv().noclip = value
				end)

				spawn(function()
					game:GetService("RunService").Stepped:Connect(function()
						if getgenv().noclip then
							for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
								if v:IsA("BasePart") then
									v.CanCollide = false
								end
							end
						end
					end)
				end)

			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
			wait(1)
			Notification:Notify(
				{Title = "Pado Hub", Description = "Sucessful"},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
			)
		end

		if game.PlaceId == 2768379856 then
		
				local notifSound = Instance.new("Sound",workspace)
				notifSound.PlaybackSpeed = 1.5
				notifSound.Volume = 0.15
				notifSound.SoundId = "rbxassetid://170765130"
				notifSound.PlayOnRemove = true
				notifSound:Destroy()

		function Hop()
			local PlaceID = game.PlaceId
			local AllIDs = {}
			local foundAnything = ""
			local actualHour = os.date("!*t").hour
			local Deleted = false
			function TPReturner()
				local Site;
				if foundAnything == "" then
					Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
				else
					Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
				end
				local ID = ""
				if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
					foundAnything = Site.nextPageCursor
				end
				local num = 0;
				for i,v in pairs(Site.data) do
					local Possible = true
					ID = tostring(v.id)
					if tonumber(v.maxPlayers) > tonumber(v.playing) then
						for _,Existing in pairs(AllIDs) do
							if num ~= 0 then
								if ID == tostring(Existing) then
									Possible = false
								end
							else
								if tonumber(actualHour) ~= tonumber(Existing) then
									local delFile = pcall(function()
										AllIDs = {}
										table.insert(AllIDs, actualHour)
									end)
								end
							end
							num = num + 1
						end
						if Possible == true then
							table.insert(AllIDs, ID)
							wait()
							pcall(function()
								wait()
								game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
							end)
							wait(4)
						end
					end
				end
			end
			function Teleport() 
				while wait() do
					pcall(function()
						TPReturner()
						if foundAnything ~= "" then
							TPReturner()
						end
					end)
				end
			end
			Teleport()
		end                   
	
			function isnil(thing)
				return (thing == nil)
			end
			local function round(n)
				return math.floor(tonumber(n) + 0.5)
			end
				Number = math.random(1, 1000000)
			function UpdatePlayerChams()
				for i, v in pairs(game:GetService "Players":GetChildren()) do
					pcall(function()
						if not isnil(v.Character) then
								if ESPPlayer then
								if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild("NameEsp" .. Number) then
								local bill = Instance.new("BillboardGui", v.Character.Head)
								bill.Name = "NameEsp" .. Number
								bill.ExtentsOffset = Vector3.new(0, 1, 0)
								bill.Size = UDim2.new(1, 200, 1, 30)
								bill.Adornee = v.Character.Head
								bill.AlwaysOnTop = true
								local name = Instance.new("TextLabel", bill)
								name.Font = "GothamSemibold"
								name.FontSize = "Size14"
								name.TextWrapped = true
								name.Text =
									(v.Name ..
									" \n" ..
										round(
											(game:GetService("Players").LocalPlayer.Character.Head.Position -
												v.Character.Head.Position).Magnitude / 3
										) ..
											" M")
								name.Size = UDim2.new(1, 0, 1, 0)
								name.TextYAlignment = "Top"
								name.BackgroundTransparency = 1
								name.TextStrokeTransparency = 0.5
								if v.Team == game.Players.LocalPlayer.Team then
									name.TextColor3 = Color3.new(170, 0, 0)
								end
							else
								v.Character.Head["NameEsp" .. Number].TextLabel.Text =
									(v.Name ..
									" | " ..
										round(
											(game:GetService("Players").LocalPlayer.Character.Head.Position -
												v.Character.Head.Position).Magnitude / 3
										) ..
											" M \n Health : " ..
												round(v.Character.Humanoid.Health * 100 / v.Character.Humanoid.MaxHealth) ..
													"%")
							end
						else
							if v.Character.Head:FindFirstChild("NameEsp" .. Number) then
								v.Character.Head:FindFirstChild("NameEsp" .. Number):Destroy()
							end
						end
					end
				end
			)
		end
	end

	function UpdateFoodChams()
		for i, v in pairs(game:GetService("Workspace").GameObjects.Physical.Items:GetChildren()) do
			pcall(function()
				if ESPFood then
						if not v.Root:FindFirstChild("NameEsp" .. Number) then
						local bill = Instance.new("BillboardGui", v.Root)
						bill.Name = "NameEsp" .. Number
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v.Root
						bill.AlwaysOnTop = true
						local name = Instance.new("TextLabel", bill)
						name.Font = "GothamSemibold"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = "Top"
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(170, 0, 0)
						name.Text =
							(v.Name ..
							" \n" ..
								round(
									(game:GetService("Players").LocalPlayer.Character.Head.Position -
										v.Root.Position).Magnitude / 3
								) ..
									" M")
					else
						v.Root["NameEsp" .. Number].TextLabel.Text =
							(v.Name ..
							"   \n" ..
								round(
									(game:GetService("Players").LocalPlayer.Character.Head.Position -
										v.Root.Position).Magnitude / 3
								) ..
									" M")
					end
				else
					if v.Root:FindFirstChild("NameEsp" .. Number) then
						v.Root:FindFirstChild("NameEsp" .. Number):Destroy()
					end
				end
			end
		)
		end
	end		

function UpdateEmployeeESP()
for i, v in pairs(game:GetService("Workspace").GameObjects.Physical.Employees:GetChildren()) do
pcall(
	function()
		if EmployeeESP then
			if
				string.find(v.Name, "Wide Employee") or string.find(v.Name, "Abomination Employee") or
					string.find(v.Name, "Block Employee") or
					string.find(v.Name, "Buff Employee") or
					string.find(v.Name, "Employee") or
					string.find(v.Name, "Woman Employee") or
					string.find(v.Name, "Man Employee")
			 then
				if not v.Head:FindFirstChild("NameEsp" .. Number) then
					local bill = Instance.new("BillboardGui", v.Head)
					bill.Name = "NameEsp" .. Number
					bill.ExtentsOffset = Vector3.new(0, 1, 0)
					bill.Size = UDim2.new(1, 200, 1, 30)
					bill.Adornee = v.Head
					bill.AlwaysOnTop = true
					local name = Instance.new("TextLabel", bill)
					name.Font = "GothamSemibold"
					name.FontSize = "Size14"
					name.TextWrapped = true
					name.Size = UDim2.new(1, 0, 1, 0)
					name.TextYAlignment = "Top"
					name.BackgroundTransparency = 1
					name.TextStrokeTransparency = 0.5
					name.TextColor3 = Color3.fromRGB(170, 0, 0)
					name.Text =
						(v.Name ..
						" \n" ..
							round(
								(game:GetService("Players").LocalPlayer.Character.Head.Position -
									v.Head.Position).Magnitude / 3
							) ..
								" M")
				else
					v.Head["NameEsp" .. Number].TextLabel.Text =
						(v.Name ..
						"   \n" ..
							round(
								(game:GetService("Players").LocalPlayer.Character.Head.Position -
									v.Head.Position).Magnitude / 3
							) ..
								" M")
				end
			end
		else
			if v.Head:FindFirstChild("NameEsp" .. Number) then
				v.Head:FindFirstChild("NameEsp" .. Number):Destroy()
			end
		end
	end
)
end
end					

		local PADOXHUBMODILE = Instance.new("ScreenGui")
		local MODILEGUIPADOXHUB = Instance.new("TextButton")
		local MODILEGUIPADOXHUBHUI = Instance.new("UICorner")
		local MODILEMAGE = Instance.new("ImageLabel")

		MODILEGUIPADOXHUBHUI.Name = "MODILEGUIPADOXHUBHUI"
		MODILEGUIPADOXHUBHUI.Parent = MODILEGUIPADOXHUB

		MODILEMAGE.Name = "MODILEMAGE"
		MODILEMAGE.Parent = MODILEGUIPADOXHUB
		MODILEMAGE.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		MODILEMAGE.BackgroundTransparency = 1.000
		MODILEMAGE.BorderSizePixel = 0
		MODILEMAGE.Position = UDim2.new(-0.005, 0,-0.001, 0)
		MODILEMAGE.Size = UDim2.new(0, 50, 0, 50)
		MODILEMAGE.Image = "http://www.roblox.com/asset/?id=11804855180"

		PADOXHUBMODILE.Name = "PADOXHUBMODILE"
		PADOXHUBMODILE.Parent = game.CoreGui
		PADOXHUBMODILE.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

		MODILEGUIPADOXHUB.Name = "MODILEGUIPADOXHUB"
		MODILEGUIPADOXHUB.Parent = PADOXHUBMODILE
		MODILEGUIPADOXHUB.BackgroundColor3 = Color3.fromRGB(30,20,20)
		MODILEGUIPADOXHUB.Position = UDim2.new(0, 0, 0.491228074, 0)
		MODILEGUIPADOXHUB.Size = UDim2.new(0, 50, 0, 50)
		MODILEGUIPADOXHUB.BackgroundTransparency = 1
		MODILEGUIPADOXHUB.BorderSizePixel = 0
		MODILEGUIPADOXHUB.Draggable = true
		MODILEGUIPADOXHUB.MouseButton1Click:Connect(function()
		game:GetService("VirtualInputManager"):SendKeyEvent(true,305,false,game)
		game:GetService("VirtualInputManager"):SendKeyEvent(false,305,false,game)
		end)

		local Update = loadstring(Game:HttpGet"https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Gui")()
		local PadoUi = Update:Window("Pado","",Enum.KeyCode.RightControl);
		local Main = PadoUi:Tab("General","6026568198")
		local ESP = PadoUi:Tab("ESP","6035202013")
		local Misc = PadoUi:Tab("Misc","6034509993") 

	local Time = Main:Label("")

	spawn(function()
		pcall(function() 
			while true do wait()
				Time:Set("Time : "..game:GetService("ReplicatedStorage").ServerSettings.TimeSettings.TimeLeft.Value)
			end
		end)
	end)

	Main:Toggle("Show Time",_G.Time, function(a)
		_G.Time = a
			if _G.Time then
				local Time = Instance.new("ScreenGui")
				local Times = Instance.new("TextButton")
				local Timess = Instance.new("UICorner")

				Timess.Name = "Timess"
				Timess.Parent = Times

				Time.Name = "Time"
				Time.Parent = game.CoreGui
				Time.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

				Times.Name = "Times"
				Times.Parent = Time
				Times.BackgroundColor3 = Color3.fromRGB(30,20,20)
				Times.Position = UDim2.new(0, 0, 0.491228074, 0)
				Times.Size = UDim2.new(0, 100, 0, 100)
				Times.TextSize = 14
				Times.TextColor3 = Color3.new(255,255,255)
				Times.BackgroundTransparency = 1
				Times.BorderSizePixel = 0
				Times.Draggable = true
				
				spawn(function()
					while wait() do
						Times.Text = "Time "..game:GetService("ReplicatedStorage").ServerSettings.TimeSettings.TimeLeft.Value
					end
				end)
			elseif _G.Time == false then
				game.CoreGui:FindFirstChild("Time"):Destroy()
			end
		end)

		Main:Seperator("Players")
	
			Playerslist = {}
		
		for i,v in pairs(game:GetService("Players"):GetChildren()) do
			table.insert(Playerslist,v.Name)
		end
		
		local SelectedPly = Main:Dropdown("Select Players",Playerslist,function(value)
			_G.SelectPly = value
		end)
		
		Main:Button("Refresh Player",function()
			Playerslist = {}
			SelectedPly:Clear()
			for i,v in pairs(game:GetService("Players"):GetChildren()) do  
				SelectedPly:Add(v.Name)
			end
		end)
	   
		Main:Button("Teleport", function()
			 game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[_G.SelectPly].Character.HumanoidRootPart.CFrame
		end)
	
		Main:Seperator("Float")

		Main:Fly()

		Main:Seperator("Body") 

		Main:Slider("Walk Speed",0,400,16,function(Value)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value            
end)

Main:Slider("Jump Hight",0,400,50,function(Value)
game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value            
end)

Main:Slider("Gravity",0,400,0, function(value)
workspace.Gravity = value
end)

Main:Line()

	Main:Toggle("Infinite Jump", nil, function(State)
	Infinite = State
	game:GetService("UserInputService").JumpRequest:connect(function()
		if Infinite then
			game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
			end
		end) 
	end)

	Main:Toggle("Full Bright",nil,function(value)
		_G.FullBright = value
		game.Lighting.Changed:connect(
			function()
				if _G.FullBright then
					game:GetService("Lighting").Ambient = Color3.new(1, 1, 1)
					game:GetService("Lighting").ColorShift_Bottom = Color3.new(1, 1, 1)
					game:GetService("Lighting").ColorShift_Top = Color3.new(1, 1, 1)
				else
					game:GetService("Lighting").Ambient = Color3.new(0, 0, 0)
					game:GetService("Lighting").ColorShift_Bottom = Color3.new(0, 0, 0)
					game:GetService("Lighting").ColorShift_Top = Color3.new(0, 0, 0)
				end
			end
		)
		end)
		
	Main:Toggle("No Fall Damage", nil, function(State)
	getgenv().yea = State
	local OldNameCall = nil
	OldNameCall = hookmetamethod(game, "__namecall", function(self, ...)
		local Args = {...}
		local Self = Args[1]
		if getnamecallmethod() == "FireServer" and self:IsA("RemoteEvent") and Args[3]:match("OriginalDamage") and getgenv().yea then
			return 
		end
		return OldNameCall(self, unpack(Args))
	end)
	end)
	
	Main:Button("Unlock Third Person", function()
	   game.Players.LocalPlayer.CameraMaxZoomDistance = 50
	   game.Players.LocalPlayer.CameraMode = Enum.CameraMode.Classic
	end)

	Main:Button("Destroy Fog", function()
		game:GetService("Lighting").Sky:Destroy()
	end)

		Main:Button("Destroy Tags",function()
			for _, v in pairs(game:GetService("Workspace"):GetDescendants()) do
				if v.Name == "Nametag" then
				v:Destroy()
			end		
		end
	end)

	ESP:Seperator("ESP")
	
	ESP:Toggle("ESP Player",false,function(value)
		ESPPlayer = value
		while ESPPlayer do wait()
			UpdatePlayerChams()
		end
	end)

	ESP:Toggle("ESP Food",false,function(value)
		ESPFood = value
		while ESPFood do wait()
			UpdateFoodChams()
		end
	end)

	ESP:Toggle("ESP Employe",false,function(value)
		EmployeeESP = value
		while EmployeeESP do wait()
			UpdateEmployeeESP()
		end
	end)

	Misc:Seperator("Server")
	
	Misc:Button("Join discord Server",function()
		local request = request or http_request or (syn and syn.request)
		if not request then return end
		local start = 6463
		local invCode = 'aQEPQA9a8e'
		for i = start-10, start+1 do
			spawn(function()
				pcall(function()
					request({Url = "http://127.0.0.1:"..tostring(i).."/rpc?v=1",Method = "POST",Headers = {["Content-Type"] = "application/json",["Origin"] = "https://discord.com"},Body = game:GetService("HttpService"):JSONEncode({["cmd"] = "INVITE_BROWSER",["nonce"] = game:GetService("HttpService"):GenerateGUID(false),["args"] = {["invite"] = {["code"] = invCode,},["code"] = invCode}})})
				end)
			end)
		end
	end)

	Misc:Button("Rejoin Server",function()
		game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
	end)

  Misc:Button("Hop Server",function()
   Hop()
  end)
  
  Misc:Button("Hop Lower Server",function()
	local Player = game.Players.LocalPlayer    
	local Http = game:GetService("HttpService")
	local TPS = game:GetService("TeleportService")
	local Api = "https://games.roblox.com/v1/games/"
	
	local _place,_id = game.PlaceId, game.JobId
	local _servers = Api.._place.."/servers/Public?sortOrder=Desc&limit=100"
	function ListServers(cursor)
	   local Raw = game:HttpGet(_servers .. ((cursor and "&cursor="..cursor) or ""))
	   return Http:JSONDecode(Raw)
	end
	
	local Next; repeat
	   local Servers = ListServers(Next)
	   for i,v in next, Servers.data do
		   if v.playing < v.maxPlayers and v.id ~= _id then
			   local s,r = pcall(TPS.TeleportToPlaceInstance,TPS,_place,v.id,Player)
			   if s then break end
		   end
	   end
	   
	   Next = Servers.nextPageCursor
	until not Next
  end)
	
	Misc:Button("Destroy Ui",function()
		if game.CoreGui:FindFirstChild("Pado Hub") then
			game.CoreGui:FindFirstChild("Pado Hub"):Destroy()
			game.CoreGui:FindFirstChild("PADOXHUBMODILE"):Destroy()
		end
	end)

	Misc:Seperator("Misc")
	
	Misc:Toggle("Anti AFK", true, function()
		local vu = game:GetService("VirtualUser")
	repeat wait() until game:IsLoaded() 
		game:GetService("Players").LocalPlayer.Idled:connect(function()
		game:GetService("VirtualUser"):ClickButton2(Vector2.new())
			vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
			wait(1)
			vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
	end)
	end)

	Misc:Toggle("Auto Rejoin",true,function(value)
		_G.AutoRejoin = value
	end)

	spawn(function()
		while wait() do
			if _G.AutoRejoin then
					_G.AutoRejoin = game:GetService("CoreGui").RobloxPromptGui.promptOverlay.ChildAdded:Connect(function(child)
						if child.Name == 'ErrorPrompt' and child:FindFirstChild('MessageArea') and child.MessageArea:FindFirstChild("ErrorFrame") then
							game:GetService("TeleportService"):Teleport(game.PlaceId)
						end
					end)
				end
			end
		end)

		Misc:Toggle("No Clip",getgenv().noclip,function(value)
			getgenv().noclip = value
		end)

		spawn(function()
			game:GetService("RunService").Stepped:Connect(function()
				if getgenv().noclip then
					for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
						if v:IsA("BasePart") then
							v.CanCollide = false
						end
					end
				end
			end)
		end)

	local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
	local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
					{Title = "Pado Hub", Description = "Sucessful"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end

	if game.PlaceId == 537413528 then
		
			local notifSound = Instance.new("Sound",workspace)
			notifSound.PlaybackSpeed = 1.5
			notifSound.Volume = 0.15
			notifSound.SoundId = "rbxassetid://170765130"
			notifSound.PlayOnRemove = true
			notifSound:Destroy()

		function Hop()
			local PlaceID = game.PlaceId
			local AllIDs = {}
			local foundAnything = ""
			local actualHour = os.date("!*t").hour
			local Deleted = false
			function TPReturner()
				local Site;
				if foundAnything == "" then
					Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
				else
					Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
				end
				local ID = ""
				if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
					foundAnything = Site.nextPageCursor
				end
				local num = 0;
				for i,v in pairs(Site.data) do
					local Possible = true
					ID = tostring(v.id)
					if tonumber(v.maxPlayers) > tonumber(v.playing) then
						for _,Existing in pairs(AllIDs) do
							if num ~= 0 then
								if ID == tostring(Existing) then
									Possible = false
								end
							else
								if tonumber(actualHour) ~= tonumber(Existing) then
									local delFile = pcall(function()
										AllIDs = {}
										table.insert(AllIDs, actualHour)
									end)
								end
							end
							num = num + 1
						end
						if Possible == true then
							table.insert(AllIDs, ID)
							wait()
							pcall(function()
								wait()
								game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
							end)
							wait(4)
						end
					end
				end
			end
			function Teleport() 
				while wait() do
					pcall(function()
						TPReturner()
						if foundAnything ~= "" then
							TPReturner()
						end
					end)
				end
			end
			Teleport()
		end                   
	
	local OldNameCall = nil
	OldNameCall = hookmetamethod(game, "__namecall", function(...)
		local Args = {...}
		local Self = Args[1]
		if getnamecallmethod()=="FireServer" and tostring(Self) == "Received" or tostring(Self) == "Sent" then
				return wait(math.huge)
		end
		return OldNameCall(...)
	end)
	function ToxmodsisHOT()
		game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart").CFrame = CFrame.new(-51.1823959, 80.6168747, -536.437805)
		tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(30, Enum.EasingStyle.Linear)
		tween =
			tweenService:Create(
			game:GetService("Players")["LocalPlayer"].Character:WaitForChild("HumanoidRootPart"),
			tweenInfo,
			{CFrame = CFrame.new(-60.5737877, 53.9498825, 8666.35059)}
		)
		tween:Play()
		wait(30)
		tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(0, Enum.EasingStyle.Linear)
		tween =
			tweenService:Create(
			game:GetService("Players")["LocalPlayer"].Character:WaitForChild("HumanoidRootPart"),
			tweenInfo,
			{CFrame = CFrame.new(-55.5486526, -360.063782, 9489.0498)}
		)
		tween:Play()
	end

	spawn(function()
		pcall(function()
			game:GetService("RunService").Stepped:Connect(function()
				if getgenv().Autofarm then
				if not game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
					local Noclip = Instance.new("BodyVelocity")
					Noclip.Name = "BodyClip"
					Noclip.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
					Noclip.MaxForce = Vector3.new(100000,100000,100000)
					Noclip.Velocity = Vector3.new(0,0,0)
				end
				for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
					if v:IsA("BasePart") then
						v.CanCollide = false  
					end
				end
			else	
				if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
						game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip"):Destroy()
					end
				end
			end)
		end)
	end)

	local PADOXHUBMODILE = Instance.new("ScreenGui")
	local MODILEGUIPADOXHUB = Instance.new("TextButton")
	local MODILEGUIPADOXHUBHUI = Instance.new("UICorner")
	local MODILEMAGE = Instance.new("ImageLabel")
	
	MODILEGUIPADOXHUBHUI.Name = "MODILEGUIPADOXHUBHUI"
	MODILEGUIPADOXHUBHUI.Parent = MODILEGUIPADOXHUB
	
	MODILEMAGE.Name = "MODILEMAGE"
	MODILEMAGE.Parent = MODILEGUIPADOXHUB
	MODILEMAGE.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	MODILEMAGE.BackgroundTransparency = 1.000
	MODILEMAGE.BorderSizePixel = 0
	MODILEMAGE.Position = UDim2.new(-0.005, 0,-0.001, 0)
	MODILEMAGE.Size = UDim2.new(0, 50, 0, 50)
	MODILEMAGE.Image = "http://www.roblox.com/asset/?id=11804855180"
	
	PADOXHUBMODILE.Name = "PADOXHUBMODILE"
	PADOXHUBMODILE.Parent = game.CoreGui
	PADOXHUBMODILE.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
	
	MODILEGUIPADOXHUB.Name = "MODILEGUIPADOXHUB"
	MODILEGUIPADOXHUB.Parent = PADOXHUBMODILE
	MODILEGUIPADOXHUB.BackgroundColor3 = Color3.fromRGB(30,20,20)
	MODILEGUIPADOXHUB.Position = UDim2.new(0, 0, 0.491228074, 0)
	MODILEGUIPADOXHUB.Size = UDim2.new(0, 50, 0, 50)
	MODILEGUIPADOXHUB.BackgroundTransparency = 1
	MODILEGUIPADOXHUB.BorderSizePixel = 0
	MODILEGUIPADOXHUB.Draggable = true
	MODILEGUIPADOXHUB.MouseButton1Click:Connect(function()
	game:GetService("VirtualInputManager"):SendKeyEvent(true,305,false,game)
	game:GetService("VirtualInputManager"):SendKeyEvent(false,305,false,game)
end)

		local Update = loadstring(Game:HttpGet"https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Gui")()
		local PadoUi = Update:Window("Pado",Enum.KeyCode.RightControl);
		local Main = PadoUi:Tab("General")
		local Combat = PadoUi:Tab("Players")
		local teams = PadoUi:Tab("Teams")
		local Teleport = PadoUi:Tab("Teleport")
		local Misc = PadoUi:Tab("Misc")    
	
		Main:Seperator("Main Farm")
	
		Main:Toggle("Auto Farm Coins", nil, function(State)
	getgenv().Autofarm = State
	game:GetService("RunService").Stepped:connect(
		function()
			if getgenv().Autofarm then
				game.Players.LocalPlayer.Character:WaitForChild("Humanoid"):ChangeState(11)
			end
		end
	)
	if getgenv().Autofarm then
		ToxmodsisHOT()
	end
	
	if not getgenv().Autofarm then
		game.Players.LocalPlayer.Character.Head:Destroy()
	end
	
	game.Players.LocalPlayer.CharacterAdded:Connect(
		function()
			repeat
				wait()
			until game.Players.LocalPlayer.Character
			wait(3)
			if getgenv().Autofarm then
				ToxmodsisHOT()
			end
		end
	)
	end)
	
	Main:Seperator("Chests")

	Main:Toggle("Auto Common Chests", nil, function(State)
		Common = State
		while Common do wait(1)
local args = {
	[1] = "Common Chest",
	[2] = 1
}

workspace.ItemBoughtFromShop:InvokeServer(unpack(args))
end
end)
	
	Main:Toggle("Auto UnCommon Chests", nil, function(State)
	UnCommon = State
	while UnCommon do wait(1)
local args = {
	[1] = "Uncommon Chest",
	[2] = 1
}

workspace.ItemBoughtFromShop:InvokeServer(unpack(args))
		end
		end)
	
	Main:Toggle("Auto Rare Chests", nil, function(State)
	Rare = State
	while Rare do wait(1)
local args = {
	[1] = "Rare Chest",
	[2] = 1
}

workspace.ItemBoughtFromShop:InvokeServer(unpack(args))
				end
				end)
			
	
	Main:Toggle("Auto Epic Chests", nil, function(State)
	Epic = State
	while Epic do wait(1)
local args = {
	[1] = "Epic Chest",
	[2] = 1
}

workspace.ItemBoughtFromShop:InvokeServer(unpack(args))
		end
	end)
	
	Main:Toggle("Auto Legendary Chests", nil, function(State)
	Legendary = State
	while Legendary do wait(1)
local args = {
	[1] = "Legendary Chest",
	[2] = 1
}

workspace.ItemBoughtFromShop:InvokeServer(unpack(args))
		end
	end)

	Combat:Seperator("Players")
	
	Playerslist = {}

for i,v in pairs(game:GetService("Players"):GetChildren()) do
	table.insert(Playerslist,v.Name)
end

local SelectedPly = Combat:Dropdown("Select Players",Playerslist,function(value)
	_G.SelectPly = value
end)

Combat:Button("Refresh Player",function()
	Playerslist = {}
	SelectedPly:Clear()
	for i,v in pairs(game:GetService("Players"):GetChildren()) do  
		SelectedPly:Add(v.Name)
	end
end)

Combat:Button("Teleport", function()
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[_G.SelectPly].Character.HumanoidRootPart.CFrame
end)

Combat:Button("Building tools", function()
	for _,v in pairs(game:GetService("ReplicatedStorage").BuildingParts:GetChildren()) do
		if v:IsA("Tool") then
			v:clone().Parent = game.Players.LocalPlayer.Backpack
		   end
		end
	end)

	Combat:Toggle("Infinite Jump", nil, function(value)
_G.Infinite = value
game:GetService("UserInputService").JumpRequest:connect(function()
if _G.Infinite then
	game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
end end) end)

Combat:Toggle("Water God Mode", nil, function(State)
getgenv().Water = State 
game:GetService('RunService').Stepped:connect(function()
pcall(function()
if getgenv().Water and game.Players.LocalPlayer.Character:FindFirstChild("WaterDetector")  then
game.Players.LocalPlayer.Character.WaterDetector:remove()
end end) end) end)

Combat:Seperator("Float")

Combat:Fly()

Combat:Seperator("Identity Info") 

Combat:Slider("Walk Speed",0,400,16,function(Value)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value            
end)

Combat:Slider("Jump Hight",0,400,50,function(Value)
game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value            
end)

Combat:Slider("Gravity",0,400,0, function(value)
workspace.Gravity = value
end)

		teams:Seperator("Teams")

		teams:Button("Black", function()
		local args = {
			[1] = game:GetService("Teams"):WaitForChild("black")
		}
		
		workspace:WaitForChild("ChangeTeam"):FireServer(unpack(args))
	end)										

	teams:Button("Blue", function()
		local args = {
			[1] = game:GetService("Teams"):WaitForChild("blue")
		}
		
		workspace:WaitForChild("ChangeTeam"):FireServer(unpack(args))
	end)										

	teams:Button("Green", function()
		local args = {
			[1] = game:GetService("Teams"):WaitForChild("green")
		}
		
		workspace:WaitForChild("ChangeTeam"):FireServer(unpack(args))
	end)										

	teams:Button("Magenta", function()
		local args = {
			[1] = game:GetService("Teams"):WaitForChild("magenta")
		}
		
		workspace:WaitForChild("ChangeTeam"):FireServer(unpack(args))
	end)										

	teams:Button("Red", function()
		local args = {
			[1] = game:GetService("Teams"):WaitForChild("red")
		}
		
		workspace:WaitForChild("ChangeTeam"):FireServer(unpack(args))
	end)			
	
	teams:Button("White", function()
		local args = {
			[1] = game:GetService("Teams"):WaitForChild("white")
		}
		
		workspace:WaitForChild("ChangeTeam"):FireServer(unpack(args))
	end)		

	teams:Button("Yellow", function()
		local args = {
			[1] = game:GetService("Teams"):WaitForChild("yellow")
		}
		
		workspace:WaitForChild("ChangeTeam"):FireServer(unpack(args))
	end)	
	
	Teleport:Seperator("Color Zone")
	
	Teleport:Button("Blue Zone", function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["Really blueZone"].CFrame * CFrame.new(0,5,0)
	end)
	
	Teleport:Button("Black Zone", function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BlackZone.CFrame * CFrame.new(0,5,0)
	end)
	
	Teleport:Button("Purple Zone", function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").MagentaZone.CFrame * CFrame.new(0,5,0)
	end)
	
	Teleport:Button("Yellow Zone", function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["New YellerZone"].CFrame * CFrame.new(0,5,0)
	end)
	
	Teleport:Button("Green Zone", function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").CamoZone.CFrame * CFrame.new(0,5,0)
	end)
	
	Teleport:Button("White Zone", function()
	game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-48.5936432, -9.65237236, -406.830872, 0.999822497, -0.000123897291, 0.0188400596, 0, 0.999978364, 0.00657612644, -0.0188404657, -0.00657495949, 0.999800861)
	end)
	
	Misc:Seperator("Server")
		
	Misc:Button("Join discord Server",function()
		setclipboard("https://discord.gg/aQEPQA9a8e")
	end)

	Misc:Button("Rejoin Server",function()
		game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
	end)

	Misc:Button("Hop Server",function()
	Hop()
	end)
	
	Misc:Button("Hop Lower Server",function()
	local Player = game.Players.LocalPlayer    
	local Http = game:GetService("HttpService")
	local TPS = game:GetService("TeleportService")
	local Api = "https://games.roblox.com/v1/games/"
	
	local _place,_id = game.PlaceId, game.JobId
	local _servers = Api.._place.."/servers/Public?sortOrder=Desc&limit=100"
	function ListServers(cursor)
		local Raw = game:HttpGet(_servers .. ((cursor and "&cursor="..cursor) or ""))
		return Http:JSONDecode(Raw)
	end
	
	local Next; repeat
		local Servers = ListServers(Next)
		for i,v in next, Servers.data do
			if v.playing < v.maxPlayers and v.id ~= _id then
				local s,r = pcall(TPS.TeleportToPlaceInstance,TPS,_place,v.id,Player)
				if s then break end
			end
		end
		
		Next = Servers.nextPageCursor
	until not Next
	end)
	
	Misc:Button("Destroy Ui",function()
		if game.CoreGui:FindFirstChild("Pado Hub") then
			game.CoreGui:FindFirstChild("Pado Hub"):Destroy()
			game.CoreGui:FindFirstChild("PADOXHUBMODILE"):Destroy()
		end
	end)

	Misc:Seperator("Misc")
		
	Misc:Toggle("Anti AFK", true, function()
		local vu = game:GetService("VirtualUser")
	repeat wait() until game:IsLoaded() 
		game:GetService("Players").LocalPlayer.Idled:connect(function()
		game:GetService("VirtualUser"):ClickButton2(Vector2.new())
			vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
			wait(1)
			vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
	end)
	end)

	Misc:Toggle("Auto Rejoin",true,function(value)
		_G.AutoRejoin = value
	end)

	spawn(function()
		while wait() do
			if _G.AutoRejoin then
					_G.AutoRejoin = game:GetService("CoreGui").RobloxPromptGui.promptOverlay.ChildAdded:Connect(function(child)
						if child.Name == 'ErrorPrompt' and child:FindFirstChild('MessageArea') and child.MessageArea:FindFirstChild("ErrorFrame") then
							game:GetService("TeleportService"):Teleport(game.PlaceId)
						end
					end)
				end
			end
		end)

		Misc:Toggle("No Clip",getgenv().noclip,function(value)
			getgenv().noclip = value
		end)

		spawn(function()
			game:GetService("RunService").Stepped:Connect(function()
				if getgenv().noclip then
					for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
						if v:IsA("BasePart") then
							v.CanCollide = false
						end
					end
				end
			end)
		end)

			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
					{Title = "Pado Hub", Description = "Sucessful"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end

			if game.PlaceId == 1240123653 or game.PlaceId == 1632210982 then
				
					local notifSound = Instance.new("Sound",workspace)
					notifSound.PlaybackSpeed = 1.5
					notifSound.Volume = 0.15
					notifSound.SoundId = "rbxassetid://170765130"
					notifSound.PlayOnRemove = true
					notifSound:Destroy()

				function Hop()
					local PlaceID = game.PlaceId
					local AllIDs = {}
					local foundAnything = ""
					local actualHour = os.date("!*t").hour
					local Deleted = false
					function TPReturner()
						local Site;
						if foundAnything == "" then
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
						else
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
						end
						local ID = ""
						if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
							foundAnything = Site.nextPageCursor
						end
						local num = 0;
						for i,v in pairs(Site.data) do
							local Possible = true
							ID = tostring(v.id)
							if tonumber(v.maxPlayers) > tonumber(v.playing) then
								for _,Existing in pairs(AllIDs) do
									if num ~= 0 then
										if ID == tostring(Existing) then
											Possible = false
										end
									else
										if tonumber(actualHour) ~= tonumber(Existing) then
											local delFile = pcall(function()
												AllIDs = {}
												table.insert(AllIDs, actualHour)
											end)
										end
									end
									num = num + 1
								end
								if Possible == true then
									table.insert(AllIDs, ID)
									wait()
									pcall(function()
										wait()
										game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
									end)
									wait(4)
								end
							end
						end
					end
					function Teleport() 
						while wait() do
							pcall(function()
								TPReturner()
								if foundAnything ~= "" then
									TPReturner()
								end
							end)
						end
					end
					Teleport()
				end        

				function isnil(thing)
						return (thing == nil)
					end
					local function round(n)
						return math.floor(tonumber(n) + 0.5)
					end
					Number = math.random(1, 1000000)
					function UpdatePlayerChams()
						for i,v in pairs(game:GetService'Players':GetChildren()) do
							pcall(function()
								if not isnil(v.Character) then
									if ESPPlayer then
										if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp'..Number) then
											local bill = Instance.new('BillboardGui',v.Character.Head)
											bill.Name = 'NameEsp'..Number
											bill.ExtentsOffset = Vector3.new(0, 1, 0)
											bill.Size = UDim2.new(1,200,1,30)
											bill.Adornee = v.Character.Head
											bill.AlwaysOnTop = true
											local name = Instance.new('TextLabel',bill)
											name.Font = "GothamSemibold"
											name.FontSize = "Size14"
											name.TextWrapped = true
											name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
											name.Size = UDim2.new(1,0,1,0)
											name.TextYAlignment = 'Top'
											name.BackgroundTransparency = 1
											name.TextStrokeTransparency = 0.5
											if v.Team == game.Players.LocalPlayer.Team then
												name.TextColor3 = Color3.new(255,0,0)
											end
										else
											v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..' | '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M \n Health : ' .. round(v.Character.Humanoid.Health*100/v.Character.Humanoid.MaxHealth) .. '%')
										end
									else
										if v.Character.Head:FindFirstChild('NameEsp'..Number) then
											v.Character.Head:FindFirstChild('NameEsp'..Number):Destroy()
										end
									end
								end
							end)
							end
						end

						local PADOXHUBMODILE = Instance.new("ScreenGui")
						local MODILEGUIPADOXHUB = Instance.new("TextButton")
						local MODILEGUIPADOXHUBHUI = Instance.new("UICorner")
						local MODILEMAGE = Instance.new("ImageLabel")
						
						MODILEGUIPADOXHUBHUI.Name = "MODILEGUIPADOXHUBHUI"
						MODILEGUIPADOXHUBHUI.Parent = MODILEGUIPADOXHUB
						
						MODILEMAGE.Name = "MODILEMAGE"
						MODILEMAGE.Parent = MODILEGUIPADOXHUB
						MODILEMAGE.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						MODILEMAGE.BackgroundTransparency = 1.000
						MODILEMAGE.BorderSizePixel = 0
						MODILEMAGE.Position = UDim2.new(-0.005, 0,-0.001, 0)
						MODILEMAGE.Size = UDim2.new(0, 50, 0, 50)
						MODILEMAGE.Image = "http://www.roblox.com/asset/?id=11804855180"
						
						PADOXHUBMODILE.Name = "PADOXHUBMODILE"
						PADOXHUBMODILE.Parent = game.CoreGui
						PADOXHUBMODILE.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
						
						MODILEGUIPADOXHUB.Name = "MODILEGUIPADOXHUB"
						MODILEGUIPADOXHUB.Parent = PADOXHUBMODILE
						MODILEGUIPADOXHUB.BackgroundColor3 = Color3.fromRGB(30,20,20)
						MODILEGUIPADOXHUB.Position = UDim2.new(0, 0, 0.491228074, 0)
						MODILEGUIPADOXHUB.Size = UDim2.new(0, 50, 0, 50)
						MODILEGUIPADOXHUB.BackgroundTransparency = 1
						MODILEGUIPADOXHUB.BorderSizePixel = 0
						MODILEGUIPADOXHUB.Draggable = true
						MODILEGUIPADOXHUB.MouseButton1Click:Connect(function()
						game:GetService("VirtualInputManager"):SendKeyEvent(true,305,false,game)
						game:GetService("VirtualInputManager"):SendKeyEvent(false,305,false,game)
					end)

					local Update = loadstring(Game:HttpGet"https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Gui")()
					local PadoUi = Update:Window("Pado","",Enum.KeyCode.RightControl);
					local Main = PadoUi:Tab("General")
					local Combat = PadoUi:Tab("Players")
					local Misc = PadoUi:Tab("Misc")

			local Cash = Main:Label("")

			spawn(function()
				pcall(function() 
					while true do wait(.1)
						Cash:Set("Cash : "..game:GetService("Players").LocalPlayer.leaderstats.Cash.Value)
					end
				end)
			end)

			local Kills = Main:Label("")

			spawn(function()
				pcall(function() 
					while true do wait(.1)
						Kills:Set("Kills : "..game:GetService("Players").LocalPlayer.leaderstats.Kills.Value)
					end
				end)
			end)

		local wave = Main:Label("")

		spawn(function()
			pcall(function() 
				while true do wait(.1)
					if game:GetService("Players").LocalPlayer.PlayerGui.MainInterface.MenuHolder.StatsMain.CurrentWave.Visible == true then
						wave:Set(game:GetService("Players").LocalPlayer.PlayerGui.MainInterface.MenuHolder.StatsMain.CurrentWave.Text)
					else
						wave:Set("Wait to Wave")
					end
				end
			end)
		end)

		local Left = Main:Label("")

		spawn(function()
			pcall(function() 
				while true do wait(.1)
					Left:Set(game:GetService("Players").LocalPlayer.PlayerGui.MainInterface.MenuHolder.StatsMain.TimeLeftBackground.TextLabel.Text)
				end
			end)
		end)

		local Level = Main:Label("")

		spawn(function()
			pcall(function() 
				while true do wait(.1)
					Level:Set("Level : " .. game:GetService("Players").LocalPlayer.leaderstats.Level.Value .. " EXP : " .. game:GetService("Players").LocalPlayer.PlayerGui.MainInterface.ButtonsHolder.LevelGUI.EXPBackground.ExpValue.Text)
				end
			end)
		end)

					Main:Toggle("Auto Farm",_G.farm2,function(value)
						_G.farm2 = value
					end)

					local groundDistance = 8
					local Player = game:GetService("Players").LocalPlayer
					local function getNearest()
					local nearest, dist = nil, 99999
					for _,v in pairs(game.Workspace.BossFolder:GetChildren()) do
					if(v:FindFirstChild("Head")~=nil)then
					local m =(Player.Character.Head.Position-v.Head.Position).magnitude
					if(m<dist)then
					dist = m
					nearest = v
					end
					end
					end
					for _,v in pairs(game.Workspace.enemies:GetChildren()) do
					if(v:FindFirstChild("Head")~=nil)then
					local m =(Player.Character.Head.Position-v.Head.Position).magnitude
					if(m<dist)then
					dist = m
					nearest = v
					end
					end
					end
					return nearest
					end
					
					_G.globalTarget = nil
					game:GetService("RunService").RenderStepped:Connect(function()
					if(_G.farm2==true)then
					local target = getNearest()
					if(target~=nil)then
					game:GetService("Workspace").CurrentCamera.CFrame = CFrame.new(game:GetService("Workspace").CurrentCamera.CFrame.p, target.Head.Position)
					Player.Character.HumanoidRootPart.CFrame = (target.HumanoidRootPart.CFrame * CFrame.new(getgenv().X, getgenv().Y, getgenv().Z))
					_G.globalTarget = target
					end
					end
					end)
					
					spawn(function()
						while wait() do
							if _G.farm2 then
								game.Players.LocalPlayer.Character.HumanoidRootPart.Velocity = Vector3.new(0,0,0)
								game.Players.LocalPlayer.Character.Torso.Velocity = Vector3.new(0,0,0)
							end
						end
					end)

				spawn(function()
					while wait() do
						if _G.farm2 then
							if(_G.farm2==true and _G.globalTarget~=nil and _G.globalTarget:FindFirstChild("Head") and Player.Character:FindFirstChildOfClass("Tool"))then
								local target = _G.globalTarget
									game.ReplicatedStorage.Gun:FireServer({["Normal"] = Vector3.new(0, 0, 0), ["Direction"] = target.Head.Position, ["Name"] = Player.Character:FindFirstChildOfClass("Tool").Name, ["Hit"] = target.Head, ["Origin"] = target.Head.Position, ["Pos"] = target.Head.Position,})
								wait()
							end
						end
					end
				end)

					Main:Toggle("Auto Powerups",_G.AutobringPowerups,function(value)
						_G.AutobringPowerups = value
					end)

					spawn(function()
						while wait() do
							if _G.AutobringPowerups then
								pcall(function()
									for i,v in pairs(game:GetService("Workspace").Powerups:GetDescendants()) do
										if v.Name == "TouchInterest" then
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Parent.CFrame
										end
									end
								end)
							end
						end
					end)

					Main:Seperator("Farm Distance X/Y/Z Settings")

					getgenv().Z = 9
					getgenv().Y = 8

					Main:Slider("Farm (X)",1,60,0,function(value)
						getgenv().X = value
					end)
					
					Main:Slider("Farm (Y)",1,60,8,function(value)
						getgenv().Y = value
					end)
					
					Main:Slider("Farm (Z)",1,60,9,function(value)
						getgenv().Z = value
					end)

					Combat:Seperator("Players")
						
					Playerslist = {}
					
					for i,v in pairs(game:GetService("Players"):GetChildren()) do
						table.insert(Playerslist,v.Name)
					end
					
					local SelectedPly = Combat:Dropdown("Select Players",Playerslist,function(value)
					_G.SelectPly = value
					end)
					
					Combat:Button("Refresh Player",function()
					SelectedPly:Clear()
					for i,v in pairs(game:GetService("Players"):GetChildren()) do
						SelectedPly:Add(v.Name)
					end
					end)
					
						Combat:Toggle("Spectate Player",false,function(value)
						SpectatePlys = value
						local plr1 = game:GetService("Players").LocalPlayer.Character.Humanoid
						local plr2 = game:GetService("Players"):FindFirstChild(_G.SelectPly)
						repeat wait(.1)
							game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players"):FindFirstChild(_G.SelectPly).Character.Humanoid
						until SpectatePlys == false
						game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players").LocalPlayer.Character.Humanoid
						end)
					
						Combat:Toggle("Teleport",false,function(bool)
						_G.Teleport1 = bool
						while _G.Teleport1 do wait(.1)
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players:FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.CFrame * CFrame.new(getgenv().Z,getgenv().Y,getgenv().X)
						end
						end)
					
						Combat:Toggle("Auto Farm Player",false,function(value)
						_G.Auto_Kill_Ply = value
						end)
					
						spawn(function()
						while wait(.1) do
							if _G.Auto_Kill_Ply then
								pcall(function()
								if _G.SelectPly ~= nil then
								if game.Players:FindFirstChild(_G.SelectPly) then
									if game.Players:FindFirstChild(_G.SelectPly).Character.Humanoid.Health > 0 then
										repeat wait(.1)
											game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players:FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.CFrame * CFrame.new(getgenv().Z,getgenv().Y,getgenv().X)
										until game.Players:FindFirstChild(_G.SelectPly).Character.Humanoid.Health <= 0 or not game.Players:FindFirstChild(_G.SelectPly) or not _G.Auto_Kill_Ply
									end
								end
								end
								end)
							end
						end
						end)

						Combat:Toggle("ESP Player",false,function(value)
							ESPPlayer = value
							while ESPPlayer do wait(.1)
								UpdatePlayerChams()
							end
						end)	

						Combat:Button("No Cooldown",function()
						local Speed; Speed = hookfunction(wait, function(v)
							v = 0;
							return Speed(v);
						end);
					end)

					Combat:Seperator("Meun")

					Combat:Toggle("Auto Veiw",_G.veiw,function(value)
					_G.veiw = value
				while _G.veiw do wait()
					game:GetService("Players").LocalPlayer.PlayerGui.MainInterface.ButtonsHolder.Main.Spectate.Visible = true
				end
				end)
				
							Combat:Seperator("Float")

					Combat:Fly()

					Combat:Seperator("Identity Info") 

			Combat:Slider("Walk Speed",0,400,16,function(Value)
			game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value 
		end)

			Combat:Slider("Jump Hight",0,400,50,function(Value)
			game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value
		end)

			Combat:Slider("Gravity",0,400,0, function(value)
			workspace.Gravity = value 
		end)

					Combat:Toggle("Infinite Jump", nil, function(value)
						_G.Infinite = value
						game:GetService("UserInputService").JumpRequest:connect(function()
							if _G.Infinite then
								game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
							end 
						end) 
					end)	

					Misc:Seperator("Server")
		
					Misc:Button("Join discord Server",function()
						local request = request or http_request or (syn and syn.request)
						if not request then return end
						local start = 6463
						local invCode = 'aQEPQA9a8e'
						for i = start-10, start+1 do
							spawn(function()
								pcall(function()
									request({Url = "http://127.0.0.1:"..tostring(i).."/rpc?v=1",Method = "POST",Headers = {["Content-Type"] = "application/json",["Origin"] = "https://discord.com"},Body = game:GetService("HttpService"):JSONEncode({["cmd"] = "INVITE_BROWSER",["nonce"] = game:GetService("HttpService"):GenerateGUID(false),["args"] = {["invite"] = {["code"] = invCode,},["code"] = invCode}})})
								end)
							end)
						end
					end)
			
					Misc:Button("Rejoin Server",function()
						game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
					end)
				
					Misc:Button("Hop Server",function()
					Hop()
					end)
					
					Misc:Button("Hop Lower Server",function()
					local Player = game.Players.LocalPlayer    
					local Http = game:GetService("HttpService")
					local TPS = game:GetService("TeleportService")
					local Api = "https://games.roblox.com/v1/games/"
					
					local _place,_id = game.PlaceId, game.JobId
					local _servers = Api.._place.."/servers/Public?sortOrder=Desc&limit=100"
					function ListServers(cursor)
						local Raw = game:HttpGet(_servers .. ((cursor and "&cursor="..cursor) or ""))
						return Http:JSONDecode(Raw)
					end
					
					local Next; repeat
						local Servers = ListServers(Next)
						for i,v in next, Servers.data do
							if v.playing < v.maxPlayers and v.id ~= _id then
								local s,r = pcall(TPS.TeleportToPlaceInstance,TPS,_place,v.id,Player)
								if s then break end
							end
						end
						
						Next = Servers.nextPageCursor
					until not Next
					end)
					
					Misc:Button("Destroy Ui",function()
						if game.CoreGui:FindFirstChild("Pado Hub") then
							game.CoreGui:FindFirstChild("Pado Hub"):Destroy()
							game.CoreGui:FindFirstChild("PADOXHUBMODILE"):Destroy()
						end
					end)

					Misc:Seperator("Jobid")
				
					Misc:Button("Copy Jobid",function()
						setclipboard(tostring(game.JobId))
					end)
				
					Misc:Textbox("join jobid Link","Type You Link",function(t)
						_G.joinjobid = t
					end)
				
					_G.joinjobid = ""
				
					Misc:Button("Join",function()
						game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId,_G.joinjobid)
					end)
			
					Misc:Seperator("Ui")

				Misc:Button("transpose Zombie",function()
					local args = {
						[1] = "request_become_zombie"
					}
					
					game:GetService("ReplicatedStorage"):WaitForChild("RemoteEventContainer"):WaitForChild("CommunicationE"):FireServer(unpack(args))
				end)														

				Misc:Button("SHOP",function()
					game:GetService("Players").LocalPlayer.PlayerGui.MainInterface.MenuHolder.Main.Visible = true
				end)														

					Misc:Seperator("Misc")
						
					Misc:Toggle("Anti AFK", true, function()
						local vu = game:GetService("VirtualUser")
					repeat wait() until game:IsLoaded() 
						game:GetService("Players").LocalPlayer.Idled:connect(function()
						game:GetService("VirtualUser"):ClickButton2(Vector2.new())
							vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
							wait(1)
							vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
					end)
					end)
			
					Misc:Toggle("Auto Rejoin",true,function(value)
						_G.AutoRejoin = value
					end)
				
					spawn(function()
						while wait() do
							if _G.AutoRejoin then
									_G.AutoRejoin = game:GetService("CoreGui").RobloxPromptGui.promptOverlay.ChildAdded:Connect(function(child)
										if child.Name == 'ErrorPrompt' and child:FindFirstChild('MessageArea') and child.MessageArea:FindFirstChild("ErrorFrame") then
											game:GetService("TeleportService"):Teleport(game.PlaceId)
										end
									end)
								end
							end
						end)

						Misc:Toggle("No Clip",getgenv().noclip,function(value)
							getgenv().noclip = value
						end)
		
						spawn(function()
							game:GetService("RunService").Stepped:Connect(function()
								if getgenv().noclip then
									for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
										if v:IsA("BasePart") then
											v.CanCollide = false
										end
									end
								end
							end)
						end)

					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
							wait(1)
							Notification:Notify(
							{Title = "Pado Hub", Description = "Sucessful"},
							{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
						)
					end

			if game.PlaceId == 662417684 then
				
					local notifSound = Instance.new("Sound",workspace)
					notifSound.PlaybackSpeed = 1.5
					notifSound.Volume = 0.15
					notifSound.SoundId = "rbxassetid://170765130"
					notifSound.PlayOnRemove = true
					notifSound:Destroy()

				function Hop()
					local PlaceID = game.PlaceId
					local AllIDs = {}
					local foundAnything = ""
					local actualHour = os.date("!*t").hour
					local Deleted = false
					function TPReturner()
						local Site;
						if foundAnything == "" then
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
						else
							Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
						end
						local ID = ""
						if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
							foundAnything = Site.nextPageCursor
						end
						local num = 0;
						for i,v in pairs(Site.data) do
							local Possible = true
							ID = tostring(v.id)
							if tonumber(v.maxPlayers) > tonumber(v.playing) then
								for _,Existing in pairs(AllIDs) do
									if num ~= 0 then
										if ID == tostring(Existing) then
											Possible = false
										end
									else
										if tonumber(actualHour) ~= tonumber(Existing) then
											local delFile = pcall(function()
												AllIDs = {}
												table.insert(AllIDs, actualHour)
											end)
										end
									end
									num = num + 1
								end
								if Possible == true then
									table.insert(AllIDs, ID)
									wait()
									pcall(function()
										wait()
										game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
									end)
									wait(4)
								end
							end
						end
					end
					function Teleport() 
						while wait() do
							pcall(function()
								TPReturner()
								if foundAnything ~= "" then
									TPReturner()
								end
							end)
						end
					end
					Teleport()
				end        

				function isnil(thing)
						return (thing == nil)
					end
					local function round(n)
						return math.floor(tonumber(n) + 0.5)
					end
					Number = math.random(1, 1000000)
					function UpdatePlayerChams()
						for i,v in pairs(game:GetService'Players':GetChildren()) do
							pcall(function()
								if not isnil(v.Character) then
									if ESPPlayer then
										if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp'..Number) then
											local bill = Instance.new('BillboardGui',v.Character.Head)
											bill.Name = 'NameEsp'..Number
											bill.ExtentsOffset = Vector3.new(0, 1, 0)
											bill.Size = UDim2.new(1,200,1,30)
											bill.Adornee = v.Character.Head
											bill.AlwaysOnTop = true
											local name = Instance.new('TextLabel',bill)
											name.Font = "GothamSemibold"
											name.FontSize = "Size14"
											name.TextWrapped = true
											name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
											name.Size = UDim2.new(1,0,1,0)
											name.TextYAlignment = 'Top'
											name.BackgroundTransparency = 1
											name.TextStrokeTransparency = 0.5
											if v.Team == game.Players.LocalPlayer.Team then
												name.TextColor3 = Color3.new(255,0,0)
											end
										else
											v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..' | '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M \n Health : ' .. round(v.Character.Humanoid.Health) ..' Minutes : ' .. round(v.leaderstats.Minutes.Value))
										end
									else
										if v.Character.Head:FindFirstChild('NameEsp'..Number) then
											v.Character.Head:FindFirstChild('NameEsp'..Number):Destroy()
										end
									end
								end
							end)
							end
						end

						local PADOXHUBMODILE = Instance.new("ScreenGui")
						local MODILEGUIPADOXHUB = Instance.new("TextButton")
						local MODILEGUIPADOXHUBHUI = Instance.new("UICorner")
						local MODILEMAGE = Instance.new("ImageLabel")
						
						MODILEGUIPADOXHUBHUI.Name = "MODILEGUIPADOXHUBHUI"
						MODILEGUIPADOXHUBHUI.Parent = MODILEGUIPADOXHUB
						
						MODILEMAGE.Name = "MODILEMAGE"
						MODILEMAGE.Parent = MODILEGUIPADOXHUB
						MODILEMAGE.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						MODILEMAGE.BackgroundTransparency = 1.000
						MODILEMAGE.BorderSizePixel = 0
						MODILEMAGE.Position = UDim2.new(-0.005, 0,-0.001, 0)
						MODILEMAGE.Size = UDim2.new(0, 50, 0, 50)
						MODILEMAGE.Image = "http://www.roblox.com/asset/?id=11804855180"
						
						PADOXHUBMODILE.Name = "PADOXHUBMODILE"
						PADOXHUBMODILE.Parent = game.CoreGui
						PADOXHUBMODILE.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
						
						MODILEGUIPADOXHUB.Name = "MODILEGUIPADOXHUB"
						MODILEGUIPADOXHUB.Parent = PADOXHUBMODILE
						MODILEGUIPADOXHUB.BackgroundColor3 = Color3.fromRGB(30,20,20)
						MODILEGUIPADOXHUB.Position = UDim2.new(0, 0, 0.491228074, 0)
						MODILEGUIPADOXHUB.Size = UDim2.new(0, 50, 0, 50)
						MODILEGUIPADOXHUB.BackgroundTransparency = 1
						MODILEGUIPADOXHUB.BorderSizePixel = 0
						MODILEGUIPADOXHUB.Draggable = true
						MODILEGUIPADOXHUB.MouseButton1Click:Connect(function()
						game:GetService("VirtualInputManager"):SendKeyEvent(true,305,false,game)
						game:GetService("VirtualInputManager"):SendKeyEvent(false,305,false,game)
					end)

					local Update = loadstring(Game:HttpGet"https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Gui")()
					local PadoUi = Update:Window("Pado","",Enum.KeyCode.RightControl);
					local Main = PadoUi:Tab("General")
					local Combat = PadoUi:Tab("LocalPlayer")
					local Misc = PadoUi:Tab("Misc")

					Main:Seperator("Magicals")

					Main:Button("Lucky Block",function()
						game.ReplicatedStorage.SpawnLuckyBlock:FireServer()
					end)

					Main:Button("Diamond Block",function()
						game.ReplicatedStorage.SpawnDiamondBlock:FireServer()
					end)

					Main:Button("Super Block",function()
						game.ReplicatedStorage.SpawnSuperBlock:FireServer()
					end)

					Main:Button("Rainbow Block",function()
						game.ReplicatedStorage.SpawnRainbowBlock:FireServer()
					end)

					Main:Button("Galaxy Block",function()
						game.ReplicatedStorage.SpawnGalaxyBlock:FireServer()
					end)

					Main:Button("Void Block",function()
						game.ReplicatedStorage.SpawnGalaxyBlock:FireServer()
						game.ReplicatedStorage.SpawnRainbowBlock:FireServer()
						game.ReplicatedStorage.SpawnGalaxyBlock:FireServer()
						game.ReplicatedStorage.SpawnRainbowBlock:FireServer()
						game.ReplicatedStorage.SpawnGalaxyBlock:FireServer()
					end)

					Combat:Seperator("Players")
			
					Playerslist = {}
					
					for i,v in pairs(game:GetService("Players"):GetChildren()) do
						table.insert(Playerslist,v.Name)
					end
					
					local SelectedPly = Combat:Dropdown("Select Players",Playerslist,function(value)
					_G.SelectPly = value
					end)
					
					Combat:Button("Refresh Player",function()
					Playerslist = {}
					SelectedPly:Clear()
					for i,v in pairs(game:GetService("Players"):GetChildren()) do
						SelectedPly:Add(v.Name)
					end
					end)
					
					Combat:Button("Kill Player",function()
						local LocalPlayer = game.Players.LocalPlayer
						Instance.new("Humanoid", LocalPlayer.Character)
						LocalPlayer.Character.Humanoid:Destroy()
						local tool = LocalPlayer.Backpack:FindFirstChildOfClass("Tool")
						local Player = game.Players:FindFirstChild(_G.SelectPly)
						tool.Parent = LocalPlayer.Character
						LocalPlayer.Character["Right Arm"].CFrame = Player.Character.Head.CFrame
						Player.Character:SetPrimaryPartCFrame(tool.Handle.CFrame)
						repeat
							wait()
						until tool.Parent ~= LocalPlayer.Character
						LocalPlayer.Character.Humanoid.Health = 0
						LocalPlayer.Character = nil						
					end)
					
				Combat:Button("Clear Item",function()
				for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
					if v:IsA("Tool") then
							v:Destroy()
						end
					end
				for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetChildren()) do
					if v:IsA("Tool") then
						v:Destroy()
					end
				end
			end)
		
						Combat:Toggle("Spectate Player",false,function(value)
						SpectatePlys = value
						local plr1 = game:GetService("Players").LocalPlayer.Character.Humanoid
						local plr2 = game:GetService("Players"):FindFirstChild(_G.SelectPly)
						repeat wait(.1)
							game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players"):FindFirstChild(_G.SelectPly).Character.Humanoid
						until SpectatePlys == false
						game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players").LocalPlayer.Character.Humanoid
						end)
					
						Combat:Toggle("Teleport",false,function(bool)
						_G.Teleport1 = bool
							while _G.Teleport1 do wait(.1)
								game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players:FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.CFrame * CFrame.new(getgenv().Z,getgenv().Y,getgenv().X)
							end
							StopTween(_G.Teleport1)
						end)
					
						Combat:Toggle("Auto Farm Player",false,function(value)
						_G.Auto_Kill_Ply = value
						StopTween(_G.Auto_Kill_Ply)
						end)
					
						spawn(function()
							while wait(.1) do
								if _G.Auto_Kill_Ply then
									pcall(function()
										if _G.SelectPly ~= nil then
											if game.Players:FindFirstChild(_G.SelectPly) then
												if game.Players:FindFirstChild(_G.SelectPly).Character.Humanoid.Health > 0 then
													repeat wait(.1)
														game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players:FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.CFrame * CFrame.new(getgenv().Z,getgenv().Y,getgenv().X)
													until game.Players:FindFirstChild(_G.SelectPly).Character.Humanoid.Health <= 0 or not game.Players:FindFirstChild(_G.SelectPly) or not _G.Auto_Kill_Ply
												end
											end
										end
									end)
								end
							end
						end)
					
						Combat:Toggle("Auto Click",false,function(value)
						_G.autoclick = value
						end)
					
						spawn(function()
							while wait(.1) do
								if _G.autoclick then
									local VirtualUser = game:GetService('VirtualUser')
									VirtualUser:CaptureController()
									VirtualUser:ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
								end
							end
						end)
					
						Combat:Toggle("Ctrl + Click = TP",false,function(vu)
						CTRL = vu
						end)
					
						local Plr = game:GetService("Players").LocalPlayer
						local Mouse = Plr:GetMouse()
						Mouse.Button1Down:connect(
						function()
							if not game:GetService("UserInputService"):IsKeyDown(Enum.KeyCode.LeftControl) then
								return
							end
							if not Mouse.Target then
								return
							end
							if CTRL then
								Plr.Character:MoveTo(Mouse.Hit.p)
							end
						end
						)

					 _G.HeadSize = 1
				
							Combat:Toggle("Hitbox",false,function(value)
								_G.Disabled = value
							end)
				
							Combat:Slider("Hitbox Size",0,150,1,function(value)
								_G.HeadSize = value
							end)
				
						game:GetService('RunService').RenderStepped:connect(function()
							if _G.Disabled then
							for i,v in next, game:GetService('Players'):GetPlayers() do
							if v.Name ~= game:GetService('Players').LocalPlayer.Name then
							pcall(function()
							v.Character.HumanoidRootPart.Size = Vector3.new(_G.HeadSize,_G.HeadSize,_G.HeadSize)
							v.Character.HumanoidRootPart.Transparency = 1 
							v.Character.HumanoidRootPart.BrickColor = BrickColor.new("Really blue")
							v.Character.HumanoidRootPart.Material = "Smooth Plastic"
							v.Character.HumanoidRootPart.CanCollide = false
						end)
					end
					end
					end
					end)
				
					
						Combat:Seperator("Float")
					
						Combat:Fly()
					
						Combat:Seperator("Identity Info")
					
						Combat:Slider("Walk Speed",0,400,16,function(Value)
						game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value
						end)
					
						Combat:Slider("Jump Hight",0,400,50,function(Value)
						game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value
						end)
					
						Combat:Slider("Gravity",0,400,0, function(value)
						workspace.Gravity = value
						end)

						Combat:Toggle("ESP Player",false,function(value)
							ESPPlayer = value
							while ESPPlayer do wait(.1)
								UpdatePlayerChams()
							end
						end)

					Misc:Seperator("Server")
			
					Misc:Button("Join discord Server",function()
						setclipboard("https://discord.gg/aQEPQA9a8e")
					end)
				
					Misc:Button("Rejoin Server",function()
						game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
					end)
				
					Misc:Button("Hop Server",function()
					Hop()
					end)
				
				Misc:Button("Hop Lower Server",function()
					local Player = game.Players.LocalPlayer
					local Http = game:GetService("HttpService")
					local TPS = game:GetService("TeleportService")
					local Api = "https://games.roblox.com/v1/games/"
				
					local _place,_id = game.PlaceId, game.JobId
					local _servers = Api.._place.."/servers/Public?sortOrder=Desc&limit=100"
					function ListServers(cursor)
						local Raw = game:HttpGet(_servers .. ((cursor and "&cursor="..cursor) or ""))
						return Http:JSONDecode(Raw)
					end
				
					local Next; repeat
					local Servers = ListServers(Next)
					for i,v in next, Servers.data do
						if v.playing < v.maxPlayers and v.id ~= _id then
							local s,r = pcall(TPS.TeleportToPlaceInstance,TPS,_place,v.id,Player)
							if s then break end
						end
					end
				
						Next = Servers.nextPageCursor
					until not Next
				end)
				
				Misc:Button("Destroy Ui",function()
					if game.CoreGui:FindFirstChild("Pado Hub") then
						game.CoreGui:FindFirstChild("Pado Hub"):Destroy()
						game.CoreGui:FindFirstChild("PADOXHUBMODILE"):Destroy()
					end
				end)
				
				Misc:Seperator("Jobid")
				
				Misc:Button("Copy Jobid",function()
					setclipboard(tostring(game.JobId))
				end)
				
				Misc:Textbox("join jobid Link","Type You Link",function(t)
					_G.joinjobid = t
				end)
				
				_G.joinjobid = ""
				
				Misc:Button("Join",function()
					game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId,_G.joinjobid)
				end)
			
				Misc:Seperator("Misc")
			
				Misc:Toggle("Anti AFK", true, function()
					local vu = game:GetService("VirtualUser")
					repeat wait() until game:IsLoaded()
						game:GetService("Players").LocalPlayer.Idled:connect(function()
						game:GetService("VirtualUser"):ClickButton2(Vector2.new())
						vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
						wait(1)
						vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
					end)
				end)
				
					Misc:Toggle("Auto Rejoin",true,function(value)
					_G.AutoRejoin = value
					end)
				
					spawn(function()
						while wait() do
							if _G.AutoRejoin then
								_G.AutoRejoin = game:GetService("CoreGui").RobloxPromptGui.promptOverlay.ChildAdded:Connect(function(child)
									if child.Name == 'ErrorPrompt' and child:FindFirstChild('MessageArea') and child.MessageArea:FindFirstChild("ErrorFrame") then
										game:GetService("TeleportService"):Teleport(game.PlaceId)
									end
								end)
							end
						end
					end)
				
					Misc:Toggle("No Clip",getgenv().noclip,function(value)
					getgenv().noclip = value
					end)
				
				spawn(function()
					game:GetService("RunService").Stepped:Connect(function()
					if getgenv().noclip then
						for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
							if v:IsA("BasePart") then
							v.CanCollide = false
							end
						end
					end
				end)
			end)

					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					wait(1)
					Notification:Notify(
					{Title = "Pado Hub", Description = "Sucessful"},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
					)
				end
				
		if game.PlaceId == 5780309044 then

				local notifSound = Instance.new("Sound",workspace)
				notifSound.PlaybackSpeed = 1.5
				notifSound.Volume = 0.15
				notifSound.SoundId = "rbxassetid://170765130"
				notifSound.PlayOnRemove = true
				notifSound:Destroy()
			
			function Hop()
				local PlaceID = game.PlaceId
				local AllIDs = {}
				local foundAnything = ""
				local actualHour = os.date("!*t").hour
				local Deleted = false
				function TPReturner()
					local Site;
					if foundAnything == "" then
						Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
					else
						Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
					end
					local ID = ""
					if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
						foundAnything = Site.nextPageCursor
					end
					local num = 0;
					for i,v in pairs(Site.data) do
						local Possible = true
						ID = tostring(v.id)
						if tonumber(v.maxPlayers) > tonumber(v.playing) then
						for _,Existing in pairs(AllIDs) do
							if num ~= 0 then
								if ID == tostring(Existing) then
									Possible = false
								end
							else
								if tonumber(actualHour) ~= tonumber(Existing) then
									local delFile = pcall(function()
									AllIDs = {}
									table.insert(AllIDs, actualHour)
									end)
								end
							end
							num = num + 1
						end
						if Possible == true then
							table.insert(AllIDs, ID)
							wait()
							pcall(function()
							wait()
							game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
							end)
							wait(4)
						end
						end
					end
				end
				function Teleport()
					while wait() do
						pcall(function()
						TPReturner()
						if foundAnything ~= "" then
						TPReturner()
						end
						end)
					end
				end
				Teleport()
			end
			
			function TP(Pos)
				Distance = (Pos.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
				if game.Players.LocalPlayer.Character.Humanoid.Sit == true then game.Players.LocalPlayer.Character.Humanoid.Sit = false end
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = Pos
				pcall(function() tween = game:GetService("TweenService"):Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(Distance/260, Enum.EasingStyle.Linear),{CFrame = Pos}) end)
				tween:Play()
				if Distance <= 250 then
					tween:Cancel()
				end
				if _G.StopTween == true then
					tween:Cancel()
					_G.Clip = false
				end
			end
			
			function isnil(thing)
				return (thing == nil)
			end
			local function round(n)
				return math.floor(tonumber(n) + 0.5)
			end
			Number = math.random(1, 1000000)
			function UpdatePlayerChams()
				for i,v in pairs(game:GetService'Players':GetChildren()) do
					pcall(function()
					if not isnil(v.Character) then
						if ESPPlayer then
						if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp'..Number) then
							local bill = Instance.new('BillboardGui',v.Character.Head)
							bill.Name = 'NameEsp'..Number
							bill.ExtentsOffset = Vector3.new(0, 1, 0)
							bill.Size = UDim2.new(1,200,1,30)
							bill.Adornee = v.Character.Head
							bill.AlwaysOnTop = true
							local name = Instance.new('TextLabel',bill)
							name.Font = "GothamSemibold"
							name.FontSize = "Size14"
							name.TextWrapped = true
							name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
							name.Size = UDim2.new(1,0,1,0)
							name.TextYAlignment = 'Top'
							name.BackgroundTransparency = 1
							name.TextStrokeTransparency = 0.5
							if v.Team == game.Players.LocalPlayer.Team then
								name.TextColor3 = Color3.new(255,0,0)
							end
						else
							v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..' | '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M \n Health : ' .. round(v.Character.Humanoid.Health) ..' ₤' .. round(v.Data.Money.Value))
						end
						else
						if v.Character.Head:FindFirstChild('NameEsp'..Number) then
							v.Character.Head:FindFirstChild('NameEsp'..Number):Destroy()
						end
						end
					end
					end)
				end
			end
			
			function UpdateItemESP()
				for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
					pcall(function()
					if ItemESP then
						if not v.Handle:FindFirstChild('NameEsp'..Number) then
						local bill = Instance.new('BillboardGui',v.Handle)
						bill.Name = 'NameEsp'..Number
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1,200,1,30)
						bill.Adornee = v.Handle
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel',bill)
						name.Font = "GothamSemibold"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1,0,1,0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(255, 0, 0)
						name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
						else
						v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
						end
					else
						if v.Handle:FindFirstChild('NameEsp'..Number) then
						v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
						end
					end
					end)
				end
			end
			
			-- CFrame
			Type = getgenv().Mode

			spawn(function()
				while wait() do
					if Type == 1 then
						Farm_Mode = CFrame.new(getgenv().X, getgenv().Y, getgenv().Z)
					end
				end
			end)

			spawn(function()
				pcall(function()
					game:GetService("RunService").Stepped:Connect(function()
						if _G.Auto_Stand or _G.Teleport1 or _G.Auto_Kill_Ply then
						if not game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
							local Noclip = Instance.new("BodyVelocity")
							Noclip.Name = "BodyClip"
							Noclip.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
							Noclip.MaxForce = Vector3.new(100000,100000,100000)
							Noclip.Velocity = Vector3.new(0,0,0)
						end
						for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
							if v:IsA("BasePart") then
								v.CanCollide = false  
							end
						end
					else	
						if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
								game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip"):Destroy()
							end
						end
					end)
				end)
			end)		
			
			function found()
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
				{Title = "Pado Hub", Description = "Found!"},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end
			
			local PADOXHUBMODILE = Instance.new("ScreenGui")
			local MODILEGUIPADOXHUB = Instance.new("TextButton")
			local MODILEGUIPADOXHUBHUI = Instance.new("UICorner")
			local MODILEMAGE = Instance.new("ImageLabel")

			MODILEGUIPADOXHUBHUI.Name = "MODILEGUIPADOXHUBHUI"
			MODILEGUIPADOXHUBHUI.Parent = MODILEGUIPADOXHUB
			
			MODILEMAGE.Name = "MODILEMAGE"
			MODILEMAGE.Parent = MODILEGUIPADOXHUB
			MODILEMAGE.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			MODILEMAGE.BackgroundTransparency = 1.000
			MODILEMAGE.BorderSizePixel = 0
			MODILEMAGE.Position = UDim2.new(-0.005, 0,-0.001, 0)
			MODILEMAGE.Size = UDim2.new(0, 50, 0, 50)
			MODILEMAGE.Image = "http://www.roblox.com/asset/?id=11804855180"
			
			PADOXHUBMODILE.Name = "PADOXHUBMODILE"
			PADOXHUBMODILE.Parent = game.CoreGui
			PADOXHUBMODILE.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			
			MODILEGUIPADOXHUB.Name = "MODILEGUIPADOXHUB"
			MODILEGUIPADOXHUB.Parent = PADOXHUBMODILE
			MODILEGUIPADOXHUB.BackgroundColor3 = Color3.fromRGB(30,20,20)
			MODILEGUIPADOXHUB.BackgroundTransparency = 1
			MODILEGUIPADOXHUB.BorderSizePixel = 0
			MODILEGUIPADOXHUB.Position = UDim2.new(0, 0, 0.491228074, 0)
			MODILEGUIPADOXHUB.Size = UDim2.new(0, 50, 0, 50)
			MODILEGUIPADOXHUB.Font = Enum.Font.SourceSans
			MODILEGUIPADOXHUB.Text = ""
			MODILEGUIPADOXHUB.TextColor3 = Color3.fromRGB(0, 0, 0)
			MODILEGUIPADOXHUB.TextSize = 14.000
			MODILEGUIPADOXHUB.Draggable = true
			MODILEGUIPADOXHUB.MouseButton1Click:Connect(function()
			game:GetService("VirtualInputManager"):SendKeyEvent(true,305,false,game)
			game:GetService("VirtualInputManager"):SendKeyEvent(false,305,false,game)
			end)
		
			local Update = loadstring(Game:HttpGet"https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Gui")()
			local PadoUi = Update:Window("Pado",Enum.KeyCode.RightControl);
			local Main = PadoUi:Tab("General")
			local Combat = PadoUi:Tab("LocalPlayer")
			local Teleport = PadoUi:Tab("Teleport")
			local Shop = PadoUi:Tab("Shop")
			local Misc = PadoUi:Tab("Misc")
		
			local Time = Main:Label("")
			
			spawn(function()
				pcall(function()
					while true do wait(.1)
						Time:Set(game:GetService("Workspace").Time.Value)
					end
				end)
			end)
			
			local Moneya = Main:Label("")
			
			spawn(function()
				pcall(function()
					while true do wait(.1)
						Moneya:Set("Money : "..game:GetService("Players").LocalPlayer.Data.Money.Value)
					end
				end)
			end)

			StandsPls = {"StickyFingers","Anubis","TheWorldOVA","CrazyDiamond","HierophantGreen","DoppioKingCrimson","StarPlatinumTW","TheWorld","StarPlatinumOVA","KingCrimsonAU","TheWorldAlternateUniverse","GoldExperience","KillerQueen","OMT","D4C","Whitesnake","SoftAndWet"}

			Main:Dropdown("Select Stand",StandsPls,function(value)
				_G.StandPly = value
			end)

			Main:Toggle("Auto Found Stand",false,function(value)
				_G.Auto_Stand = value
				StopTween(_G.Auto_Stand)
			end)	
		
				spawn(function()
					while wait(1) do
						if _G.Auto_Stand then
							pcall(function()	
								if game.Players.LocalPlayer.Backpack:FindFirstChild(_G.StandPly) or game.Players.LocalPlayer.Character:FindFirstChild(_G.StandPly) then
									found()
								elseif not game.Players.LocalPlayer.Backpack:FindFirstChild(_G.StandPly) or game.Players.LocalPlayer.Character:FindFirstChild(_G.StandPly) then
										game:service('VirtualInputManager'):SendKeyEvent(true, "Q", false, game)
									if game.Players.LocalPlayer.Backpack:FindFirstChild('Rokakaka Fruit') or game.Players.LocalPlayer.Character:FindFirstChild('Rokakaka Fruit') then
										wait(1)
									 	game.Players.LocalPlayer:findFirstChildOfClass('Backpack')['Rokakaka Fruit'].Parent = game.Players.LocalPlayer.Character
										game:GetService("ReplicatedStorage").ItemEvents.Roka:FireServer()
									if game.Players.LocalPlayer.Backpack:FindFirstChild('Arrow') or game.Players.LocalPlayer.Character:FindFirstChild('Arrow') then
										wait(1)
										game.Players.LocalPlayer:findFirstChildOfClass('Backpack')['Arrow'].Parent = game.Players.LocalPlayer.Character
										game:GetService("ReplicatedStorage").ItemEvents.Arrow:FireServer()
									end
								end
							end
						end)
					end
				end
			end)
			

			Main:Toggle("Auto Found Server Hop ",false,function(value)
				_G.Auto_Stand_Server = value
			end)	
		
				spawn(function()
					while wait(1) do
						if _G.Auto_Stand_Server then
							pcall(function()	
								if game.Players.LocalPlayer.Backpack:FindFirstChild(_G.StandPly) or game.Players.LocalPlayer.Character:FindFirstChild(_G.StandPly) then
									game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
								end
							end)
						end
					end
				end)	


		Main:Toggle("Bring Arrow and Roka",arrowroka,function(a)
			arrowroka = a
		end)

		spawn(function()
			pcall(function()
				while wait(_G.Timebring) do
					if _G.Auto_Stand then
					 	if arrowroka then
							for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
								if v.Name == "Arrow" or v.Name == "Rokakaka Fruit" then
									pcall(function()
										repeat wait()
												v.Handle.CFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,1,0)
												wait() 
												firetouchinterest(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart,v.Handle,0)
												wait()     
											until not arrowroka or not v.Parent or v.Humanoid.Health <= 0
										end)
									end
								end
							end
						end
					end
				end)		
			end)

		_G.Timebring = 0
		Main:Slider("Time Bring %",0,60,0,function(value)
			_G.Timebring = value
		end)
		
			Main:Seperator("Item bank")

		local ItemPls = {"All"
					,"Banknote"
					,"Arrow"
					,"Aja Mask"
					,"Alien"
					,"Blue Heart"
					,"Bone"
					,"Camera"
					,"DIO's Diary"
					,"DIO's Skull 2"
					,"Ender Pearl"
					,"Frog"
					,"Hell Arrow"
					,"Requiem Arrow"
					,"Ornstein's Spear"
					,"Red Heart"
					,"Toxic Chemicals"
					,"Volcanic Rock"
					,"Vampire Mask"
					,"Uncanny Key"
					,"Pot Platinum's Diary"		
					,"Ice Shard"
					,"Canny Key"
					,"Samurai Diary"}
					
					_G.ItemPls = "All"

					Main:Dropdown("Select Item",ItemPls,function(value)
						_G.ItemPls = value
					end)

		Main:Toggle("Auto Farm Item",Item,function(a)
			Item = a
		end)
			
			spawn(function()
				pcall(function()
					while wait(_G.Timebrings) do
						if Item then
							for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
								if v:IsA("Tool") then
									if v.Name == _G.ItemPls or _G.ItemPls == "All" then
										pcall(function()
											repeat wait()
												v.Handle.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0, 0, 0)
												wait()
												firetouchinterest(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart,v.Handle,0)
											until not Item or not v.Parent or v.Humanoid.Health <= 0
										end)
									end
								end
							end
						end
					end
				end)		
			end)
			
			Main:Toggle("Auto Farm Bank",Bank,function(a)
				Bank = a
			end)
			
				spawn(function()
					pcall(function()
						while wait(_G.Timebrings) do
							if Bank then
								repeat wait()
									game:GetService("ReplicatedStorage"):WaitForChild("Bank"):FireServer("Slot1",false,false)
									game:GetService("ReplicatedStorage"):WaitForChild("Bank"):FireServer("Slot2",false,false)
									game:GetService("ReplicatedStorage"):WaitForChild("Bank"):FireServer("Slot3",false,false)
									game:GetService("ReplicatedStorage"):WaitForChild("Bank"):FireServer("Slot4",false,false)
									game:GetService("ReplicatedStorage"):WaitForChild("Bank"):FireServer("Slot5",false,false)
									game:GetService("ReplicatedStorage"):WaitForChild("Bank"):FireServer("Slot6",false,false)
									game:GetService("ReplicatedStorage"):WaitForChild("Bank"):FireServer("Slot7",false,false)
									game:GetService("ReplicatedStorage"):WaitForChild("Bank"):FireServer("Slot8",false,false)
									game:GetService("ReplicatedStorage"):WaitForChild("Bank"):FireServer("Slot9",false,false)
								until not Bank or not v.Parent or v.Humanoid.Health <= 0
							end
						end
					end)
				end)
		
			_G.Timebrings = 0
			Main:Slider("Time Bring %",0,60,0,function(value)
				_G.Timebrings = value
			end)	

 			Main:Seperator("Auto Farm Banknote")

			Main:Toggle("Auto Banknote",getmoneyR,function(a)
				getmoneyR = a
			end)
			
		spawn(function()
			pcall(function()
				while wait() do
					if getmoneyR then
						for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
							if v.Name == "Banknote" then
								pcall(function()
									repeat wait()
										v.Handle.CFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,1,0)
										wait() 
										firetouchinterest(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart,v.Handle,0)
										wait()     
									until not getmoneyR or not v.Parent or v.Humanoid.Health <= 0
								end)
							end
						end
					end
				end
			end)		
		end)	

			Main:Toggle("Auto keep Banknote",getmoney,function(a)
				getmoney = a
			end)
				
					spawn(function()
						pcall(function()
							while wait(1) do
								if getmoney then
									if game.Players.LocalPlayer.Backpack:FindFirstChild("Banknote") or game.Players.LocalPlayer.Character:FindFirstChild("Banknote") <= 0 then
										pcall(function()
											repeat wait(1.1)
												game.Players.LocalPlayer:FindFirstChild('Backpack')['Banknote'].Parent = game.Players.LocalPlayer.Character
												game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
											until not getmoney or not v.Parent or v.Humanoid.Health <= 0
										end)
									end
								end
							end
						end)		
					end)


			Main:Toggle("Auto keep Banknote Hop",getmoneyHop,function(a)
				getmoneyHop = a
			end)

				spawn(function()
					pcall(function()
						while wait(5) do
							if getmoneyHop then
								if game.Players.LocalPlayer.Backpack:FindFirstChild("Banknote") or game.Players.LocalPlayer.Backpack:FindFirstChild("Banknote") then
									else 
										Hop()
											end
										end
									end
								end)
							end)

			Combat:Seperator("Players")
			
			Playerslist = {}
			
			for i,v in pairs(game:GetService("Players"):GetChildren()) do
				table.insert(Playerslist,v.Name)
			end
			
			local SelectedPly = Combat:Dropdown("Select Players",Playerslist,function(value)
			_G.SelectPly = value
			end)
			
			Combat:Button("Refresh Player",function()
			Playerslist = {}
			SelectedPly:Clear()
			for i,v in pairs(game:GetService("Players"):GetChildren()) do
				SelectedPly:Add(v.Name)
			end
			end)
			
			Combat:Toggle("Spectate Player",false,function(value)
				SpectatePlys = value
				local plr1 = game:GetService("Players").LocalPlayer.Character.Humanoid
				local plr2 = game:GetService("Players"):FindFirstChild(_G.SelectPly)
				repeat wait(.1)
					game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players"):FindFirstChild(_G.SelectPly).Character.Humanoid
				until SpectatePlys == false
				game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players").LocalPlayer.Character.Humanoid
				end)
			
				Combat:Toggle("Teleport",false,function(bool)
				_G.Teleport1 = bool
					while _G.Teleport1 do wait()
						game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players:FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.CFrame * CFrame.new(getgenv().Z,getgenv().Y,getgenv().X)
					end
					StopTween(_G.Teleport1)
				end)
			
				Combat:Toggle("Auto Farm Player",false,function(value)
				_G.Auto_Kill_Ply = value
				StopTween(_G.Auto_Kill_Ply)
				end)
			
				spawn(function()
					while wait() do
						if _G.Auto_Kill_Ply then
							pcall(function()
								if _G.SelectPly ~= nil then
									if game.Players:FindFirstChild(_G.SelectPly) then
										if game.Players:FindFirstChild(_G.SelectPly).Character.Humanoid.Health > 0 then
											repeat wait(.1)
												game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players:FindFirstChild(_G.SelectPly).Character.HumanoidRootPart.CFrame * CFrame.new(getgenv().Z,getgenv().Y,getgenv().X)
											until game.Players:FindFirstChild(_G.SelectPly).Character.Humanoid.Health <= 0 or not game.Players:FindFirstChild(_G.SelectPly) or not _G.Auto_Kill_Ply
										end
									end
								end
							end)
						end
					end
				end)
			
				Combat:Toggle("Auto Block",_G.block,function(a)
					_G.block = a
				end)

				spawn(function()
					pcall(function()
						while wait(1) do
							if _G.block then
								pcall(function()
									repeat wait()
									game:GetService("ReplicatedStorage").Main.Input:FireServer("Alternate","Block")
									game:GetService("ReplicatedStorage").Main.Input:FireServer("Alternate","Block",true)
								until not _G.block or not v.Parent or v.Humanoid.Health <= 0
							end)
						end
					end
				end)
			end)

				Combat:Toggle("Auto Click",false,function(value)
				_G.autoclick = value
				end)
			
				spawn(function()
					while wait() do
						if _G.autoclick then
							game:GetService('VirtualUser'):CaptureController()
							game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
						end
					end
				end)
			
				Combat:Toggle("Ctrl + Click = TP",false,function(vu)
				CTRL = vu
				end)
			
				local Plr = game:GetService("Players").LocalPlayer
				local Mouse = Plr:GetMouse()
				Mouse.Button1Down:connect(
				function()
					if not game:GetService("UserInputService"):IsKeyDown(Enum.KeyCode.LeftControl) then
						return
					end
					if not Mouse.Target then
						return
					end
					if CTRL then
						Plr.Character:MoveTo(Mouse.Hit.p)
					end
				end
				)
			
				Combat:Seperator("Other specials")

			
			Combat:Button("click \n rachael but she saw scary thing and now crying",function()
			fireclickdetector(game:GetService("Workspace")["rachael but she saw scary thing and now crying"].ClickDetector)
			end)

			Combat:Toggle("Ticket",_G.Ticket,function(a)
				_G.Ticket = a
			end)

			spawn(function()
				pcall(function()
					while wait(1) do
						if _G.Ticket then
							pcall(function()
								repeat wait()
									game:GetService("Players").LocalPlayer.Data.Ticket.Value = true
								until not _G.Ticket or not v.Parent or v.Humanoid.Health <= 0
							end)
						end
					end
				end)		
			end)
			
			Combat:Toggle("turn off Muisc",false,function(value)
				if value == true then
					game:GetService("Workspace").Music.Playing = false
				else          
					game:GetService("Workspace").Music.Playing = true
				end
			end)

				Combat:Button("Clear Item",function()
					for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
						if v:IsA("Tool") then
								v:Destroy()
							end
						end
					for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetChildren()) do
						if v:IsA("Tool") then
							v:Destroy()
						end
					end
				end)
			
				Combat:Button("Anti Time Stop",function()
				for _,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
					if v.Name == "Anchor" then
						  v:clone().Parent = game:GetService("ReplicatedStorage")
					   end
					end
			
					wait(1)
			
					game:GetService("ReplicatedStorage").Anchor:Destroy()
				end)
			
			
				Combat:Button("Unlimited islands",function()

				local args = {
				    [1] = "Alternate",
				    [2] = "ParticleEvent",
				    [3] = "enable"
				}
				
						game:GetService("ReplicatedStorage").Main.Input:FireServer(unpack(args))
					local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
					local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
					
					wait(1)
					Notification:Notify(
					{Title = "Pado Hub", Description = "Must be a Samurai Only."},
					{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
					)
						end)
			
				Combat:Button("Unlimited Damage Reflection",function()
			local args = {
				[1] = "Alternate",
				[2] = "RTZ",
				[3] = true
			}
			game:GetService("ReplicatedStorage").Main.Input:FireServer(unpack(args))
			local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
			local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
			
			wait(1)
			Notification:Notify(
			{Title = "Pado Hub", Description = "Must be a Gold Experience Requiem Only."},
			{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
			)
			end)
			
			Combat:Button("Unlimited Dodge",function()
			local args = {
				[1] = "Alternate",
				[2] = "STWRTZ",
				[3] = true
			}
			game:GetService("ReplicatedStorage").Main.Input:FireServer(unpack(args))
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				
				wait(1)
				Notification:Notify(
				{Title = "Pado Hub", Description = "Must be a Shadow The World only."},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end)
						
			Combat:Button("Fake Death", function()

			local args = {
			    [1] = true
			}
			
				game:GetService("ReplicatedStorage").Main.Death:FireServer(unpack(args))
			end)
			
			
			Combat:Button("Fake Boost heart", function()
			
			local args = {
			[1] = "Alternate",
			[2] = "Fix",
			[3] = true
			}
			
			game:GetService("ReplicatedStorage").Main.Input:FireServer(unpack(args))
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				
				wait(1)
				Notification:Notify(
				{Title = "Pado Hub", Description = "Must be a Carzy diamoad only."},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end)
	
			Combat:Button("Effect Soft", function()

			local args = {
			    [1] = "Alternate",
			    [2] = "Movement",
			    [3] = true
			}
			
			game:GetService("ReplicatedStorage").Main.Input:FireServer(unpack(args))
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				
				wait(1)
				Notification:Notify(
				{Title = "Pado Hub", Description = "Must be a SoftAndWet only."},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end)
	
			Combat:Button("Menacing",function()
				game:GetService("ReplicatedStorage").Main.Menacing:FireServer(true)
			end)
			
			Combat:Button("Remove Fire",function()
			for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
			pcall(function()
			if v.Name == "Fire" then
			v:Destroy()
			end
			end)
			end
			end)
			
			Combat:Button("Barrage invision ",function()
				game:GetService('UserInputService').InputBegan:Connect(function(key, gameProcessed)
				   if gameProcessed then return end
				   if key.KeyCode == Enum.KeyCode.E then
				       game:GetService("ReplicatedStorage").GoroTeleport:FireServer(CFrame.new(351.104675, 16.5, 882.90564, 0.194466844, 0.164552182, -0.967008412, -3.7252903e-09, 0.985828817, 0.167754769, 0.980909109, -0.0326227359, 0.191711009))
				   end
				end)
				local args = {
				    [1] = "Alternate",
				    [2] = "Barrage"
				}
				
				game:GetService("ReplicatedStorage"):WaitForChild("Main"):WaitForChild("Input"):FireServer(unpack(args))
				game:GetService("ReplicatedStorage").Main.Input:FireServer(unpack(args))
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				
				wait(1)
				Notification:Notify(
				{Title = "Pado Hub", Description = "Must be a DTW only."},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end)

				Combat:Seperator("ESP")
			
				Combat:Toggle("ESP Player",false,function(value)
				ESPPlayer = value
				while ESPPlayer do wait(.1)
					UpdatePlayerChams()
				end
				end)
				
				Combat:Toggle("ESP Item",false,function(value)
				ItemESP = value
				while ItemESP do wait(.1)
					UpdateItemESP()
				end
				end)
							
				Combat:Seperator("Float")
			
				Combat:Fly()
			
				Combat:Seperator("Identity Info")
			
				Combat:Slider("Walk Speed",0,400,16,function(Value)
				game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value
				end)
			
				Combat:Slider("Jump Hight",0,400,50,function(Value)
				game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value
				end)
			
				Combat:Slider("Gravity",0,400,0, function(value)
				workspace.Gravity = value
				end)
			
				Combat:Seperator("Skill Use")
			
				Combat:Toggle("Skill E",false,function(a)
				_G.E = a
				repeat wait(.1)
					game:service('VirtualInputManager'):SendKeyEvent(true, "E", false, game)
				until _G.E == false
				end)
			
				Combat:Toggle("Skill C",false,function(a)
				_G.C = a
				repeat wait(.1)
					game:service('VirtualInputManager'):SendKeyEvent(true, "C", false, game)
				until _G.C == false
				end)
			
				Combat:Toggle("Skill T",false,function(a)
				_G.T = a
				repeat wait(.1)
					game:service('VirtualInputManager'):SendKeyEvent(true, "T", false, game)
				until _G.T == false
				end)
			
				Combat:Toggle("Skill R",false,function(a)
				_G.R = a
				repeat wait(.1)
					game:service('VirtualInputManager'):SendKeyEvent(true, "R", false, game)
				until _G.R == false
				end)
			
				Combat:Toggle("Skill Y",false,function(a)
				_G.Y = a
				repeat wait(.1)
					game:service('VirtualInputManager'):SendKeyEvent(true, "Y", false, game)
				until _G.Y == false
				end)
			
				Combat:Toggle("Skill F",false,function(a)
				_G.F = a
				repeat wait(.1)
					game:service('VirtualInputManager'):SendKeyEvent(true, "F", false, game)
				until _G.F == false
				end)
			
				Combat:Toggle("Skill X",false,function(a)
				_G.X= a
				repeat wait(.1)
					game:service('VirtualInputManager'):SendKeyEvent(true, "X", false, game)
				until _G.X == false
				end)
			
				Combat:Toggle("Skill H",false,function(a)
				_G.H= a
				repeat wait(.1)
					game:service('VirtualInputManager'):SendKeyEvent(true, "H", false, game)
				until _G.H == false
				end)
			
				Teleport:Seperator("Teleport")

				Teleport:Button("Arena",function()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1121.18225, 583.293335, -680.932434, 0.998740196, 1.05270637e-07, 0.0501801185, -1.0422832e-07, 1, -2.33882584e-08, -0.0501801185, 1.81286044e-08, 0.998740196)				
				end)

				Teleport:Button("ABD Map",function()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1391.58887, 587.66864, -432.658356, 0.00209909398, 3.51848928e-09, 0.999997795, 1.52867532e-08, 1, -3.55058538e-09, -0.999997795, 1.52941713e-08, 0.00209909398)
				end)

				Teleport:Button("Bank",function()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1342.41565, 587.622925, -553.506531, 0.999499857, -9.45195655e-09, 0.0316238143, 7.48851381e-09, 1, 6.22059062e-08, -0.0316238143, -6.19379747e-08, 0.999499857)
				end)

				Teleport:Button("Stadium",function()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1248.16333, 583.668091, -280.276031, -0.00195235433, 2.6514547e-08, 0.999998093, 2.36975133e-08, 1, -2.64683315e-08, -0.999998093, 2.36457929e-08, -0.00195235433)
				end)

				Teleport:Button("WareHouse",function()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1386.86621, 604.741943, -284.569641, -0.97431308, 6.82178367e-08, -0.225197792, 6.5325203e-08, 1, 2.02960848e-08, 0.225197792, 5.06364861e-09, -0.97431308)
				end)
				
				Teleport:Button("Camp Fire",function()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1529.41553, 585.047791, -289.651703, 0.767191172, -9.26921473e-09, 0.641418517, 1.32677613e-09, 1, 1.28641808e-08, -0.641418517, -9.01826702e-09, 0.767191172)
				end)

				Teleport:Button("Farming Zone",function()
					game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-303.969604, 463.317749, -1495.84753, -0.487106264, 9.1222141e-08, -0.873342693, 1.07882112e-08, 1, 9.84345974e-08, 0.873342693, 3.85263021e-08, -0.487106264)
				end)

				Shop:Seperator("Gui")
			
				Shop:Button("Tom Shop",function()
					game:GetService("Players").LocalPlayer.PlayerGui.ShopGUI.Enabled = true
				end)
				
				Shop:Button("Tim Shop",function()
					game:GetService("Players").LocalPlayer.PlayerGui.ShopGUI2.Enabled = true
				end)

				Shop:Button("Timmy Shop",function()
					fireclickdetector(game:GetService("Workspace").Map.Timmy.ClickDetector)
 				end)

				Shop:Button("Store Bank",function()
					game:GetService("ReplicatedStorage").Bank:FireServer("Slot1",false,false)
					game:GetService("ReplicatedStorage").Bank:FireServer("Slot2",false,false)
					game:GetService("ReplicatedStorage").Bank:FireServer("Slot3",false,false)
					game:GetService("ReplicatedStorage").Bank:FireServer("Slot4",false,false)
					game:GetService("ReplicatedStorage").Bank:FireServer("Slot5",false,false)
					game:GetService("ReplicatedStorage").Bank:FireServer("Slot6",false,false)
					game:GetService("ReplicatedStorage").Bank:FireServer("Slot7",false,false)
					game:GetService("ReplicatedStorage").Bank:FireServer("Slot8",false,false)
				end)

				Shop:Seperator("SHOPS")

				Shop:Button("Arrow [ $500 ]",function()
				game:GetService("ReplicatedStorage").Purchase:FireServer("Arrow")
				end)
			
				Shop:Button("Rokakaka Fruit [ $250 ]",function()
				game:GetService("ReplicatedStorage").Purchase:FireServer("Rokakaka Fruit")
				end)
			
				Shop:Button("Sword [ $13500 ]",function()
				game:GetService("ReplicatedStorage"):WaitForChild("Purchase"):FireServer("sword")
				end)
			
				Shop:Button("Shiny Arrow [ $1500 ]",function()
				game:GetService("ReplicatedStorage").Purchase:FireServer("Shiny Arrow")
				end)
			
				Shop:Button("Shin Sword [ $100000 ]",function()
				game:GetService("ReplicatedStorage"):WaitForChild("Purchase"):FireServer("shinysword")
				end)

				Shop:Button("Hamon [ $50000 ]",function()
					game:GetService("ReplicatedStorage").Purchase:FireServer("Hamon")
				end)	
			
				Shop:Button("Water [ $10 ]",function()
				game:GetService("ReplicatedStorage").Purchase:FireServer("Water")
				end)
			
				Shop:Button("Ticket [ $12000 ]",function()
				game:GetService("ReplicatedStorage").Purchase:FireServer("Ticket")
				end)
			
				Misc:Seperator("Server")
			
				Misc:Button("Join discord Server",function()
				local request = request or http_request or (syn and syn.request)
				if not request then return end
				local start = 6463
				local invCode = 'aQEPQA9a8e'
				for i = start-10, start+1 do
					spawn(function()
					pcall(function()
					request({Url = "http://127.0.0.1:"..tostring(i).."/rpc?v=1",Method = "POST",Headers = {["Content-Type"] = "application/json",["Origin"] = "https://discord.com"},Body = game:GetService("HttpService"):JSONEncode({["cmd"] = "INVITE_BROWSER",["nonce"] = game:GetService("HttpService"):GenerateGUID(false),["args"] = {["invite"] = {["code"] = invCode,},["code"] = invCode}})})
					end)
					end)
				end
				end)
			
				Misc:Button("Rejoin Server",function()
				game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
				end)
			
				Misc:Button("Hop Server",function()
				Hop()
				end)
			
				Misc:Button("Hop Lower Server",function()
				local Player = game.Players.LocalPlayer
				local Http = game:GetService("HttpService")
				local TPS = game:GetService("TeleportService")
				local Api = "https://games.roblox.com/v1/games/"
			
				local _place,_id = game.PlaceId, game.JobId
				local _servers = Api.._place.."/servers/Public?sortOrder=Desc&limit=100"
				function ListServers(cursor)
					local Raw = game:HttpGet(_servers .. ((cursor and "&cursor="..cursor) or ""))
					return Http:JSONDecode(Raw)
				end
			
				local Next; repeat
				local Servers = ListServers(Next)
				for i,v in next, Servers.data do
					if v.playing < v.maxPlayers and v.id ~= _id then
						local s,r = pcall(TPS.TeleportToPlaceInstance,TPS,_place,v.id,Player)
						if s then break end
					end
				end
			
				Next = Servers.nextPageCursor
			until not Next
			end)
			
			Misc:Button("Destroy Ui",function()
			if game.CoreGui:FindFirstChild("Pado Hub") then
				game.CoreGui:FindFirstChild("Pado Hub"):Destroy()
				game.CoreGui:FindFirstChild("PADOXHUBMODILE"):Destroy()
			end
			end)
			
			Misc:Seperator("Jobid")
			
			Misc:Button("Copy Jobid",function()
			setclipboard(tostring(game.JobId))
			end)
			
			Misc:Textbox("join jobid Link","Type You Link",function(t)
			_G.joinjobid = t
			end)
			
			_G.joinjobid = ""
			
			Misc:Button("Join",function()
			game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId,_G.joinjobid)
			end)
			
			Misc:Seperator("Farm Distance X/Y/Z Settings")
			
			getgenv().X = 4
			
			Misc:Slider("Farm (X)",1,60,4,function(value)
			getgenv().X = value
			end)
			
			Misc:Slider("Farm (Y)",1,60,0,function(value)
			getgenv().Y = value
			end)
			
			Misc:Slider("Farm (Z)",1,60,0,function(value)
			getgenv().Z = value
			end)

			Misc:Seperator("Misc")
			
			Misc:Toggle("Anti AFK", true, function()
			local vu = game:GetService("VirtualUser")
			repeat wait() until game:IsLoaded()
			game:GetService("Players").LocalPlayer.Idled:connect(function()
			game:GetService("VirtualUser"):ClickButton2(Vector2.new())
			vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
			wait(1)
			vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
			end)
			end)
			
				Misc:Toggle("Auto Rejoin",true,function(value)
				_G.AutoRejoin = value
				end)
			
				spawn(function()
					while wait() do
						if _G.AutoRejoin then
							_G.AutoRejoin = game:GetService("CoreGui").RobloxPromptGui.promptOverlay.ChildAdded:Connect(function(child)
								if child.Name == 'ErrorPrompt' and child:FindFirstChild('MessageArea') and child.MessageArea:FindFirstChild("ErrorFrame") then
									game:GetService("TeleportService"):Teleport(game.PlaceId)
								end
							end)
						end
					end
				end)
			
				Misc:Toggle("No Clip",getgenv().noclip,function(value)
				getgenv().noclip = value
				end)
			
					spawn(function()
						game:GetService("RunService").Stepped:Connect(function()
							if getgenv().noclip then
								for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
									if v:IsA("BasePart") then
									v.CanCollide = false
									end
								end
							end
						end)
					end)
			
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
				{Title = "Pado Hub", Description = "Sucessful"},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end
		
			if game.PlaceId == 11423467063 then
	
				local Update = loadstring(Game:HttpGet"https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Gui")()
				local PadoUi = Update:Window("Pado",Enum.KeyCode.RightControl);
				local Boss = PadoUi:Tab("Boss")
				
				Boss:Button("BeboScript","Gives You an OP gui",function()
				loadstring(game:HttpGet("https://raw.githubusercontent.com/Bebo-Mods/BeboScripts/main/StandAwekening.lua"))()
				end)
				 
				Boss:Button("God Mode","Gives God mode (W?)",function()
				loadstring(game:HttpGet("https://raw.githubusercontent.com/Just3itx/Deezs/main/Games/Stands%20Awakening/Loader.lua"))()
				end)
				 
				Boss:Button("No Cooldown","Gives you no cooldown (Use with auto kill)",function()
				loadstring(game:HttpGet(('https://raw.githubusercontent.com/itsyouranya/free/main/Anya%20Stands%20Awakening%20Helper.lua'),true))()
				end)
				 
				Boss:Button("Auto Kill (Recommended)",function()
				getgenv().WaitTime = 420
				loadstring(game:HttpGet("https://raw.githubusercontent.com/sunexn/standsawakening/main/uncanny.lua",true))() -- open source
				end)			
								
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
				{Title = "Pado Hub", Description = "Sucessful"},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end
		
	if game.PlaceId == 13621938427 then
			
			local notifSound = Instance.new("Sound",workspace)
			notifSound.PlaybackSpeed = 1.5
			notifSound.Volume = 0.15
			notifSound.SoundId = "rbxassetid://170765130"
			notifSound.PlayOnRemove = true
			notifSound:Destroy()	
			
			local PADOXHUBMODILE = Instance.new("ScreenGui")
			local MODILEGUIPADOXHUB = Instance.new("TextButton")
			local MODILEGUIPADOXHUBHUI = Instance.new("UICorner")
			local MODILEMAGE = Instance.new("ImageLabel")

			MODILEGUIPADOXHUBHUI.Name = "MODILEGUIPADOXHUBHUI"
			MODILEGUIPADOXHUBHUI.Parent = MODILEGUIPADOXHUB
			
			MODILEMAGE.Name = "MODILEMAGE"
			MODILEMAGE.Parent = MODILEGUIPADOXHUB
			MODILEMAGE.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			MODILEMAGE.BackgroundTransparency = 1.000
			MODILEMAGE.BorderSizePixel = 0
			MODILEMAGE.Position = UDim2.new(-0.005, 0,-0.001, 0)
			MODILEMAGE.Size = UDim2.new(0, 50, 0, 50)
			MODILEMAGE.Image = "http://www.roblox.com/asset/?id=11804855180"
			
			PADOXHUBMODILE.Name = "PADOXHUBMODILE"
			PADOXHUBMODILE.Parent = game.CoreGui
			PADOXHUBMODILE.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			
			MODILEGUIPADOXHUB.Name = "MODILEGUIPADOXHUB"
			MODILEGUIPADOXHUB.Parent = PADOXHUBMODILE
			MODILEGUIPADOXHUB.BackgroundColor3 = Color3.fromRGB(30,20,20)
			MODILEGUIPADOXHUB.BackgroundTransparency = 1
			MODILEGUIPADOXHUB.BorderSizePixel = 0
			MODILEGUIPADOXHUB.Position = UDim2.new(0, 0, 0.491228074, 0)
			MODILEGUIPADOXHUB.Size = UDim2.new(0, 50, 0, 50)
			MODILEGUIPADOXHUB.Font = Enum.Font.SourceSans
			MODILEGUIPADOXHUB.Text = ""
			MODILEGUIPADOXHUB.TextColor3 = Color3.fromRGB(0, 0, 0)
			MODILEGUIPADOXHUB.TextSize = 14.000
			MODILEGUIPADOXHUB.Draggable = true
			MODILEGUIPADOXHUB.MouseButton1Click:Connect(function()
			game:GetService("VirtualInputManager"):SendKeyEvent(true,305,false,game)
			game:GetService("VirtualInputManager"):SendKeyEvent(false,305,false,game)
			end)
			
			local Update = loadstring(Game:HttpGet"https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Gui")()
			local PadoUi = Update:Window("Pado",Enum.KeyCode.RightControl);
			local Main = PadoUi:Tab("General")
			local Combat = PadoUi:Tab("LocalPlayer")
			
			
			
				local NotificationHolder = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication"))()
				local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/REWzaKunGz1/premium/main/Nofitication_2"))()
				wait(1)
				Notification:Notify(
				{Title = "Pado Hub", Description = "Sucessful"},
				{OutlineColor = Color3.fromRGB(80, 80, 80),Time = 5, Type = "default"}
				)
			end
