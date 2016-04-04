# XM8_repairMate

Repair Mate script for Exile mod
This script adds more advanced repair mechanics to Exile.
Deferent items can be used to perform repair, some will be
consumed as materials others are used as tools.
There are 5 types of repairs for cars. They are engine, wheels, glasses,
fuel and body. Script is highly configurable, and allows to set exact
material costs and reqiured tools for deferent types of repair.
It is allowed to have materials and tools inside vehicle being repaired.
Script requires improved XM8 apps to work.

Authors
art and design - z3ro
code - vitaly'mind'chizhikov

Future plans
1. Support for helicopters (mostly done, will be added soon)

INSTALLATION
1) Paste XM8_repairMate folder to the root of mission folder.
2) Add following lines to XM8_apps\XM8_apps_config.sqf. 
	XM8_apps_app1 = [
		"Repair Mate",
		"XM8_repairMate\icons\repairMate_icon.paa",
		{"" execVM "XM8_repairMate\scripts\XM8_repairMate_init.sqf"}
	];
		Change "XM8_apps_app1" to application number you like, from 1 to 13.
3) Add class "repairMate" to class CfgXM8 inside XM8_apps_sliders.hpp
	This step is done by default.
	class CfgXM8 {
		...
		class repairMate {
			controlID = 960050;
			title = "Repair Mate";
		};
		...
	};
4) Change XM8_repairMate\XM8_repairMate_costConfig.sqf to your liking.
5) Enjoy!


