<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Scripts Roblox</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
      padding: 20px;
      max-width: 800px;
      margin: auto;
    }
    h1 {
      color: #333;
    }
    .script {
      background-color: #fff;
      border-radius: 5px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      padding: 15px;
      margin-bottom: 20px;
    }
    pre {
      background-color: #272822;
      color: #f8f8f2;
      padding: 10px;
      border-radius: 3px;
      overflow-x: auto;
    }
  </style>
</head>
<body>
  <h1>Scripts de Roblox</h1>

  <div class="script">
    <h2>Exemplo: Script para dar saltos altos</h2>
    <pre>
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

humanoid.JumpPower = 100 -- define o poder de salto para 100
    </pre>
  </div>

  <div class="script">
    <h2>Exemplo: Script para coletar moedas</h2>
    <pre>
local player = game.Players.LocalPlayer
local coins = workspace.Coins:GetChildren()

for i, coin in pairs(coins) do
  if (coin.Position - player.Character.HumanoidRootPart.Position).magnitude &lt; 10 then
    coin:Destroy() -- remove a moeda
  end
end
    </pre>
  </div>

</body>
</html>
