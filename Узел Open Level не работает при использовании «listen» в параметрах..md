https://forums.unrealengine.com/t/open-level-node-doesnt-work-when-using-listen-in-the-options/1182174

[/Script/Engine.GameEngine] !NetDriverDefinitions=ClearArray +NetDriverDefinitions=(DefName="GameNetDriver",DriverClassName="/Script/SteamSockets.SteamSocketsNetDriver",DriverClassNameFallback="/Script/SteamSockets.SteamNetSocketsNetDriver")

Мне пришлось поместить это в начало моего файла DefaultEngine.ini: