
# bshift-xash-rt
### Half Life: Blue Shift ray traced using the [xash-rt](https://github.com/sultim-t/xash-rt) engine built by [sultim-t](https://github.com/sultim-t).

#### This repo is used as a staging ground for all the changes I need to do to maps, files, models in the Blue Shift campaign for Half-Life in order to get it functional and playable in the engine. [Opposing force might've been easier to start with, but YOLO]


### Previews:
![Start of the game](https://img.boofi.dev/u/gebD6r.jpg)
![Start of the game 2](http://img.boofi.dev/u/5yF0tE.jpg)
![ba_tram2](http://img.boofi.dev/u/pcWfgq.jpg)

### What does this require?
#### You will need to:

 1. Compile hlsdk-portable's bshift branch (Found [here](https://github.com/FWGS/hlsdk-portable/tree/bshift)) as x64, as this engine branch cannot run 32 bit game DLL's (**I might be able to provide  the compiled engine DLL**)
 3. Download the required files for every map/model to fully utilise the ray traced engine.
 4. **Most importantly, have some patience with the game. A lot of features that bshift uses are non-existent/broken in this engine fork, and I do not posses enough skills/knowledge to fix them/add them into the engine (I'm a web developer, not a C developer) [Although I might learn one day]**



<br><br><br><br>

## I am using this as an opportunity to learn!
### This means this will never reach professional quality like the main game converted by sultim-t himself!
#### I am only here to learn how to mess around with GLTF, PBR textures and RTGL1.
#### Do not expect professional grade quality from this conversion, it is my first time doing this sort of stuff.


# Work checklist
 - [x] ***ba_tram1***
 - [x] ***ba_tram2***   
   - [x] **Fix the func_illusionary at the start of the map [The giant black rectangle]** Fixed by hex editing the map to remove the entity itself.
   - [x] **Fix missing textures**  This turned out to be a user issue, as I didn't restart Blender every time I worked on a new map, Blender thus kept all of the old material files which caused conflicts in the newly imported GLTF files and renamed all duplicate materials causing the game to not know where to find the files for them
	- [ ] **Fix RT fireflies at the start of the map** (The sun LOVES to leak on this one)
- [x] ***ba_tram3***
  - [x] **Add some RT sprinkle here and there, as the map is incredibly bland and has a lot of phantom lights**
- [x] ***ba_security1*** [Short in-between map, no work needed other than exporting the gltf]
- [ ] ***ba_security2***
  - [x]  **Again as with ba_tram2, the map requires a lot of fixing missing/incorectly exported textures** 
  - [ ] **Fix the lights in the elevator that goes to the armory**
  - [x] **Add some RT sprinkles again**
