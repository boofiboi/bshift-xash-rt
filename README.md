
# bshift-xash-rt
### Half Life: Blue Shift ray traced using the [xash-rt](https://github.com/sultim-t/xash-rt) engine built by [sultim-t](https://github.com/sultim-t).

#### This repo is used as a staging ground for all the changes I need to do to maps, files, models in the Blue Shift campaign for Half-Life in order to get it functional and playable in the engine. [Opposing force might've been easier to start with, but YOLO]




### What does this require?
#### You will need to:

 1. Compile hlsdk-portable's bshift branch (Found [here](https://github.com/FWGS/hlsdk-portable/tree/bshift)) as x64, as this engine branch cannot run 32 bit game DLL's
 2. Use a tool such as [bspfix](https://valvedev.info/tools/bspfix/) to convert all Blue Shift maps into a format that the new engine understands.
 3. Download the required files for every map/model to fully utilise the ray traced engine.
 4. **Most importantly, have some patience with the game. A lot of features that bshift uses are non-existent/broken in this engine fork, and I do not posses enough skills/knowledge to fix them/add them into the engine (I'm a web developer, not a C developer) [Although I might learn one day]**

#### I might be able to provide  the compiled engine DLL, but you have to get the rest.


<br><br><br><br>

## I am using this as an opportunity to learn!
### This means this will never reach professional quality like the main game converted by sultim-t himself!
#### I am only here to learn how to mess around with GLTF, PBR textures and RTGL1.
#### Do not expect professional grade quality from this conversion, it is my first time doing this sort of stuff.

 - [x] ***ba_tram1***
 - [ ] ***ba_tram2***   
   - [ ] **Fix the func_illusionary at the start of the map [The giant black rectangle]** (Probably impossible without altering engine code, maybe I can force the texture it uses  to be translucent/invisible [Still haven't figured out how, textures.json doesn't seem to know it exists])
   - [ ] **Fix missing textures** (Involves remaking the base texture thats missing as a .ktx2 file, since a texture missing = it is an invalid .tga that the base engine just ran with, RTGL1 however does not and doesn't properly export it, which causes the .gltf scene for the map to not include it, and it just appears as a gray texture)
	- [ ] **Fix RT fireflies at the start of the map**
- [x] ***ba_tram3***
  - [ ] **Add some RT sprinkle here and there, as the map is incredibly bland and has a lot of phantom lights**
- [x] ***ba_security1*** [Short in-between map, no work needed other than exporting the gltf]
- [ ] ***ba_security2***
  - [ ]  **Again as with ba_tram2, the map requires a lot of fixing missing/incorectly exported textures** 
  - [ ] **Fix the elevator lights that go to the armoury**
  - [ ] **Add some RT sprinkles again**
