want to add some stuff for this mod?
Great! here are some guidelines.
put ALL config's that you add in the RTG(USERS CONFIG INSTALL HERE) file
if you want to be ambitious.. you can use github and push a pull request.
there is 2 parts you need to know. RTGM for general mods and RTGF for karbonite or any resource that can be drilled / mined
here is how you Edit a config :

@PART[RTGM]:NEEDS[mod file name]
{

	MODULE
	{
		name = ModuleGenerator
		isAlwaysActive = false
		activateGUIName = {Name of mod} On
		shutdownGUIName = {Name of mod} Off
		actionGUIName = Toggle {Name of mod} Generator
		OUTPUT_RESOURCE
		{
			name = ElectricCharge
			rate = 1000000.00
		}
	}
}



You can copy paste OUTPUT_RESOURCE  as MANY TIMES AS YOU WANT.

FINAL notes:
DO NOT EDIT DIRECTLY the parts folder or I will reject your pull request.
DO NOT EDIT ANY OTHER FOLDERS except for the .cfg in the folder specified above

Thats it! ~joshwoo69