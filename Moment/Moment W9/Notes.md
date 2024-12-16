## December 13, 2024

* Via different composite modes in my comp 1 - you can get different kind of outputs
	- Set to multiply, to effectively use your objects as a mask on your main texture
	- set to add, and nullify main texture to only use your object texture and use each independently
	- set to subtract, and white out each object texture to have your main texture only in the background, and not on the objects

* I wish I could do this complex compositing from within Kantan Mapper, cause right now I'm having to use two kantanmappers, one for all the objects and one for just the main table
	- the one for the main table is used for remapping the main texture that's coming in
	- and the one for the objects is being used as a mask on this main texture

 * Right now the style that i'm mainly going for is to just composite the main texture, that is filling the whole table, with my object masks in different ways
	- this means that the main texture does not get transformed according to the uv map of each object - i.e. doesn't shrink to fill only the object
	- I chose this cause it looks better due to the objects all having different sizes
	- but if I do want to actually make stuff that is shrunk to the uv map of the object, I can just do that within the object texture on its own, and composite in add mode

