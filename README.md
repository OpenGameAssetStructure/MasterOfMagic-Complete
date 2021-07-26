# MasterOfMagic-Complete
The MasterOfMagic-Complete repository tries to agregate various Master of Magic asset, data and engine repositories into one complete project. 
The MasterOfMagicCollection repository tries to agregate various Master of Magic implementstions into one big project.
The standard folders should be:
* assets
* data
* engines
* scripts
* setup
* sources

## LFS repositories
The assets, engines and setup are generaly made up of binary files and would need Large File System (LFS) repositories. The data, scripts and sources are generaly made op of text that can use normal repositories.

## Formats
The most common asset formats are PNG and JPG as most every image viewer can open those. Most open source projects use PNG as it has an alphachannel and is pixel friendly.

The most common data formats are XML, JSON and YAML. MoM-IME uses XML. OpenMoM uses YAML and that is much easier to read. Defining a JSON schedule could benefit those that try to tweak the data.

The most common script formats in gaming are Python and Lua. C# is also used as a scripting language, but that gets compiled. No MoM implemtatation uses scripting jet.

The most common game engines are Unity and Unreal, with Godot being a great open source runner up. These are are only engines for the game as they can run the game, probably with the help of a lot of script. The compiled code of MoM-IME and OpenMoM are the currently available game engines. Idealy a build of one of those project whould place the output in a versioned folder in the engines folder.

## Implementation independant subrepositories
The assets, data and scripts are indpendent of the implementation. Having those in seperate repositories would make it easier to reuse for other engine implementations.
These can also be distributed as a zip and unpacked in memory by the engine. This would probably be faster as reading small files from disk as processors can unpack an archive very quickly.

The Theatrical Approach should be used to structure the assets, data and scripts. This would create a folder structure with the folders names related to the story of the game. The folders would be categories of specific dimentsion and thus describe an aspect of an asset, data file or script. See "Game Assets folder structuring approaches and dimension. Introducing the Theatrical approach" for details.

## Implementations
Currently there are a number of implementations of Master of Magic:
* The original
* Caster of Mageic
* MoM-IME (Java project on SourceForge)
* OpenMoM (C++ on GitHub)
* master-of-magic (ocaml on GitHub)
* Master of Magic 2 is being worked on

Only MoM-IME, master-of-magic and OpenMoM are open source so only those 3 could land in this repository.
There might be a C# version under way as C# is used by many game engines these days.
