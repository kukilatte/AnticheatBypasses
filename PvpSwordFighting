if game.PlaceId==7918735461 then --You use it in this game
Fucker = hookmetamethod(game, "__namecall", function(Self,ThatTable,...)
	local ncm = getnamecallmethod()
	if not checkcaller() and tostring(Self)=="checkState" and ncm:lower()=="fireserver" then
		local cstate=game.ReplicatedStorage.acevents.checkState
		local tbl=ThatTable
		if tbl.WalkSpeed>16 or tbl.Flying==true or tbl.Kick==true or tbl.JumpPower>50 then
			local newtable={
				Kick = false,
				Flying = false,
				JumpPower = 50,
				WalkSpeed = 16,
			}
			return cstate:FireServer(newtable)
		end
		return Fucker(Self,ThatTable,...)
	end
	return Fucker(Self,ThatTable,...)
end)
Bypass = hookmetamethod(game, "__namecall", function(Self, Reason,...)
    local ncm = getnamecallmethod()
    if Self == game.Players.LocalPlayer and ncm:lower() == "kick" then
        if Reason=="Exploits detected!" then
            return BypassScript
        end
    end
    return Bypass(Self,Reason,...)
end)
else
	warn("Wrong game dumb fuck") --yes
end
