game:GetService("minatoz"):SetCore("SendNotification", {
title = "minatoz hub",
duration = 6
})wait(2)game:GetService("minatoz"):SetCore("SendNotification", {
  Title = "script carregando?:",
  Text = "aguarde.",
  Button1 = "entendi",
  Duration = 10
})

local a=loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()

--window

local Window = Library.CreateLib("minatoz hub", "LightTheme")

--tabs

local Tab = Window:NewTab("beta")

Section:NewLabel("troll")
Section:NewLabel("carro")
Section:NewLabel("roupas")
Section:NewLabel("casas")

funcoes

Section:NewButton("selecionar jogador", "minato hub v1", function()
    print("minatoz hub beta")
end)

Section:NewToggle("velocidade", "ToggleInfo", function(state)
    if state then
        print("velocidade on")
    else
        print("velocidade Off")
    end
end)

Section:NewToggle("pulo do jogador", "ToggleInfo", function(state)
    if state then
        print("pulo on")
    else
        print("pulo Off")
    end
end)

Section:NewSlider("quantidade", "SliderInfo", 500, 0, function(s) -- 500 (500) | 0 (0)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

Section:NewSlider("SliderText", "SliderInfo", 500, 0, function(s) -- 500 (500) | 0 (0)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)







