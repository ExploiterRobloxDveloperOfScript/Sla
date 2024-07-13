local function onCommand(player, command)
    if command == "kick" then
        -- Implemente a lógica para expulsar o jogador
    elseif command == "ban" then
        -- Implemente a lógica para banir o jogador
    elseif command == "char" then
        -- Implemente a lógica para alterar o personagem do jogador
    elseif command == "sit" then
        -- Implemente a lógica para fazer o jogador sentar
    elseif command == "kill" then
        -- Implemente a lógica do jogador matar qualquer jogador
    elseif command == "explode" then
        -- Implemente a lógica do jogador explodir qualquer outro jogador
     end
end

game.Players.PlayerAdded:Connect(function(player)
    player.Chatted:Connect(function(message)
        local command = message:lower()
        onCommand(player, command)
    end)
end)
