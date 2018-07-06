# Ceci est un script pour booster vos voitures IG
[INSTALLATION]
1) Mettre le fichier "boostvoiture" dans votre dossier resource [../fxserver/resource]
2) start votre fichier: start boostvoiture

# ########################################################################
  Citizen.CreateThread(function()
   while true do
    Citizen.Wait(0)
    if IsVehicleModel(GetVehiclePedIsIn(GetPlayerPed(-1), true), GetHashKey("Nom de la voiture")) then
       SetVehicleEnginePowerMultiplier(GetVehiclePedIsIn(GetPlayerPed(-1), true), 2.5)
       SetVehicleEngineTorqueMultiplier(GetVehiclePedIsIn(GetPlayerPed(-1), true), 2.5)
     end
   end
 end)
 
# Vous avez juste à remplacer le "Nom de la voiture" par le nom de la voiture que vous voulez boost
# Un exemple :

  Citizen.CreateThread(function()
   while true do
    Citizen.Wait(0)
    if IsVehicleModel(GetVehiclePedIsIn(GetPlayerPed(-1), true), GetHashKey("t20")) then
       SetVehicleEnginePowerMultiplier(GetVehiclePedIsIn(GetPlayerPed(-1), true), 2.5)
       SetVehicleEngineTorqueMultiplier(GetVehiclePedIsIn(GetPlayerPed(-1), true), 2.5)
     end
   end
 end)
 
 
# Et le 2.5 vosu le changez en ce que vous voulez, il faut savoir que plus vous augmentez ce chiffre, plus la voiture ira vite, 2.5 c'est # deja tres bien !
