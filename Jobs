--[[---------------------------------------------------------------------------
DarkRP custom jobs
---------------------------------------------------------------------------
This file contains your custom jobs.
This file should also contain jobs from DarkRP that you edited.

Note: If you want to edit a default DarkRP job, first disable it in darkrp_config/disabled_defaults.lua
      Once you've done that, copy and paste the job to this file and edit it.

The default jobs can be found here:
https://github.com/FPtje/DarkRP/blob/master/gamemode/config/jobrelated.lua

For examples and explanation please visit this wiki page:
https://darkrp.miraheze.org/wiki/DarkRP:CustomJobFields

Add your custom jobs under the following line:
---------------------------------------------------------------------------]]
--[[
    Property Manager Job
    Generated using: DarkRP | Job Generator
    https://yourdevtools.com/gmod/darkrp-job
--]]

TEAM_CORPORATE = DarkRP.createJob("Property Manager", {
    color = Color(234, 234, 0),
    model = {
        "models/fearless/dbsuit07.mdl",
        "models/fearless/dbsuit07.mdl",
        "models/fearless/bsuit04.mdl",
        "models/fearless/dgsuit12.mdl",
        "models/fearless/gsuit15.mdl",
        "models/player/suits/male_01_closed_tie.mdl",
        "models/suits/group1/male_01_open.mdl",
        "models/suits/group3/male_01_open.mdl"
    },
    description = [[
        Manager of all property in the city
    ]],
    weapons = {},
    command = "propertymanager",
    max = 3,
    salary = 35,
    admin = 0,
    vote = false,
    hasLicense = false,
    category = "Business",
    canDemote = false,
    customCheck = function(ply) 
        return CLIENT or table.HasValue({"Hotelcorp"}, ply:GetUserGroup()) 
    end,
    CustomCheckFailMsg = "You havent been whitelisted for this job!",
})


--[[---------------------------------------------------------------------------
Define which team joining players spawn into and what team you change to if demoted
---------------------------------------------------------------------------]]
GAMEMODE.DefaultTeam = TEAM_CITIZEN
--[[---------------------------------------------------------------------------
Define which teams belong to civil protection
Civil protection can set warrants, make people wanted and do some other police related things
---------------------------------------------------------------------------]]
GAMEMODE.CivilProtection = {
    [TEAM_POLICE] = true,
    [TEAM_CHIEF] = true,
    [TEAM_MAYOR] = true,
}
--[[---------------------------------------------------------------------------
Jobs that are hitmen (enables the hitman menu)
---------------------------------------------------------------------------]]
DarkRP.addHitmanTeam(TEAM_MOB)
