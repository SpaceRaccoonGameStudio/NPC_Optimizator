# v.1.6.3

### Fixed:
- Issue with wrong change wave event execution
- Return missed variable - "Disable Optimizations On Listen Server" (by default: false)
- Crash on some cases

### Added: 
- New option "Disable optimization on dedicated server" (by default: true)
- Groom component optimization for metahumans
- Add support non pawn/characters actors

# v.1.6.2

### Improved:
- Clean up code

### Fixed:
- Issue with package in shipping build

### Added:
- Blueprint function 'EnableForceOptimizationWave'

# v.1.6.0

### Fixed:
- In some cases skeletal meshes with optimization component have visual glitch

# v.1.5.9

### Fixed:
- Issue with max culling distance for skeletal meshes

### Known issues:
- In some cases skeletal meshes with optimization component have visual glitch. We work on fix this bug now.

# v.1.5.8

### Added:
- Official UE5 support

# v.1.5.7

### Fixed:
- Crash on some cases

### Added:
- New parameter : “IgnoreOptimizationTag” - Special tag to ignore any component optimizations 


# v.1.5.6

### Fixed:
-  Crash on some cases

# v.1.5.5

### Fixed:
-  Missed some settings for invisible wave

### Added:
- New parameter : "Ignore camera sight" - Enable this setting in order to ignore the calculation of the visibility of NPCs by the camera and calculate optimization waves only by distance. 
- New parameter: "Ignore camera sight in no optimization distance" - Ignore camera visibility when bots are close to the player. It's about the distance to the first wave of optimization. If the bots are within this distance, they will automatically switch to the "no optimization" state, regardless of whether the camera sees them or not. 

# v.1.5.4

### Tweaked:
- Added possibility change setting for invisible wave

# v.1.5.3

### Fixed: 
- Fixed behavior of a ragdoll after disabling all optimizations

# v.1.5.2

### Fixed: 
- Issue with ticking actors

# v.1.5

### Added:
- 4.27 support
- PS4, XboxOne, IOS support

### Fixed: 
- Issue with skip interpolation update for kinematic bones
	 
# v.1.4.3

### Fixed: 
- Minor issue with physics channels
- Static mesh hiding method

# v.1.4.2

### Fixed: 
- Issue with missed NPC_OPTIMIZATOR_API definition in optimization component

### Added:
- Possibility hide attached static meshes for every wave
- New blueprint event “OnChangeWave” - It’s executed when an optimization component goes to some optimization wave. Can be very helpful for done some custom logic 

# v.1.4.1

### Added:
- Added possibility hide static meshes attached to skeletal meshes (enabled by default)

### Tweaked:
- Updated documentation about troubleshooting

# v.1.4

### Added:
- Plugin stat command stat NPC_Optimizator - provide statistic about optimizations
- Console variable npc.optimizator.fov (default 90). Used for setting FOV for optimization
- Console variable npc.optimizator.MaxOptimizedOnOneFrame (default 15). How many bots can be optimized in one optimization thread tick. A lower value reduces the synchronization delay with the main thread, but worsens the visual perception
- Console variable npc.optimizator.DrawDebug (default 0) - Can be used for enable draw debug

### Tweaked:
- More optimization in some cases 

# v.1.3

### Fixed:
- Crash on some case

### Tweaked:
- More optimization in some cases

# v.1.2

### Fixed: 
- Issue with flying some characters in no optimization wave
- Issue with self controlled optimizated character

### Added:
- Blueprint function "DisableAllOptimizations"

### Tweaked: 
- MORE optimization logic & tweaks
- Added new potato mode to example project 
- Now have ~ +20-40 fps in some scenarios
- Updated demo project
- Update example project