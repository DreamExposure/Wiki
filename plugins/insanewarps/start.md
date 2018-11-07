# InsaneWarps
InsaneWarps introduces better handling of warps, spawns, tpr and more with new unique mechanics. Locations can easily be set and controlled with permissions and delays. Signs can be used for quick commandless teleports. And add more immersive features like a GTA 5 style teleportation! 

Purchase and Download now: https://www.spigotmc.org/resources/insanewarps.61941/


# Features
* Warp/Hub/Lobby/Spawn handling
* Respawn handling
* Spawn sharing (Die in the Nether, respawn in the Overworld)
* TPR (Randomly teleport to a location far away)
* Teleportation Upon Join (foce a player to teleport to the spawn or other locations when they join the server)
* Multiblock structures
	* Portal (Step into a portal and teleport)
	*  Platform (Stand or crouch on a platform to teleport)
	*  ItemBlock (Floating item above a block to represent the location, right click the sign to teleport)
* Holograms for multiblock structures
* Teleport signs
* GTA V teleportation animation
* Economy integration
* And more! Don't see a feature? Request it on our discord!

# Planned Features
* Particle Effects and Particle animations
* Inventory menus
* Integrated support for Bungee networks (transfer servers seamlessly)
* And more! Don't see a feature? Request it on our discord!

# Installation
MAKE SURE TO ALSO DOWNLOAD NOVALIB: https://jenkins.dreamexposure.org/job/NovaLib/

Installation of NovaLib is really simple. Download the latest version from the official spigot page, then just drag and drop the .jar file into your plugins folder.
Fully stop and then start the server to generate the default configuration. Configure the plugin to your liking and completely stop and then start the server once again.

Please do not use /reload as that is meant only for developers and should NEVER be used in a production environment.

## Dependencies
* NovaLib: https://jenkins.dreamexposure.org/job/NovaLib/
* (Optional for economy support) Vault: https://www.spigotmc.org/resources/vault.34315/

# Configuration
## Config.yml
The config.yml is simple to understand and setup. Its default values are set to balance existing mechanics with new ones. 


```yaml
DO NOT DELETE:
  A: InsaneWarps is developed and managed by DreamExposure
  B: Replicating or sharing this plugin without our approval will result in legal
    action
# Whether or not to check for updates and/or download the update
Updates:
  Check: true
  Download: false
# Used for extra debug info in the console. Use this to help figure out any issues
Console:
  Debug: false
  Verbose: false
# Select the language (currently only English is supported)
Language: EN_US
Economy:
  # Whether or not to enable econ settings.
  Enabled: false
  # Whether or not to allow users with econ bypass to bypass the economy costs
  Use Bypass Permission: true
# Settings for teleportation upon join
Join:
  Teleport:
    Enabled: false
    Type: SPAWN
    LocName: world
	# Whether or not to allow users with join bypass to bypass the teleportation
    AllowBypass: true
Warp:
  Delay:
    Enabled: false
    Seconds: 5
Hub:
  Delay:
    Enabled: false
    Seconds: 5
Lobby:
  Delay:
    Enabled: false
    Seconds: 5
Spawn:
  Delay:
    Enabled: false
    Seconds: 5
Respawn:
  Handle: true
TPR:
  Enabled: true
  Delay:
    Enabled: false
    Seconds: 5
  Cooldown:
    Enabled: true
    Seconds: 3600
  Cost: 0.0
  # Max distance, in blocks, that the player may be teleported
  Max Distance: 1000
  # Worlds where tpr can be used.
  Worlds:
  - world
# Teleport mechanics settings
Teleport:
  GTA Style:
    Enabled: true
	# How many stages there are. GTA 5 has 3.
    Drops Up: 3
	# Y coordinate height to go to.
    Target Y: 150
	# Delay in seconds for each stage.
    Drop Delay: 1
	# Delay in seconds for each stage down.
    Down Delay: 1
	# The sound played for each stage.
    Sound: ENTITY_EXPERIENCE_ORB_PICKUP
# Multiblock structure settings
Structure:
  PORTAL:
	# Allow portals
    Enabled: true
	# Base of portal where sign is displayed
    Base: SEA_LANTERN
	# Portal frame
    Frame: BLACK_CONCRETE
    Portal:
	  # If the inside of the portal is a nether portal
      NetherPortal: true
	  # If the inside of the portal is water (if both false, its air)
      Water: false
  PLATFORM:
    Enabled: true
    Base: SEA_LANTERN
    Center: LAPIS_BLOCK
    Sides: BLACK_CONCRETE
    Corners: GLOWSTONE
    Hologram:
      Enabled: true
      Text:
        WithCrouch: '&6Crouch here to teleport!'
        NoCrouch: '&6Stand here to teleport!'
	# Whether or not to make players crouch to teleport
    Crouch:
      Require: true
  ITEM_BLOCK:
    Enabled: true
    Base: SEA_LANTERN
	# Show floating item above base block.
    ShowItem: true
    Hologram:
      Enabled: true
      Text: '&6Click sign to teleport!'
```


## World Shares
For the world shares, a very simple format is used. 

```yaml
#default values
world_nether: world
world_the_end: world

#A very simple format example:
#world_name_from: world_name_to
```


# Commands & Permissions
## Commands


## Permissions

# Advanced Features
* Signs: 
* Multiblock structures: 

# Additional Links
* Discord Support Server: https://discord.gg/2TFqyuy
* SpigotMC page: https://www.spigotmc.org/resources/insanewarps.61941/
* Minecraft Server: mc.dreamexposure.org